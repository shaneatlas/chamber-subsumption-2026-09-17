# Archived-workspace evidence for the cross-seat reconciliation

Prepared September 17, 2026. Local, read-only archive inspection. No source script executed. These are historical captured bytes, not a new GitHub fetch or live Source result.

## Archive identity

`1jsB2l4DsJnSRLGi-grok-workspace.zip`
SHA-256: `b674592b7d39a7cbe4be2e26126a593d69db1a499c379731c9e786823bfc7e83`

## Captured code identity

Repository capture: `797eb52f45101a98cedc9c3275d822cfda0d3a85`; the other capture at `9266d8cd31a56ecdf43d0830ab69f66a4af23ab4` has identical source bytes.
Path: `scripts/enrich_with_voyage.py`
Git blob: `ae50f42120977657220f50efbd9299263c3dd256`
Source SHA-256: `18f386faa5a75eafc15c3a4db7cf3bf8b4c340611a6b0d30bf1afa42dbae23c5`

The Git blob SHA was recomputed over the captured UTF-8 file bytes and matches the envelope. This establishes internal identity, not independent authentication of the captured service response.

## Selected exact source lines

### Generation anti-join

Original source lines 69–79.

```text
069:             if entity_ids:
070:                 cur.execute("""
071:                     SELECT ce.id, ce.title, LEFT(ce.content, 8000) AS content
072:                     FROM corpus_entities ce
073:                     LEFT JOIN corpus_embeddings em
074:                       ON em.entity_id = ce.id AND em.model = %s
075:                     WHERE ce.id = ANY(%s)
076:                       AND ce.content IS NOT NULL AND LENGTH(ce.content) > 50
077:                       AND em.entity_id IS NULL
078:                     LIMIT %s
079:                 """, (VOYAGE_MODEL, entity_ids, int(limit)))
```

### Entity-only embedding persistence

Original source lines 130–146.

```text
130: def persist_embeddings(entities: list, embeddings: list) -> list:
131:     """Upsert vectors; return exact persisted entity IDs (RETURNING)."""
132:     import hashlib
133:     persisted = []
134:     with db_connection() as conn:
135:         with conn.cursor() as cur:
136:             for e, vec in zip(entities, embeddings):
137:                 text = f"{e['title']}\n\n{e['content'][:4000]}"
138:                 cur.execute("""
139:                     INSERT INTO public.corpus_embeddings (entity_id, embedding, model, content_hash, created_at)
140:                     VALUES (%s, %s::vector, %s, %s, now())
141:                     ON CONFLICT (entity_id) DO UPDATE
142:                         SET embedding = EXCLUDED.embedding, model = EXCLUDED.model,
143:                             content_hash = EXCLUDED.content_hash, created_at = now()
144:                     RETURNING entity_id""",
145:                     (e["id"], "[" + ",".join(f"{x:.6f}" for x in vec) + "]",
146:                      VOYAGE_MODEL, hashlib.md5(text.encode()).hexdigest()))
```

### Global pair query and error propagation

Original source lines 188–217.

```text
188: def compute_global_pairs(entities: list, embeddings: list, threshold: float, k: int = 8):
189:     """kNN each NEW embedding against the WHOLE corpus_embeddings via pgvector —
190:     closes the intra-batch-only pair scope (S2026-07-16 finding: chunk-clique
191:     topology; pairs never crossed chunk or corpus boundaries).
192:     Returns id-keyed pairs [(id_a, id_b, sim), ...]."""
193:     pairs = []
194:     with db_connection() as conn:
195:         cur = conn.cursor()
196:         try:
197:             from core.vector_guard import apply_hnsw_gucs
198:             apply_hnsw_gucs(conn)
199:         except Exception:
200:             pass
201:         for ent, vec in zip(entities, embeddings):
202:             vs = "[" + ",".join(f"{x:.6f}" for x in vec) + "]"
203:             try:
204:                 cur.execute(
205:                     """SELECT entity_id, 1 - (embedding <=> %s::vector) AS sim
206:                        FROM corpus_embeddings
207:                        WHERE entity_id <> %s
208:                        ORDER BY embedding <=> %s::vector LIMIT %s""",
209:                     (vs, ent["id"], vs, k))
210:                 for eid, sim in cur.fetchall():
211:                     if sim is not None and float(sim) >= threshold:
212:                         a, b = sorted((ent["id"], eid))
213:                         pairs.append((a, b, float(sim)))
214:             except Exception as e:
215:                 print(f"  global-kNN error for {ent['id'][:30]}: {str(e)[:80]}")
216:                 conn.rollback()
217:     return sorted(set(pairs))
```

### Existing relationship writer

Original source lines 241–272.

```text
241: def _write_id_edges(edge_params: list) -> int:
242:     """Batched id-keyed SIMILAR_TOPIC MERGE; counts REAL server-side writes."""
243:     try:
244:         from core.neo4j_driver import run_query
245:     except ImportError:
246:         print("  Neo4j driver not available — skipping projection")
247:         return 0
248:     created = 0
249:     EDGE_BATCH = 200
250:     for k in range(0, len(edge_params), EDGE_BATCH):
251:         batch = edge_params[k:k + EDGE_BATCH]
252:         try:
253:             rows = run_query("""
254:                 UNWIND $edges AS e
255:                 MATCH (a:CorpusEntity {id: e.id_a})
256:                 MATCH (b:CorpusEntity {id: e.id_b})
257:                 WHERE a <> b
258:                 MERGE (a)-[r:SIMILAR_TOPIC]-(b)
259:                 SET r.weight = e.weight,
260:                     r.source = 'voyage_enrichment',
261:                     r.model = $model
262:                 RETURN count(r) AS written
263:             """, {"edges": batch, "model": VOYAGE_MODEL})
264:             try:
265:                 created += int(rows[0]["written"]) if rows else 0
266:             except Exception as exc:
267:                 raise ValueError(f"unreadable_edge_write_count: {exc}") from exc
268:         except ValueError:
269:             raise
270:         except Exception as e:
271:             print(f"  Edge batch error at {k}: {str(e)[:100]}")
272:     return created
```

### Flag contract

Original source lines 313–316.

```text
313:     parser.add_argument("--global-pairs", action="store_true",
314:         help="ALSO kNN each new embedding against the whole corpus_embeddings "
315:              "(pgvector) instead of only the in-batch matrix — cross-chunk + "
316:              "cross-corpus SIMILAR_TOPIC edges (S2026-07-16).")
```

### Classification and early exit

Original source lines 364–386.

```text
364:     entities = get_entities_to_embed(args.category, args.limit, entity_ids=entity_ids or None)
365:     selected_ids = [str(e["id"]) for e in entities]
366:     receipt["selected_ids"] = selected_ids
367:     print(f"  Entities to embed: {len(entities)}")
368: 
369:     missing, skipped = ([], [])
370:     if entity_ids:
371:         missing, skipped = _classify_targets(entity_ids)
372:         receipt["missing_ids"] = missing
373:         receipt["skipped_existing"] = skipped
374:         receipt["ineligible_ids"] = [
375:             i for i in entity_ids
376:             if i not in selected_ids and i not in missing and i not in skipped
377:         ]
378: 
379:     if not entities:
380:         print("  Nothing to embed.")
381:         if entity_ids and not missing and skipped and not receipt["ineligible_ids"]:
382:             _finish("EMPTY_ALREADY_SATISFIED", 0)
383:         if entity_ids:
384:             receipt["failed_ids"] = list(missing or entity_ids)
385:             _finish("FAILED" if missing else "PARTIAL", 3 if missing else 2)
386:         _finish("EMPTY_ALREADY_SATISFIED", 0)
```

### Pair invocation and final outcome

Original source lines 419–453.

```text
419:     persisted_ids = persist_embeddings(entities[:len(all_embeddings)], all_embeddings)
420:     receipt["persisted_ids"] = [str(x) for x in persisted_ids]
421:     print(f"  Persisted to corpus_embeddings: {len(persisted_ids)}")
422: 
423:     pairs = []
424:     created = 0
425:     try:
426:         if args.global_pairs:
427:             gp = compute_global_pairs(entities[:len(all_embeddings)], all_embeddings, args.threshold)
428:             print(f"  Global corpus-wide pairs (>={args.threshold}): {len(gp)}")
429:             if gp:
430:                 gp_params = [{"id_a": a, "id_b": b, "weight": round(sim, 4)} for a, b, sim in gp]
431:                 receipt["edges_attempted"] += len(gp_params)
432:                 created += _write_id_edges(gp_params)
433:         pairs = compute_similarities(embeddings_array, args.threshold)
434:         print(f"  Similar pairs (>={args.threshold}): {len(pairs)}")
435:         if pairs:
436:             receipt["edges_attempted"] += len(pairs)
437:             created += project_edges_to_neo4j(entities, pairs)
438:             print(f"  Neo4j edges created: {created}")
439:         receipt["edges_observed"] = created
440:     except ValueError as exc:
441:         if "unreadable_edge_write_count" in str(exc):
442:             receipt["edges_unreadable"] = True
443:             print(f"  ERROR: {exc}")
444:             receipt["failed_ids"] = failed_ids
445:             _finish("PARTIAL", 2)
446:         raise
447: 
448:     receipt["failed_ids"] = failed_ids
449:     if failed_ids or missing or len(persisted_ids) < len(selected_ids):
450:         print(f"\n=== PARTIAL: {len(persisted_ids)} persisted, failed={failed_ids[:8]} ===")
451:         _finish("PARTIAL", 2)
452:     print(f"\n=== COMPLETE: {len(all_embeddings)} embedded, {len(pairs)} pairs, threshold={args.threshold} ===")
453:     _finish("COMPLETE", 0)
```

## Workspace scope

`package.json`: name `app-builder-workspace`; `build` runs a Vite build and then `npm run db:migrate`. No package command was executed.
`src/lib/chamber.ts`, lines 1–13 and 127–199: the reviewed data exports import local `src/data/*.json` snapshots.
`src/data/membrane.json`: `observed_at=2026-09-17T07:02:00Z`; `claim_ceiling=PACKAGE_UPDATED_CONTROLLER_ROUTE_DENIED`; historical graph-only `closure.next` remains present.
`src/data/pulse.json`: `observed_at=2026-09-17T06:09:50Z`.
The captured repository-tree response marks `truncated=true`; it is not a full source-tree census.
No captured B8 registered-hook body, raw timing output, or numerical organizational ranking DAG was recovered in the scoped search. The new user report remains their source.

## Captured body consistency

20 bodies, 16 distinct Git blobs, 20 matching envelope hashes. Not test cases, tasks, or live execution witnesses.
