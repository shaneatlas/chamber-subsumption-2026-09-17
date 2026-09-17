# Source — retrieval fidelity, Nornic execution contracts, and coherent metric publication

**R3 supplemental reconciliation · September 17, 2026**  
**State: PREPARATION_ONLY / NO_SOURCE_ACTION / NO_RECALL_RESULT**  
**Parent: accepted R2 graph-plane interpretation under the existing SLP-1 aligned takeover.**

This is a localized supplement, not another replacement architecture, executable patch, permission grant, index-rebuild decision, or public capability-status change. It reconciles the three latest operator contributions together: vector quantization and pgvector; recall and the newly reported embedded-suite inspection; and the Nornic cookbook/fork distinction. The existing root takeover, all twelve work packages, and its beneficial-reentry requirement remain unchanged.

## 1. Governing finding: preserve the information a later decision needs

The relevant utility is not maximum ANN speed, a new quantization type, a longer cookbook, or a fresher timestamp. It is that an authorized task receives the evidence and qualified routing signals it needs, and that later work can use a verified procedural lesson without repeating incompatible or unsafe choices.

There are now three closely related, but non-interchangeable, acceptance questions:

1. **Execution fidelity:** did the effective query, after scope and policy were applied, use a supported owner and execution contract on the installed build?
2. **Retrieval fidelity:** did the candidate generator retain the required exact neighbors within the declared eligible universe, and did the composed retrieval path supply useful evidence?
3. **Publication fidelity:** did a consumer receive the metric fields and completeness guarantees that its decision actually requires, rather than infer them from a global timestamp?

These questions fit existing owners. They do not require a new skill marketplace, an additional ANN store, a new metric database, or a universal graph-first route. A failure in one must not automatically be attributed to the learner: failed embedding ingestion, unavailable search, an invalid filter, and a bad memory policy require different corrective actions.

**Preparation decision:** retain the reported incumbent scalar Aura index; prepare a properly scoped recall experiment; bind Nornic documentation, local skill, installed implementation and effective query separately; and finish the existing suite-to-routing consumer trace. Do not rebuild, invoke a suite, change routing, or change public `graph_gds` from this document.

## 2. Evidence ledger: what advanced and what did not

### 2.1 Latest operator records

| Record | New information supplied | Evidence ceiling in this supplement |
|---|---|---|
| U1 — quantization/pgvector contribution | Reported Aura `2423a9f4`, Vector Optimized 8GB, ten ONLINE indexes, scalar `vector-3.0`, roughly 3.92M 1024-dimensional Voyage-3 corpus vectors; comparisons with pgvector | Operator-reported Source inventory and technical argument. Public documentation was checked; Source database and private file were not independently read here. |
| U2 — recall plus suite inspection | No bound recall fixture, a five-row smoke; reported script inspection at repository `c1422791e08498ac6615973b1f5dcf951a1df73d`, blob prefix `27ba5106…`; `.write` calls, sequential partial completion and global timestamp; consumer copy still unbound | User-bound source inspection, as reported. Not an independently executed suite or observed consumer. The no-fixture statement is not upgraded to a universal six-month absence proof. |
| U3 — Nornic cookbook | Upstream commit `e917408d61c32eb537082e7c905a6b1c1d4ff951`, file hash prefix `c99acbf5…`; condensed Source fork, missing local cookbook link, named routes and pitfalls | Reported pinned upstream documentation plus Source-fork inspection. Current public `main` corroborates several descriptions but does not verify the exact pin or Source's installed Nornic. |
| R2 | Existing per-owner interpretation and fourteen dispositions | Accepted preparation baseline, not Source execution. |
| SLP-1/root takeover | Work, evidence, evaluation, authority, release and beneficial-use requirements | Controlling implementation/evaluation plan in an authorized successor environment. |

The reported served revision `2b542cf7…`, catalog `0e6cad304fb4e343`, generation `dae69cc80dec0bee`, and 42/42 native identity result remain a different observation from GitHub repository `c1422791…`. Do not combine them into a single tested-deployed identity. The old U1 reference `3143a91…` remains historical. A full upstream commit was supplied; abbreviated blob hashes remain abbreviated, with no manufactured full hash.

The previous graph-generation, source-e2e refusal, and terminal-degraded async records are not reopened. No new Source call, credential path, shell on the operator's host, paid query, database scan, or runtime test is performed here.

### 2.2 External verification boundary

This pass selectively read current official Neo4j manuals; pgvector and PostgreSQL documentation; Lucene codec/quantizer documentation; Faiss documentation; a paper abstract; Voyage's model contract; and public Nornic `main` documentation. The exact pinned Nornic cookbook/vector-skill URLs and the two pinned Source file URLs did not return readable contents through the available web reader. Their inaccessible state is not absence, and `main` is not a substitute for pin verification.

The external register W01–W16 at the end identifies the exact pages and review depth. No cited benchmark was reproduced. No external model/API was used to embed user data. No fresh claim is made about account billing, live cache residency, installed package support, query plans or the missing consumer's behavior.

## 3. What to carry forward from quantization—and what to correct

### 3.1 Keep the useful separation

U1 correctly separates the neighbor topology, search values and optional full-precision rescoring. Neo4j's operational guide attributes Lucene vector files to the OS filesystem cache and supplies the same million-vector file-size example. It warns that segments and compound files affect accounting, and that filter data and graph-property access add different memory demands. Those measurements describe the documented example, not Source. [W02]

For the operator-reported 3,920,000 vectors at 1,024 dimensions, the following are arithmetic planning quantities, not measured resident memory:

| Quantity | Bytes | Decimal GB |
|---|---:|---:|
| Raw FLOAT32 coordinates | 16,056,320,000 | 16.05632 |
| One byte per coordinate, before corrections/metadata | 4,014,080,000 | 4.01408 |
| One bit per coordinate, before corrections/metadata | 501,760,000 | 0.50176 |
| Conservative graph formula `8 × count × m`, at `m=16` | 501,760,000 | 0.50176 |

The raw FLOAT32 payload alone is approximately **14.954 GiB**. It cannot all be resident in a nominal 8GB instance simultaneously. That does **not** prove search is impossible without compression, nor that an observed workload is thrashing, nor that scalar's complete working set fits. Partial locality, storage performance, other indexes, filter fields, heap/page-cache allocation, concurrency, and reranking access all matter.

The 128-dimensional Skill index and the 1,024-dimensional corpus index have different populations and purposes. Neither one dictates the other's compression policy. Likewise, a reported 48GB embedded-GDS host must not be treated as spare filesystem-cache capacity for the distinct reported 8GB vector instance.

A nearly unchanged `.vex` size in an example establishes neither bit-identical connectivity nor a universal graph-size constant. Quantization primarily compresses values; build order and quantized comparisons can still interact with the constructed search structure. File suffixes and layouts are codec-specific, so runtime evidence should identify the actual provider/codec rather than assume all Lucene binary formats use identical files. [U1; W02; W08]

### 3.2 Correct the provider/default clock

The currently documented provider distinction supports scalar quantization on `vector-3.0`, with richer quantization/expansion features in later providers. The scalar `1.5` expansion default must **not** be retrospectively attached to `vector-3.0`. The current settings page labels the expansion option as introduced in 2026.07, while the release chronology records it as preview in 2026.06 and generally available in 2026.07. Binary becomes the documented default in 2026.08. [W01; W03]

The important correction is therefore not whether one describes introduction by preview or GA date; it is that **this later setting is not established as an option or stored value on the reported older index**.

Keep these independent: database version; configured Cypher language; index provider; effective index options; query interface; and actual search behavior. A server upgrade does not mean an existing index was recreated. Explicit creation can choose a newer provider automatically; consequently, rollback cannot be assumed to recreate the old provider merely by replaying old DDL. [W01]

For newer scalar HFQ, the provider table explicitly describes scalar and binary HFQ on `vector-2026.07`; its `vector-2026.08` entry emphasizes binary. Do not infer either automatic loss or guaranteed preservation of scalar HFQ on all future providers from that uneven wording. Test the exact intended provider/configuration before an admission claim.

**No rebuild is approved.** Current source readback should record full index schema, options, state, provider, query contract and relevant population under the existing catalog owner. A version-specific claim about `enabled:false` failures remains a reported compatibility concern until tied to the actual build and error. It is not a reason to combine contradictory legacy/new options speculatively.

### 3.3 A larger requested result window remains an experiment before rebuild

The absence of a separate exposed `ef_search` knob does not prohibit asking a supported API for a larger authorized candidate window. Compare the current owner's direct top-10 with top-50, and measure exact-top-10 membership within those fifty results. This is output-window overfetch, **not** an assertion that the owner exposes query-time HFQ expansion or a specific internal beam.

If authorized and compatible original vectors are available, separately evaluate reranking that candidate set. Record the extra work, transfer and property-read costs. No global improvement or monotonic recall guarantee is assumed. In some implementations the returned top-10 from a larger request can differ from the direct request, which is why both are measured rather than treated as prefixes by definition.

Changing Cypher query syntax and changing index population/filterable schema are also different experiments. A `SEARCH` migration should preserve the intended eligible population and be qualified independently from a quantization rebuild. Do not import `SEARCH` into Nornic or add filterable properties merely because an example contains them. [U1; U2; W01; W04]

### 3.4 Binary is not one shared sign-code format

pgvector's inspected `binary_quantize` function uses the sign of raw components. The documented Lucene binary codec uses optimized, centroid-centered quantization, correction factors and asymmetric query/data precision. The relevant conclusion is **non-equivalence**, not an unsupported claim about Source's exact internal codec. [W07–W09]

Do not use a pgvector bit vector, its Hamming ranking, or its published recall to predict Aura HFQ rankings. Nominal one-bit storage and similar compression ratios do not bind the transform, distance approximation, graph construction or rescoring policy.

`halfvec` is float16. It is not an int8 scalar-code option, and reranking on a `halfvec` heap is not full-FLOAT32 reranking when the original precision was already discarded. If any future test changes storage precision, preserve the original-vector reference and assess representation loss separately.

### 3.5 The pgvector expression-index prohibition should not survive

The maintainer documents expression-index binary retrieval and an outer rerank. PostgreSQL explains that a stored index expression is not recomputed for every row during an indexed search. A generated stored bit column is an option, not a mandatory optimization or proof against drift. The exact index-matching expression, cast, operator class and query plan matter. [W05; W06]

A fallback sequential plan can behave differently, so validate the actual plan rather than categorically prescribing one SQL surface. Query tuning belongs inside an explicitly scoped transaction where applicable, not a persistent pooled-connection setting accidentally inherited by another request.

The usual `ef_search >= candidate count` rule describes a fixed-scan planning concern, not a sufficient recall guarantee. pgvector's optional iterative scans add another termination/ordering contract. Filters, invisible/dead tuples and resource caps still affect results. Comparing Neo4j's construction default 100 with pgvector's 64 does not establish which complete engine has better Source recall. [W05]

No PG ANN or new embedding copy is proposed. An offline exact evaluator is not an additional serving vector store. The 2,000/4,000/64,000 figures describe the documented HNSW indexing limits for the respective types, not an undifferentiated set of SQL storage-type limits.

## 4. Recall: define the experiment, not just the headline

### 4.1 Set membership, ranking and task value are distinct

For query q over an explicitly eligible frozen universe C(q), let G_k(q) be the exact nearest-neighbor set and A_n(q) the unique ANN candidates returned up to depth n.

When at least k items are eligible:

`recall@k(q) = |G_k(q) ∩ A_k(q)| / k`

`candidate_recall@k_in_n(q) = |G_k(q) ∩ A_n(q)| / k`

Report a query-macro average and predeclared strata, retaining per-query records. Do not pool all matching IDs as though all queries or tenants have the same opportunity. Faiss explicitly distinguishes 1-recall@R from intersection/R-recall@R; the metric definition must accompany the name. [W12]

A high similarity score says nothing about whether a missing closer item exists. Precision equals this recall only when both evaluated sets have exactly k unique items and the relevance set is precisely G_k. With fewer eligible items, either define the denominator as `min(k, |C(q)|)` and label it accordingly, or exclude/report those queries under a predeclared policy. An empty eligible universe has no defined neighbor recall. It must not be counted as a perfect hit merely because both lists are empty.

Preserve duplicate-ID faults, illegal IDs, self-match policy, and short results separately. Do not discard failed or incomplete requests from the product metric without reporting their frequency. An unavailable instrument is neither an exact-empty result nor a factual absence finding.

### 4.2 Tie policy is part of ground truth

Identical or near-identical vectors can produce a tied k-boundary. A deterministic ID tie-break can make results reproducible but may penalize another equally valid tied neighbor. Either preserve deterministic-ID recall with that limitation or add a declared distance-tolerant/tie-aware measure. Numerical tolerance must be fixed before outcomes and must not turn distant misses into accepted neighbors.

Remove self-matches by identity when the use case requires exclusion, not by dropping every score of one: separate documents may have identical vectors. Document whether the ID is a chunk, node, document or evidence object. Deduplicating at a different granularity changes the metric.

### 4.3 nDCG and MRR require a relevance definition

Reversing the exact top-k set can leave binary-relevance MRR and nDCG unchanged when all returned members are equally relevant. Therefore “add nDCG” does not automatically measure fidelity to the exact distance order. Use explicitly graded exact-distance/rank gains, a defined rank-correlation statistic, or separately labeled task relevance, depending on the question.

Keep four results distinct: ANN set recall, exact-order fidelity, hybrid/reranker relevance, and downstream task/evidence coverage. A cross-encoder score is not HNSW recall. A perfect exact-vector result may still omit the decisive legal evidence because the embedding representation did not rank it near the query.

### 4.4 Separate vector-only and hybrid measurements

Nornic's `queryNodes` branch can be assessed against the corresponding exact vector metric. A result already fused through BM25/RRF or reranking has a different objective. Comparing that fused list against pure-cosine G_k produces a useful overlap statistic only if named as such; it is not a clean measurement of the ANN algorithm. Upstream explicitly places hybrid retrieval in separate procedures. [W15]

For a composed route, preserve the vector candidates before fusion, lexical candidates, fused candidates, post-filter survivors, reranked output and cross-store joins where those stages are actually exposed. Do not invent internal candidates if the provider only returns final results. The evidence type should identify that limitation.

Join on an authorized canonical identity mapping, not raw scores or presumed equality of local element IDs. The same ID with conflicting vector/content versions must be resolved, not accepted as perfect overlap.

## 5. Ground truth must represent the actual population

### 5.1 Freeze more than the embedding-model name

Ground-truth identity includes:

- Corpus/snapshot identity and the complete eligible ID set, including relevant additions, updates, deletions and tombstones.
- Exact document vector values or their accessible immutable references; dimensions, encoding, normalization, model/revision where available and input-role preprocessing.
- Query bytes and vector bytes, query/document role, text transformation and any allowed server-side embedding path.
- Effective tenant, permission, case/domain filter and suppression/visibility rules.
- Distance/order definition, arithmetic precision, tie and self-match policies.
- Extraction completeness, index coverage and any inaccessible or invalid populations.

Changing ANN construction, search parameters or quantization while retaining this exact full-precision target universe does not itself require recomputing G_k. Changing corpus content, query vectors, filters, eligibility or intended metric does. A stable catalog hash cannot establish that those dependencies stayed fixed.

The operator's Voyage-3 1024 versus Voyage-3-lite 512 distinction is supported by the model documentation. But dimension equality alone is insufficient: different 1024-dimensional models can inhabit incompatible spaces. A Nornic string query uses its configured embedder; do not assume it matches frozen Voyage query vectors. [W16; W15]

### 5.2 Do not hide ingestion loss inside the denominator

If ground truth is built only from the index's surviving entries, a silently skipped embedding cannot appear as a retrieval miss. Maintain separate counts for intended eligible source objects, objects with valid compatible vectors, index-eligible objects, indexed entries and returned results.

This is especially relevant to the reported Nornic write behavior and to documents without embeddings. Vector recall over valid indexed vectors and coverage of the intended corpus are distinct measurements. Neither a skipped 512-dimensional value nor an unknown embedding is ordinary quantization error.

Likewise, an exact pass under privileged access must not be compared with an ANN query under restricted access. Ground truth needs the same legitimately eligible population; do not disable row security or suppression just to obtain a convenient reference set. Authority is an input to the experiment, not an obstacle to bypass.

### 5.3 Full-corpus exact search does not require full GPU residency

Faiss provides exact flat search and documents the conditions for cosine/inner-product equivalence. An exact evaluator can also read permitted vector blocks, compute each block's exact top-k and merge them with the current top-k. No item outside a block's own top-k can be in the global top-k under the same total ordering, so this merge is exact apart from the declared numerical arithmetic. [W10; W11; derivation]

This can bound working memory without restricting the corpus. It still requires legitimate data access, complete snapshots and an appropriate resource budget. Exporting private vectors or sending real queries to an embedding service is not automatically authorized by a request to prepare an audit.

At the reported population, a dense dot-product pass uses about 4.014 billion multiply-accumulates per query. This arithmetic is not a wall-time estimate. Batch size, bandwidth, compute, filtering and implementation determine duration; no CPU/GPU performance was measured here.

A 50k or 100k stratified corpus can support exact **subset** results. It does not lie when honestly labeled, but it cannot certify 3.92M-vector performance. Prefer reducing the initial number of representative queries while retaining the full eligible corpus when feasible. If only a subset is permitted or available, preserve the full-corpus obligation explicitly and never relabel the subset as production ground truth.

### 5.4 Baseline before tuning; independent confirmation afterward

The proposed 200–500 real or representative queries are an initial design choice, not a guarantee of sufficient statistical precision. Keep development/tuning and final confirmation separated by query/source family. A held-out set repeatedly inspected during parameter selection stops being a clean acceptance holdout.

Use paired per-query comparisons, slice-level coverage and uncertainty at the appropriate query/session/family unit. Prespecify the sampling and failure accounting. Rare critical evidence may need purpose-built coverage cases beside traffic-weighted means.

A 0.95 or 0.99 target remains a proposal to justify against task consequence and cost. Neither is a general legal-completeness guarantee. A clean 0.99 geometric score can coexist with missing one crucial authority. Downstream value informs the tradeoff, but cannot waive privacy, access, required evidence, or other non-compensable constraints.

## 6. Loss attribution and resource measurement

The proposed loss stack is a useful diagnostic list, not an additive causal model. Graph construction, quantization, candidate depth, filtering and rescoring interact. A dimension/model mismatch belongs in compatibility and ingestion diagnostics; cross-store identity loss belongs in the join; policy suppression belongs in eligibility. Do not subtract percentages from unrelated benchmarks and call the remainder Source recall.

Reranking a candidate set cannot recover an item that never entered it. Overfetch can help only to the extent that it makes the needed candidate available. Even then, the rerank representation and objective must remain appropriate.

The HNSW paper's abstract reports up to twelve percentage points of change from insertion order in its examined settings. This supports preserving build order/category schedule and testing representative ingestion. It does not establish a twelve-point Source loss, that the reported Phase 3.5 order is the cause of a currently measured defect, or that one model family shares another benchmark's distribution. [W13]

The reported external AWS/Katz/random-vector figures remain **unreproduced benchmark pointers**, not Source targets. They may motivate an experiment, but fixed overfetch ratios, build-speed factors and default-recall claims must not become configuration policy. Relevant primary benchmark pages were not successfully recovered in this bounded pass; no claim of validating those exact numbers is made.

Keep these observations separate:

| Measurement | Required qualification |
|---|---|
| recall@10, recall@50, recall@10-in-50 | Exact universe, per-query IDs, metric, mask and tie policy |
| Indexed coverage | Intended compatible population versus actual membership |
| Short-result/error/timeout rates | Expected available count and failure cause, not silently discarded queries |
| p50/p95/p99 | Workload, sample support, concurrency and comparable cache state |
| QPS | Measured recall and error rate at that load, not maximum throughput alone |
| Cold/warm | Actual or honestly unknown filesystem/index/process state; no destructive production cache manipulation |
| Filtered quality | Filter predicate, eligible population, index prefilter versus application post-filter, policy scope |
| Final task quality | Supported useful evidence, misses, false refusal, citation/qualification preservation and operator repair |
| Cost | Whole query/work path, ground-truth preparation, extra candidates, property reads and recurring maintenance |

Cold filesystem cache primarily changes access cost; warming must not be used to claim a different algorithm by itself. Timeouts, budgets or partial-result paths can make delivered recall differ, and those failures must be visible. Natural first-query behavior, lazy index construction, cold OS cache and cleared application result cache are not the same condition. Do not restart services or flush shared caches without the relevant owner authority.

## 7. Nornic: the inventory is a menu, not an allowlist

### 7.1 Correct the documentation relationship without fabricating a local file

The latest operator report says the Source skill is a condensed fork and its relative cookbook path does not exist in `the-source`. Treat that as a reported pointer defect to verify in the current checkout. A useful repair is an exact pinned upstream locator plus the Source-specific delta and applicable-build field—not a synthetic local cookbook created to make a link pass.

Retain the distinction among:

`upstream documentation pin → inspected implementation → installed build/configuration → Source skill/template → effective authorized query → observed execution route → result and resource behavior`.

The public `main` inventory corroborates fourteen traced route names, a composite pipeline and five pattern flags. It is not evidence that Source's installed engine supports all of them. An exact pin in a report also does not authenticate a binary.

### 7.2 Preserve all named route families from the operator contribution

The following is a review index of U3's named families, not new Source capability IDs or an admission list:

| Family | Retained purpose | Acceptance nuance |
|---|---|---|
| `OuterIndexTopK` / `OuterScanFallbackUsed` | Indexed or fallback ordered reads | Bind actual index/predicate/sort; fallback can be correct but slower. |
| `SimpleMatchLimitFastPath` | Very narrow simple-limit shape | Additional label/filter/sort can select another path; preserve isolation regardless. |
| `TraversalStartSeedTopK` / `TraversalEndSeedTopK` | Seeded bounded traversal | Verify actual depth, direction, multiplicity and result scope. |
| `UnwindSimpleMergeBatch` | Simple batch upsert | A mutation needs its own grant, key and effect contract. |
| `UnwindMergeChainBatch` | Multi-node/relationship merge and supported row-bound stages | Preserve exact semantics and prove dedicated-handler choice; do not infer from a clause substring. |
| `UnwindFixedChainLinkBatch` | Fixed-depth chain materialization | Use approved literal depth, not unchecked interpolation. |
| `UnwindMultiMatchCreateBatch` | Restricted bulk-create shape | Missing clauses are shape conditions, not an opportunity to omit required checks. |
| `CompoundQueryFastPath` | Staged mutation decomposition | Rewriting to multiple requests can change atomicity and visibility; not only latency. |
| `CallTailTraversalFastPath` | Subquery-tail traversal/count | Aggregate and binding changes can alter optimization and results. |
| `MergeSchemaLookupUsed` / `MergeScanFallbackUsed` | Indexed versus scan-based MERGE lookup | Index use is not proof of uniqueness or authorization. |
| `FabricBatchedApplyRows` | Cross-shard batch lookup | Preserve per-shard identity, scope, partial failures and visibility. |
| `executePipeline` | Composite execution facility | Handler fallback is not a security denial; original authority must still govern dedicated execution. |

Retain the five observed upstream pattern names as diagnostic vocabulary: `PatternMutualRelationship`, `PatternIncomingCountAgg`, `PatternOutgoingCountAgg`, `PatternEdgePropertyAgg`, `PatternLargeResultSet`. A flag can support diagnosis but cannot certify a grant or a bounded effect. [U3; W14]

### 7.3 Scope first; optimize the resulting query

For a shared store, a tenant predicate cannot be removed to recover the simple-limit optimization. For a dedicated database, verify the actual owner-enforced boundary instead of inventing a `tenantId` property. The correct output can legitimately use a slower route. A fast-path acceptance target is conditional on semantic and policy compatibility, not a reason to alter the task.

The examples' `EntityA`, `LINKS_TO` and `tenantId` are not facts about all Source schemas. The reported `Skill`, `COACTIVATES` and `SYNERGIZES_WITH` apply to the bound Skill graph, not automatically to a corpus or legal graph. Schema-first means the particular owner/population, not one global substitution dictionary.

### 7.4 Preserve local deltas and semantic equivalence

Keep Source's explicit anti-pattern #8 for parameterized traversal depth, while recording that the supplied upstream list has seven numbered items and expresses the literal-bound constraint elsewhere. Do not rewrite the source history to make the numbering match.

When replacing cross-property OR with UNION, preserve duplicate semantics and ordering. When replacing optional predicates with two templates, cover omitted/null/empty-value cases. Pre-normalizing an indexed property is a write/model change, not a free query edit. Keyset pagination needs a stable total order and tie-break, not merely one nonunique timestamp. Source permission must be present in every applicable branch.

Whitespace-sensitive plan caching is an optimization characteristic to test on the installed build. Keep exact emitted-query hashes for evidence; any canonicalized hash is a separate convenience and must not erase meaning-changing differences. Do not rewrite already qualified templates cosmetically as part of the harvest.

`ON CREATE SET` must be interpreted within MERGE, not converted into a CREATE route through loose text matching. A dedicated mutation handler still needs authorization, transaction, idempotency and target-effect checks. `WITH n LIMIT k` limits selected nodes but not all their incident relationships or lock duration; cleanup on high-degree objects needs an effect-aware budget.

### 7.5 Search state is an instrument state

The current public vector documentation describes dimension omissions, string embedding through the configured model, disabled vector search returning empty plus a warning, lazy search blocking while initialization runs, and policy suppression affecting retrieval. These are upstream descriptions to test on the installed Source build, not current observations. [W15]

A normal liveness check should not implicitly force lazy ANN construction. A genuine cold-search acceptance case may intentionally do so under its budget. The owner must not interpret missing caller-visible warnings as proof that the instrument is available: the warning may be logged elsewhere, so the actual state/readback contract matters.

This supports a particularly valuable learning negative: no result from a disabled, unbuilt, incompatible, inaccessible or suppressed search path may be reinforced as proof that the corpus contains no relevant evidence.

## 8. Embedded suite: the source-inspection advance and remaining consumer question

### 8.1 What the new report narrows

U2 reports actual inspection of the newer script, not merely a projection-only skill sentence. It identifies Cypher `.write` procedures and sequential updates of separate metric families. It reports PageRank as primary, permitted degraded completion, a fallback path and a broad `gds_updated_at` stamp after partial execution. It distinguishes cleanup of a suite projection from AGA session lifecycle.

On that report, R2.P05 now has a more specific **producer-side inspection witness**. R2.P06 is correspondingly straightforward: server Cypher procedure strings are not Python typed-client calls and should not be snake_cased. A no-`.mutate` search remains scoped to the inspected tree and revision.

This supplement has not fetched the private script body successfully, executed it, or observed the active deployment. The operator-reported write path is not downgraded to a mere filename guess, but neither is it relabeled independently verified here.

### 8.2 Mixed property ages versus unsafe observed routing

If the reported control flow is accurate, the writer permits a state in which some property families are new and others remain older. A global completion timestamp is therefore not sufficient evidence of every family's freshness. This is a structural production risk even before a live run is attempted.

But the missing routing-copy consumer remains decisive. Three consumer designs have different valid outcomes:

| Consumer requirement | Partial suite outcome | Correct adjudication target |
|---|---|---|
| PageRank alone is required | PageRank valid and current; optional metrics skipped | May be eligible if the existing contract allows it and scope/readback match. |
| A coherent multi-metric bundle is required | Some required fields are stale/missing | Do not publish/admit that bundle as fully fresh; retain approved prior bundle or explicit unavailable/degraded behavior. |
| Explicit fieldwise freshness is supported | Required fields satisfy their own policies; optional fields can be old | May be eligible, but only with visible field ages, actual selection rule and qualified output. |

Do not globally disable routing, require every optional expensive algorithm, or create a new metric store to resolve this. First locate the exact current consumer, discover which properties it uses, and determine whether it relies on the aggregate timestamp. An empty code-index search does not prove the consumer absent.

### 8.3 Disposable acceptance matrix

Under the existing owner and disposable target, design cases for a complete suite; PageRank-only success; a skipped heavy algorithm; an error before any required write; partial writes followed by failure; a stale consumer; conflicting run/snapshot identity; and fallback to an incumbent.

Observe both metric values and their actual consumption. A zero process exit may truthfully indicate tolerated degradation, but must not be treated as a universal completed-bundle label. Test whether required fields, not merely success text or `gds_updated_at`, govern publication.

If the current owner already enforces the appropriate rule, record a no-change finding. If it does not, change the producer and consumer together through the existing release mechanism and current authority. There is no permission here to invoke the live suite, overwrite metric properties, or alter public exposure.

## 9. Minimal preparation records for the existing owners

These fields are a field map, not a requirement to create another table or registry:

**Retrieval run:** work/query identity; authenticated scope; owner/database/instance; installed engine and effective query; index/provider/options; corpus and vector snapshot; query embedding contract; eligibility/filter policy; search mode and candidate depth; query budget; errors/partial states; ordered unique returned IDs; actual candidate/fusion stages where exposed; result hash and allowed evidence pointers.

**Exact reference:** exact universe and count; complete permitted vector snapshot; query bytes; metric/normalization/precision; tie/self policy; k; exact IDs and optional reference distances; extraction/coverage exclusions; evaluator implementation/version; resource/run provenance. A string saying `exact=true` is not enough.

**Suite publication:** suite run/snapshot; algorithm/property family; required/optional role for this consumer; result status, value and population; per-field or whole-bundle freshness rule; errors/fallback; source and publication identity; actual consumer selection; target/readback and task consequence.

**Learned procedure:** original error and correction; applicability and exclusions; source/build versions; independent evaluation; retained dissent or uncertainty; current authority; actual later use; reduced incompatible attempts, needless refusals, evidence misses or resource waste; adverse cases and retirement trigger.

These records preserve explanatory state while current authorization is rechecked. They do not grant access to raw private vectors, plaintext traffic or reserved mutations.

## 10. Existing work-package crosswalk and next actions

| Existing package | Narrow addition |
|---|---|
| WP00 | Bind exact code/build/index/population identities; confirm fork pointer and locate suite publication consumer. No whole-estate re-audit. |
| WP01 | Preserve retrieval unavailable versus exact-empty; valid denominators, duplicate identity, snapshot consistency and measurement masks. |
| WP02 | Effective tenant-safe Nornic template, correct vector syntax, warning/degradation preservation, qualified hybrid branches. |
| WP03 | Metric result and its publication/consumer must agree; global timestamp is not fieldwise evidence. |
| WP04 | Keep writes, profiling, scans, exporting, resource use and cleanup under actual owners and grants. |
| WP05 | Qualified procedures for owner/dialect selection, false-zero diagnosis and coherent metric use. |
| WP06 | Frozen full-universe or explicitly subset ground truth, independent confirmation, coverage and cache/resource accounting. |
| WP07 | One evidence-driven comparison; no automatic binary, halfvec, provider, kNN or full-suite experiment. |
| WP08 | Exact admitted configuration/procedure reaches a real later consumer; assess benefit and adverse slices. |
| WP09 | Revalidate population, index build, filters, embedder, suppression, metric publication and engine drift. |
| WP10 | Optional compression/acceleration only if measured value justifies it and current authority permits it. |
| WP11 | No new weight learning or reward from cosine, PageRank, recall, or a passing package alone. |

The next legitimate *implementation-session* operations are two bounded investigations that can proceed independently when authorized: bind the suite-copy consumer and its completeness predicate; and locate/reuse the actual retrieval evaluation owner before preparing the recall fixture. Neither requires waiting for a vendor choice. Neither justifies restarting the six-month retrospective.

**No new numbered Source acceptance universe is minted.** The companion R3.D01–D35 items are local review dispositions linked to existing work packages. Their test descriptions are unexecuted proposals, not additional passing tests.

## 11. Takeover continuation — use beneath the existing root, not instead of it

**EXECUTION MODE — CONSUME THE R3 RETRIEVAL/PUBLICATION DELTA UNDER THE ACCEPTED ROOT TAKEOVER.**

Preserve R2 and all existing authority/refusal/public-exposure boundaries. Read this supplement once, bind the new operator observations to current permitted source access, and do not rewrite old manifest/test results. Do not reset to `3143a91…`, `c1422791…` or the upstream documentation commit merely because it appears in a report.

First locate the current `SUITE_V3_TO_ROUTING` or equivalent copy/consumer and determine its exact required metric fields and freshness rule. Trace whether `gds_updated_at` is merely observation time or an incorrectly sufficient publication signal. In disposable tests distinguish complete, partial-but-sufficient, partial-insufficient, stale, conflicting and fallback states. Preserve legitimate bounded PageRank-only use where its actual contract permits it. No live suite invocation is supplied by this text.

In parallel, bind Nornic's installed image/build/configuration, the Source skill's actual path and the upstream documentation relationship. Repair only a demonstrated pointer or contract mismatch through existing owners. Keep Source's local literal-depth warning and all applicable tenant semantics. Observe the actual effective query and dedicated route; do not make the optimization name a grant or require a particular fast path when a correct scoped fallback satisfies the task.

For the vector branch, read the existing index metadata under the appropriate admitted owner. Preserve reported scalar `vector-3.0` as the incumbent until actual evidence says otherwise. Do not fill a missing expansion field with 1.5. Do not add PG ANN, move canonical recall, rebuild an index, upgrade dependencies or purchase compute for parity.

Locate any existing recall/evaluation tooling by relevant scope. Do not interpret a five-neighbor demonstration as an ANN evaluation. Prepare a permitted, frozen query/corpus/embedding/filter contract and an exact reference. Prefer complete eligible-universe search with bounded blocks if that avoids a false sampled-corpus claim. Where only a subset is available, label it and retain the full-corpus gap. No traffic export or embedding API call without its applicable data-use and resource authority.

Compare vector-only ANN sets first, preserving direct top-k and larger candidate windows as different arms. Measure indexed coverage and errors beside recall. Evaluate hybrid/reranked output for its separate task objective. Keep exact IDs, input snapshots and numerical/tie rules stable; no raw-score joins or fabricated independent witnesses. Do not present external default benchmarks as Source results.

Before any tuning candidate is evaluated for admission, freeze margins, ordinary/rare slices, stopping rule, holdout ownership and complete costs under WP06. Reuse existing satisfactory paths; a supported decision not to rebuild is a legitimate result. If a new metric configuration or procedure is warranted, carry it through the existing scoped release and later-consumer evaluation. Rejected or inconclusive experiments remain evidence, not a forced win.

Continue the parent learning objective. A cookbook link, source inspection, baseline recall, corrected timestamp or index catalog is an intermediate artifact. The useful terminal claim is an admitted procedure/configuration that a later task actually uses and that measurably reduces the relevant error or burden without violating the retained constraints. Genuine live-release, data-use, cost and effect gates remain separate; no permission is minted here.

## 12. What is deliberately not done

No Source patch, test execution, index creation/deletion, re-embedding, ANN query, exact corpus evaluation, PROFILE, GDS suite, AGA allocation, registry mutation, family-status change, credential/circuit change, learning admission or deployment was performed. No new measured recall, cold-cache latency, ingestion loss or routing corruption is asserted.

Preparation consists of reading R2, targeted primary documentation review, reconciling all three latest contributions, arithmetic from the operator's reported population, 35 scoped dispositions, and preservation hashes of the named parent files. Those hashes establish byte continuity only. A current official page is not an installed-version witness, and an operator source-inspection report is not a live run.

## 13. Source register

U1, U2 and U3 are the three latest operator messages in this conversation, not invented exported files or independent sources for their repeated claims. U2's reported script body and U3's pinned cookbook remain distinct source-inspection assertions. R2 and the aligned takeover are named in the preparation manifest with exact local hashes.


**W01 — Neo4j vector indexes**  
https://neo4j.com/docs/cypher-manual/current/indexes/semantic-indexes/vector-indexes/  
Review ceiling: Selected settings, provider table, queries, and known limitations; not the installed Source index.

**W02 — Neo4j vector-index memory configuration**  
https://neo4j.com/docs/operations-manual/current/performance/vector-index-memory-configuration/  
Review ceiling: Selected file-layout, measured-example, cache and filter-memory sections; example is not Source telemetry.

**W03 — Neo4j version changes**  
https://neo4j.com/docs/cypher-manual/current/deprecations-additions-removals-compatibility/  
Review ceiling: 2026.06 preview and 2026.07 GA entries for binary/expansion; 2026 feature chronology.

**W04 — Neo4j SEARCH**  
https://neo4j.com/docs/cypher-manual/current/clauses/search/  
Review ceiling: Selected syntax and filter semantics; not Source permission.

**W05 — pgvector maintainer README**  
https://github.com/pgvector/pgvector  
Review ceiling: Selected expression indexing, reranking, exact comparison, iterative scanning, parameter and type sections; mutable upstream.

**W06 — PostgreSQL expression indexes**  
https://www.postgresql.org/docs/current/indexes-expressional.html  
Review ceiling: Stored index-expression evaluation versus recomputation; no plan for Source was run.

**W07 — pgvector binary_quantize implementation**  
https://github.com/pgvector/pgvector/blob/master/src/vector.c  
Review ceiling: Selected binary_quantize body uses component > 0; mutable upstream, not installed extension.

**W08 — Lucene 10.3.1 binary quantizer codec**  
https://lucene.apache.org/core/10_3_1/core/org/apache/lucene/codecs/lucene102/Lucene102BinaryQuantizedVectorsFormat.html  
Review ceiling: Documents centroid-centered, corrected, asymmetric binary quantization. Not a codec readback from Source.

**W09 — Lucene 10.3.1 optimized scalar quantizer**  
https://lucene.apache.org/core/10_3_1/core/org/apache/lucene/util/quantization/OptimizedScalarQuantizer.html  
Review ceiling: Selected interval/centroid/correction mechanism, not Source binary equivalence.

**W10 — Faiss exact indexes**  
https://github.com/facebookresearch/faiss/wiki/Faiss-indexes  
Review ceiling: Flat L2/IP are exact search forms; no dataset or GPU run.

**W11 — Faiss metrics**  
https://github.com/facebookresearch/faiss/wiki/MetricType-and-distances  
Review ceiling: Cosine/inner-product equivalence requires the appropriate normalization; exact numerical contract remains to bind.

**W12 — Faiss evaluation criteria**  
https://github.com/facebookresearch/faiss/wiki/Index-IO,-cloning-and-hyper-parameter-tuning  
Review ceiling: Distinguishes 1-recall@R and R-recall@R/intersection; do not equate all benchmark labels.

**W13 — HNSW ordering and intrinsic dimensionality paper**  
https://arxiv.org/abs/2405.17813  
Review ceiling: Abstract-level review only; reports up to 12 percentage points on its tested scenarios, not on Source.

**W14 — Nornic hot-path cookbook**  
https://github.com/orneryd/NornicDB/blob/main/docs/performance/hot-path-query-cookbook.md  
Review ceiling: Selected main inventory, tenant, query and diagnostic sections. Exact user-pinned commit fetch did not succeed.

**W15 — Nornic vector-search skill**  
https://github.com/orneryd/NornicDB/blob/main/docs/skills/vector-search.skill.md  
Review ceiling: Selected model/dimension, string query, hybrid, suppression, disabled and lazy-warming sections. Not installed Source build.

**W16 — Voyage embedding contracts**  
https://docs.voyageai.com/docs/embeddings  
Review ceiling: Selected older model dimensions and query/document role contract; no embedding API request.

## Appendix — Individual carry-forward dispositions

These 35 entries preserve the distinct technical and evidence decisions. They are not native capability IDs or executed tests. All Source execution remains NOT_RUN.

### R3.D01 — R2 remains accepted; no patches, suite invocation, exposure change or index rebuild authorized

**Disposition:** RETAIN  
**Existing work:** WP00, WP08  
**Basis:** U2, U3, R2

This is a narrow preparation supplement under SLP-1 and R2. No new authority or blanket public-status transition.

### R3.D02 — Nornic pinned upstream cookbook is the engine fact

**Disposition:** QUALIFY_EVIDENCE_LAYER  
**Existing work:** WP00, WP02  
**Basis:** U3, W14

Retain the reported commit/file identities as upstream documentation. Distinguish documented recognition, inspected implementation, installed binary and observed effective execution.

### R3.D03 — Source cookbook link is missing; Source skill is a condensed fork

**Disposition:** RETAIN_AS_OPERATOR_REPORTED  
**Existing work:** WP00, WP02  
**Basis:** U3

Treat as a documentation-provenance defect to confirm in current checkout. Prefer pinned upstream reference plus local deltas, not a fabricated local full cookbook.

### R3.D04 — SimpleMatchLimitFastPath conflicts with tenant WHERE

**Disposition:** RETAIN  
**Existing work:** WP02, WP04  
**Basis:** U3, W14

Authorize and scope first, then observe the effective route. A slower valid route may pass. Never drop isolation to earn a fast-path name.

### R3.D05 — Literal traversal bound is a Source fork delta

**Disposition:** RETAIN_WITH_INPUT_SAFETY  
**Existing work:** WP02, WP04  
**Basis:** U3, W14

Keep the literal-bound rule without inventing an eighth upstream list item. Select from trusted bounded templates; parameterize data values.

### R3.D06 — OR/function/optional-filter rewrites and plan cache rules

**Disposition:** RETAIN_AS_BUILD_SPECIFIC_OPTIMIZATIONS  
**Existing work:** WP02, WP07  
**Basis:** U3, W14

Prove semantic equivalence including duplicates, nulls, ordering and scope. Preserve exact emitted text separately from any normalized fingerprint.

### R3.D07 — Pipeline falls back on unsupported clauses

**Disposition:** DISTINGUISH_FALLBACK_FROM_DENIAL  
**Existing work:** WP02, WP04  
**Basis:** U3, W14

An optimization miss is not a policy refusal. Trace the dedicated handler and enforce original authority across the dispatch.

### R3.D08 — Batch deletion with WITH LIMIT is bounded

**Disposition:** QUALIFY_EFFECT_SIZE  
**Existing work:** WP04, WP09  
**Basis:** U3

Node count alone does not bound incident relationships, lock duration or transaction work. Keep cleanup separately authorized and degree/effect bounded.

### R3.D09 — Nornic vector disabled returns empty/WARN; lazy search blocks

**Disposition:** RETAIN_AS_UPSTREAM_CONTRACT  
**Existing work:** WP01, WP02, WP05  
**Basis:** U3, W15

Bind installed settings and returned/logged evidence. Health checks should not accidentally trigger search/warming. Empty unavailable instruments are not factual negatives.

### R3.D10 — Nornic dimensions silently skipped; string query auto-embeds

**Disposition:** ADD_COVERAGE_AND_MODEL_CHECK  
**Existing work:** WP00, WP01, WP06  
**Basis:** U3, W15, W16

Audit eligible versus indexed vectors and query embedding identity. Equal dimension does not imply same embedding space. Prefer frozen query bytes for ANN-only comparison.

### R3.D11 — 3.92M 1024-d Aura corpus is scalar vector-3.0 on 8GB

**Disposition:** RETAIN_AS_OPERATOR_REPORTED_INVENTORY  
**Existing work:** WP00, WP06  
**Basis:** U1, W01, W02

Bind instance, index, provider/options, valid vector population, model and actual memory before claiming live fit or recall. Separate this instance from the reported GDS suite host.

### R3.D12 — Quantization reduces vector payload, not application graph

**Disposition:** RETAIN_WITH_SCOPE  
**Existing work:** WP00, WP06  
**Basis:** U1, W02

Keep the Lucene cache distinction and measured example scope. Do not infer identical HNSW connectivity or Source sizes from nearly equal example .vex sizes.

### R3.D13 — Scalar current workload fits; none cannot run

**Disposition:** CORRECT_CAPACITY_CLAIM  
**Existing work:** WP06, WP10  
**Basis:** U1, W02

Raw FLOAT32 payload exceeds nominal 8GB capacity; that is full-residency arithmetic, not proof of impossibility or measured thrashing. Include other indexes, filters, graph cache, heap, concurrency and rescore I/O.

### R3.D14 — vector-3.0 has expansion 1.5 frozen until rebuild

**Disposition:** CORRECT_UNSUPPORTED_PROVIDER_SETTING  
**Existing work:** WP00, WP02, WP06  
**Basis:** U1, U2, W01, W03

1.5 is a newer scalar expansion default. Release notes describe expansion preview in 2026.06 and GA in 2026.07. Do not attach that field to vector-3.0 without actual evidence.

### R3.D15 — Binary is the new default; rebuild to pick up HFQ

**Disposition:** RETAIN_NO_AUTO_REBUILD  
**Existing work:** WP06, WP08, WP10  
**Basis:** U1, W01, W03

Keep explicit supported settings on a separately authorized rebuild, not automatic latest defaults. Verify provider-specific rescoring on target; keep active scalar unchanged during baseline measurement.

### R3.D16 — Neo4j binary and pgvector binary are the same sign function

**Disposition:** REJECT_EQUIVALENCE  
**Existing work:** WP02, WP06  
**Basis:** U1, W07, W08, W09

pgvector uses raw component sign; documented Lucene binary uses centered optimized quantization and corrected/asymmetric scoring. Do not claim identical codes or ranking without actual codec proof.

### R3.D17 — Never use binary_quantize(table_col) in ORDER BY; generated column required

**Disposition:** REJECT_BLANKET_RULE  
**Existing work:** WP02, WP07  
**Basis:** U1, W05, W06

The matching expression index is an official pgvector pattern. Stored expression values need not be recomputed in an indexed search. Generated columns are an optional tradeoff; inspect the actual plan.

### R3.D18 — PG ef_search must always exceed inner LIMIT; default ef_c is weaker than Neo4j

**Disposition:** QUALIFY_VERSION_AND_COMPARISON  
**Existing work:** WP02, WP06  
**Basis:** U1, U2, W05

Fixed-scan capacity and iterative scans differ. Use scoped session settings, actual returned count, filters and cost. Cross-engine default numbers do not establish comparative recall.

### R3.D19 — halfvec and bit HNSW should be the PG first cut

**Disposition:** DO_NOT_ADOPT_NEW_STORE  
**Existing work:** WP00, WP10  
**Basis:** U1, W05

No PG ANN is needed for this measurement. halfvec is lossy float16, not scalar int8 and not full-FLOAT32 rerank. Preserve original vectors where required; no mandated storage conversion.

### R3.D20 — Recall@k equals exact/ANN set overlap divided by k

**Disposition:** RETAIN_WITH_EDGE_CASES  
**Existing work:** WP01, WP06  
**Basis:** U2, W12

Freeze target universe, exact metric, unique identity, tie policy and self-exclusion. Handle fewer than k eligible objects and empty universes explicitly; preserve short-result/error rates.

### R3.D21 — Every ANN benchmark uses the same recall metric

**Disposition:** QUALIFY_METRIC_IDENTITY  
**Existing work:** WP06  
**Basis:** U2, W12

Faiss documents both 1-recall@R and intersection. Store the definition rather than trusting a label or comparing unrelated numbers.

### R3.D22 — One formula and common floors can qualify legal retrieval

**Disposition:** REJECT_UNIVERSAL_ACCEPTANCE  
**Existing work:** WP06, WP07  
**Basis:** U2, SLP

0.95/0.99 are proposed operating targets, not evidence of legal completeness. Separate geometric neighbor fidelity, relevant evidence coverage and task-specific acceptance.

### R3.D23 — Ground truth changes only with model/dimension/metric

**Disposition:** EXTEND_INVALIDATION  
**Existing work:** WP06, WP09  
**Basis:** U2

Also rebind corpus membership, vector values, query bytes, filters/policy visibility, tombstones, snapshot and tie rule. ANN-only construction/beam changes on identical universe do not change exact neighbors.

### R3.D24 — Sample-corpus ground truth lies

**Disposition:** QUALIFY_SCOPE_NOT_DISCARD  
**Existing work:** WP06, WP07  
**Basis:** U2, W10, W11

Subset exact truth is valid for that subset, not the full corpus. Prefer fewer representative queries against the full eligible corpus before claiming scale-wide recall.

### R3.D25 — Exact ground truth requires everything in GPU memory

**Disposition:** REJECT_REQUIREMENT  
**Existing work:** WP06  
**Basis:** U2, W10, W11

Exact blockwise search and top-k merge can cover the full corpus using bounded working memory. Freeze arithmetic precision and tie handling; do not claim Faiss/GPU execution occurred.

### R3.D26 — db.retrieve can occupy the same ANN recall column as queryNodes

**Disposition:** SPLIT_OBJECTIVES  
**Existing work:** WP02, WP06, WP07  
**Basis:** U2, U3, W15

Evaluate vector-only fidelity before fusion. Fused hybrid output against cosine neighbors is overlap, not ANN-only quality; assess task relevance and preserve branch provenance separately.

### R3.D27 — MRR/nDCG necessarily detect inverted exact top-k order

**Disposition:** REQUIRE_RELEVANCE_DEFINITION  
**Existing work:** WP06  
**Basis:** U2

Binary relevance for all k exact neighbors can leave those metrics unchanged after permutation. Use specified graded gains or an exact-order statistic; retain human task relevance separately.

### R3.D28 — HNSW, quantization, rescore and filters are separate subtractors

**Disposition:** KEEP_DIAGNOSIS_REJECT_ADDITIVE_CAUSALITY  
**Existing work:** WP01, WP06, WP07  
**Basis:** U2, W13

They interact and may change candidate and construction behavior. Use controlled ablations; dimension mismatch is an invalid representation/coverage state, not ordinary approximation loss.

### R3.D29 — Source category insertion caused about 12 points of loss

**Disposition:** DO_NOT_INFER_MAGNITUDE  
**Existing work:** WP06, WP07  
**Basis:** U2, W13

The paper supports a hypothesis and a representative-ingest test, not a Source penalty or universal default ranking. Preserve source benchmark claims at their actual review ceiling.

### R3.D30 — Cold/warm cache changes retrieval product

**Disposition:** RETAIN_WITH_MEASUREMENT_CONTROL  
**Existing work:** WP06, WP09  
**Basis:** U2, W02

Measure independent latency/error and retrieval outcomes under comparable state. Do not flush/restart production to manufacture cold conditions. Record unknown cache state honestly.

### R3.D31 — Suite writes database, no need for snake_case rewrite

**Disposition:** RETAIN_USER_BOUND_SOURCE_INSPECTION  
**Existing work:** WP00, WP02  
**Basis:** U2, R2

Update inspection evidence only: reported Cypher .write body, not client API, not live invocation. Bounded scripts search for .mutate is not universal absence.

### R3.D32 — Partial suite plus global timestamp proves mixed routing

**Disposition:** SPLIT_PRODUCER_AND_CONSUMER_PROOF  
**Existing work:** WP00, WP03, WP08  
**Basis:** U2, R2

Writer structure permits mixed metric ages if reported control flow holds. Actual routing uptake/requirements remain unbound. Timestamp cannot certify a coherent multi-metric bundle.

### R3.D33 — DEGRADED_PARTIAL must block all routing

**Disposition:** QUALIFY_PER_CONSUMER  
**Existing work:** WP02, WP03, WP08  
**Basis:** U2, R2

A PageRank-only consumer may remain valid; an all-metric consumer must prove required completeness/freshness or use an authorized fallback. Do not disable current service from preparation.

### R3.D34 — Catalog/served identity is enough to reuse quality evidence

**Disposition:** REJECT_SINGLE_GENERATION_SHORTCUT  
**Existing work:** WP00, WP03, WP06, WP09  
**Basis:** U1, U2, U3, SLP

Preserve independent implementation, index/provider, dataset, query/filter, metrics-publication and policy/evaluator identities. A stable catalog cannot freeze those dependencies.

### R3.D35 — Recall fixture and cookbook update establish learning

**Disposition:** REQUIRE_BENEFICIAL_LATER_USE  
**Existing work:** WP05, WP06, WP07, WP08  
**Basis:** U1, U2, U3, R2, SLP

Measure a scoped procedure preventing incompatible, unscoped, stale or false-absence behavior while preserving useful successful work, then observe later use and task value.

---

**Sources ·** R2 and the existing root handoff; U1–U3 operator reports; W01–W16 at stated primary-source review depths.

**Assumptions ·** This continues the non-actuating preparation. Operator-reported installed inventory, source checks and served observations are not independently rerun here.

**Next action ·** Bind the exact suite consumer and retrieval evaluation owner in the authorized Source execution session; preserve the incumbent, qualify the instrument, and carry a useful procedural improvement into assessed later work.
