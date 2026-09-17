# Source — pairs-only reuse: one existing-owner implementation delta

**Date:** September 17, 2026.  
**Controlling interpretation:** accepted R4, under the existing aligned SLP-1 takeover.  
**State of this deliverable:** implementation contract prepared; no Source code modified and no Source tests or live data operations run here. This is not R5, a replacement architecture, or another package-readiness program.

## 1. What the latest source inspection settles

[OPERATOR-REPORTED SOURCE INSPECTION] At repository prefix `9266d8cd`, `scripts/enrich_with_voyage.py` blob prefix `ae50f421…` selects generation candidates by anti-joining the requested IDs against `corpus_embeddings` for the requested model. If none remain, it exits `EMPTY_ALREADY_SATISFIED` before the `--global-pairs` branch. `compute_global_pairs` receives newly minted in-memory vectors; the inspected path does not reload satisfied anchors from PG. The current flag inventory contains no pairs-only or reuse-existing mode.

This advances the earlier hypothesis into a reported, source-bound control-flow defect. It does not establish that a newer checkout has the same bytes; rebind the actual current owner without repeating the history audit. Do not invent complete hashes from abbreviated identities.

The three products remain independent:

| Product | Reported batch state | Repair implication |
|---|---|---|
| Embedding generation | 23 already satisfied in PG | Reuse only after content/representation validation; no Voyage call for this repair. |
| Qualified cross-corpus pair computation | Not run | Run for the exact valid requested anchors, not only newly embedded rows. |
| Cosine edge projection | Not run | Publish qualified pairs through the existing writer and observe their actual meaning. |

The reported 162 type-cluster edges are not the missing cosine product. The retired/destroyed Aura `2423a9f4` inventory is historical according to the latest operator report, not a destination to revive or probe for this repair. Resolve the current intended graph destination from the existing owner.

## 2. Execution capability in this preparation session

All 32 currently discoverable `the_source` action schemas were inspected. They include discovery and product reads/composites but no repository-file read, checkout, generic Source invocation, or repository-edit contract. No Source action was invoked. The visible working directory contains supplied artifacts; no authenticated Source checkout was established. An API tool-count difference does not prove a server regression or change the earlier 42/42 observation.

The R4 attachment was read in full. Only public primary documentation was consulted to check the quoted MERGE/SET semantics and PG query-setting behavior. No attempt was made to route a repository task through Drug/Gene search, an unconstrained composite parameter, a chat endpoint, or the previously denied `source-e2e` operation. There is consequently no honest current-repository patch or test result to report from this session.

## 3. Minimal orchestration change

Keep the existing selector, vector reader, kNN owner, edge writer, receipts, and parent ingest. Change their product dependency, not their ownership.

### 3.1 Retain requested identities before generation filtering

Resolve the exact 23 corpus IDs from the owning batch, not queue range 5168898–5168920. Carry source document/section, current content hash, model, dimension, input role/preprocessing where recorded, quality eligibility, permission scope, and vector version/hash. Identify missing, stale, incompatible, duplicate, or unauthorized rows explicitly. Loading `entity_id, embedding` alone is insufficient when the current row's content binding has not also been verified.

Do not rely on array position to join reused/new vectors to entities. Use the existing canonical key and representation identity. Equal lengths do not establish equal content. A model string alone does not prove a current vector.

### 3.2 Separate generation input from pair input

Generation candidates remain the missing/stale items eligible for a separately requested production operation. Pair anchors are all valid requested embeddings: reusable persisted values plus successfully produced values when ordinary combined generation is actually requested.

For this batch, enforce reuse-only behavior: all admitted pair anchors come from existing qualified PG vectors. Missing or stale vectors are unresolved producer obligations; they must not silently trigger Voyage to make the repair pass.

The generation-only empty result must not exit the process before separately requested pair work and receipt finalization. Conversely, a caller requesting only generation should not acquire an unrequested global pair computation. Preserve existing defaults and explicit opt-in behavior.

An explicit reuse-only flag could be added if that is the smallest safe CLI contract, but it does not exist in the inspected version. Do not publish a command using that flag until it is implemented and its parser tested. Extending the current `--global-pairs` semantics is another option if it preserves the no-generation guarantee for this operation and compatibility for ordinary callers.

### 3.3 Keep stage order correct

The reported parent order is embedding production in phase 3.5, node projection in phase 4, then similarity work in phase 5b. A MATCH-only edge writer cannot publish a relationship before required endpoint nodes exist.

For these 23 anchors, nodes are reported present, but current exact endpoint/version readback is still required. For new ingest compatibility, stage pair computation when its vectors become available and publish only once the required endpoint projection exists. A missing endpoint is pending/failed edge materialization, not a successfully completed zero-neighbor search.

Do not merely add `--global-pairs` to every phase-3.5 call: that both widens the workload and can preserve the zero-observed-edge failure on newly projected nodes. Reuse the existing stage/receipt owners instead of adding a queue or moving all work into a new pipeline.

## 4. Qualify the existing kNN path before broadening who can reach it

The latest operator report says the existing query excludes only the anchor ID, then orders by cosine distance and limits to k. Its reported absence of model and authorization scoping is a defect in the proposed reuse path's prerequisites, not permission to run it unchanged over the whole table.

The 23 IDs are anchors. The candidate universe is the larger same-space population actually authorized for the selected product. It is not a 23-document clique and is not unrestricted simply because the flag is named `global-pairs`.

Bind these rules at existing owners:

- **Representation:** the actual compatible model/version, dimension, normalization/preprocessing and content state. Same-dimensional models are not interchangeable.
- **Access:** current tenant/principal/population restrictions at retrieval and at graph publication. An authorized read of two sources does not automatically authorize a durable cross-scope relationship exposed to other readers.
- **Product:** the self-ID exclusion and intended same-document policy. For cross-document discovery, exclude same-parent fragments before top-k or explicitly account for their removal; do not spend the candidate window on the original island.
- **Domain:** apply the task's actual permitted domain policy. Do not silently require same-domain membership when the authorized product is cross-domain discovery.
- **Resources:** admitted anchor count, candidate depth, query/operation deadlines and bounded retries. At most `anchor_count × k` returned directed pair candidates is a result bound, not a database-work bound.

Keep raw ascending cosine distance in the relevant `ORDER BY`; a display similarity in SELECT does not alter it. Inspect the actual plan and filtered behavior rather than asserting HNSW use from query text. No new index or DDL is included. [W3]

Use transaction-local search settings inside the same checked-out connection and actual transaction as the kNN query. Test restoration after success, failure and cancellation, including the next borrower and a previously contaminated session baseline. Do not create an incompatible nested transaction inside a caller-owned transaction. [W4]

`assert_knn_complete` remains a cardinality guard, not an exact-recall evaluator. Keep pre-threshold candidate sufficiency, post-threshold qualifying pairs, and vector-recall evidence distinct. A sufficiently executed search can legitimately have zero above-threshold pairs. Neither 0.65 nor 0.80 is a required edge-production quota. Underfetch or a timed-out search must not be labeled a fully assessed absence.

## 5. The quoted edge pattern does not by itself separate provenance

[NEW INFERENCE FROM THE SUPPLIED QUERY, CHECKED AGAINST CYPHER SEMANTICS]

The supplied relationship pattern is:

`MERGE (a)-[r:SIMILAR_TOPIC]-(b)`

It does not include `source`, model or another provenance identity in the matched pattern. Neo4j MERGE can therefore bind an existing relationship of that type between those bound endpoints, including a type-cluster relationship. An undirected pattern searches both directions. [W1]

If `r.source`, `r.model` and `r.weight` are then assigned unconditionally or on match, the existing relationship's provenance/value can be overwritten. If they are assigned only on create, matching a type-cluster edge can instead prevent creation of the intended separate cosine edge. The full setter path and any additional guards were not supplied here, so neither failure is claimed as a separately observed live incident. [W1; W2]

This does not undo the useful endpoint safeguard: MATCHed endpoints do not require node creation in the quoted path. It means **no-node-mint and no-provenance-overwrite are separate predicates**.

Required implementation behavior:

1. Bind edge identity through the existing owner's representation of endpoints, permitted scope, generator and compatible representation. Reuse its established key/provenance mechanism; do not automatically introduce another label, table or constraint.
2. Ensure a type-cluster relation cannot satisfy the cosine-edge match or be silently relabeled/reweighted as Voyage output.
3. Ensure the downstream consumer distinguishes generators or explicitly aggregates them without treating duplicate source-derived relationships as independent evidence.
4. Retain legitimate replay/update behavior for an existing cosine relationship. Do not include mutable similarity or the current run ID in a MERGE key merely to force every run to create another edge.
5. Resolve direction, duplicate unordered pairs, multiple source versions, concurrency and endpoint uniqueness under the current contract. The cosine measure's symmetry does not make the top-k neighbor selection itself symmetric.

The minimal decisive fixture seeds a type-cluster edge for the exact same endpoints, runs the proposed writer, and checks that its original identity/provenance/weight remain intact while the intended qualified cosine product has an unambiguous owner-visible representation. Run it twice and through the real consumer. This is a designed test, not an executed result.

Missing endpoints require a typed exact-ID disposition and zero unintended nodes. Zero writer rows must not be conflated with zero qualified pair candidates. No automatic legacy-edge cleanup or global deduplication is authorized by this repair.

## 6. Product receipts and phase 5b

Map these facts into existing receipt fields or extend that owner minimally; the names here are semantic fields, not new canonical status enums:

- Generation requested or not; reused, generated and unresolved anchors by identity.
- Pair computation requested; eligible anchors/universe; actual representation/filter/budget; candidate search completeness and limitations.
- Staged qualifying pairs, including score basis and same-parent ancestry.
- Graph publication attempted, newly created, already-current, changed, missing endpoints, conflicts and unresolved effects.
- Consumer result and its provenance/qualification.

The generation phase may continue reporting `EMPTY_ALREADY_SATISFIED`, but that must not be the aggregate result of an operation with unperformed requested pair work. Do not change aggregate exit behavior without updating the parent consumer and its tests.

Phase 5b must select its availability probe by the requested product. For PG-vector-to-edge work, it reads the PG representation and an identity-bound pair result. It does not re-test Aura `n.embedding` as the prerequisite. Missing pair evidence is pending/not-run, not a factual absence and not automatic authorization to run an unbounded global operation.

Type navigation can remain a separate available product, but its use and incomplete semantic work must remain visible. A qualified zero-neighbor result need not create a cosine edge. An unqualified search cannot be hidden by a successful type-cluster fallback.

## 7. Regression and consumer acceptance — all unrun here

| Case | Required observation |
|---|---|
| All 23 already satisfied; pair work requested | Zero Voyage calls; all qualified anchors reach pair computation; receipt does not stop at generation skip. |
| Generation-only caller, no missing vectors | Existing no-generation outcome retained; no unrequested global pair work. |
| Missing/stale vector in reuse-only mode | Exact unresolved ID; no implicit generation; admitted partial behavior is explicit or the batch stops under its contract. |
| Ordinary mixed new/reused call | Each vector joins to the correct ID/version; no duplicate anchor or position-based misassociation. |
| Foreign model/unauthorized population/same-parent-only candidates | Apply the actual restrictions before accepting pairs; no implicit island rebuild or cross-scope link. |
| Selective underfetch and valid zero-neighbor case | Distinct results; cardinality sufficiency not labeled recall; no forced threshold lowering. |
| Session success/error/cancel then another borrower | Query-local settings do not contaminate the next request. |
| Same endpoints already have type-cluster edge | Original edge meaning remains intact; cosine product is separately identified and correctly consumed. |
| Replayed cosine pair, reversed input, competing attempt | Existing owner idempotency/direction/concurrency behavior holds; no duplicate evidence inflation. |
| Missing or conflicting endpoint/version | No node mint; exact publication failure remains open. |
| New ingest stages 3.5 → 4 → 5b | Edge publication waits for endpoints; generation success does not conceal absent publication. |
| Partial edge publication then resume | Reconcile actual target before retry; resume only unresolved eligible products. |
| Phase 5b sees valid PG vectors but no Aura vector property | Correctly uses the selected PG pair contract; no inappropriate property-copy prerequisite. |
| Real reader inspects cosine and type-cluster products | The reader preserves basis, source and confidence ceiling, rather than treating both as cosine evidence. |

A test fixture with a known qualifying pair can establish the positive writer/consumer behavior even if the real batch correctly yields no qualifying neighbors. Neither fixture success nor real edge presence establishes full-corpus ANN recall or beneficial learning on its own.

## 8. Continuation to the authorized Source work session

Consume this delta under the accepted R4 and existing root takeover. Do not restart retrospective or graph-method research.

1. Read the current `enrich_with_voyage.py`, its parser/target classifier, `compute_global_pairs`, full `_write_id_edges` query, parent phase 3.5/4/5b path, vector guard and relevant queue consumer. Bind the actual tested checkout, owner and batch identities. Preserve other-seat work. Do not reset to a historical prefix.
2. Apply one coordinated existing-owner change: separate generation candidates from valid requested pair anchors; qualify the existing candidate search; stage pair evidence; make edge identity preserve generator provenance; and change 5b/receipts to inspect the selected product. Multiple touched files can be one logical owner repair when they implement that same producer–consumer contract.
3. Implement and run the relevant regression cases above using the current repository's test interfaces and disposable targets. Do not fabricate passing results from this document or expose production connection defaults to fixtures.
4. Once permitted under the existing target-specific authority, execute only the actual qualified 23-anchor reuse operation. No Voyage, re-ingest, index DDL, Aura vector SET, GDS, FastRP, GNN, Nornic rebuild/mirror, provider change or unrelated schema migration.
5. Process only queue rows whose current payload/handler requires the corrected product. Preserve exact queue ownership, lease/version and target readback. Do not drain unrelated alignment work through the new pair operation merely because its row count is 23.
6. Read the actual cosine/type provenance through the intended consumer and retain the outcome. Queue completion, pair count and edge count remain different evidence.
7. Keep 3pass DEFERRED, conferral/release adjudication separate, and `dwq#3501` independently owned. No push/merge, another seat's writer, or broader release grant is supplied by this artifact.

The later SLP-1 lesson remains product-aware reuse: generation can be satisfied while a distinct consumer product remains incomplete. Its beneficial later use must be measured under the existing learning protocol, not inferred from this repair's new receipt.

## 9. Evidence and scope

**U1:** latest user report beginning “R4 is accepted. Copy-first is dead,” including code excerpts and abbreviated source identities. Its repository findings are source-bound reports by the operator; the live file was not independently fetched in this session.

**P1:** accepted `SOURCE_REPRESENTATION_AND_TERMINATION_R4_2026-09-17.md`, read in full through Files. Its prior no-pairs-path hypothesis is narrowed by U1, not deleted. Exact file hash is in the companion preparation record.

**W1:** Neo4j Cypher Manual, MERGE — https://neo4j.com/docs/cypher-manual/current/clauses/merge/ . Selected existing-relationship and undirected-relationship semantics checked September 17, 2026. Not a Source query run.

**W2:** Neo4j Cypher Manual, SET — https://neo4j.com/docs/cypher-manual/current/clauses/set/ . Selected relationship-property update semantics. Not a Source writer inspection.

**W3:** pgvector maintainer README — https://github.com/pgvector/pgvector . Selected index-compatible ordering, filtering and iterative-scan behavior; installed extension/version remains to bind.

**W4:** PostgreSQL SET — https://www.postgresql.org/docs/current/sql-set.html . Transaction-local versus session scope. Not a live pool test.

**Sources ·** U1, P1, current tool-schema discovery and W1–W4 at their stated ceilings.  
**Assumptions ·** The reported code defect is the current repair target until the real execution checkout confirms or supersedes it. Actual corpus IDs, source/vector hashes, target and full writer behavior remain to bind.  
**Next action ·** Implement the coupled selection/pair/projection/consumer delta in the authorized checkout; first prove it does not overwrite a pre-existing type-cluster edge. No Source action occurred here.
