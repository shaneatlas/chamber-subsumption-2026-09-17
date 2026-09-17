# Source — target-aware ingest completion and Nornic indexing reconciliation

**Prepared:** September 17, 2026.  
**State:** PREPARATION_ONLY. No Source operation, queue claim, vector generation, graph write, index rebuild, setting change, or learning activation was performed.  
**Parent:** the mounted R2 graph-plane interpretation and the existing aligned SLP-1 takeover. This is a scoped continuation, not a replacement architecture or authorization grant.

## 1. Decision: resolve the intended reader before copying anything

The new ingest report identifies a useful, narrow discrepancy: stored PostgreSQL vectors and mirrored Aura nodes do not imply that the requested graph-vector representation exists. The most promising repair is target-aware completion in the existing ingest owner, not another ingest of the whole document, another embedding call, a GDS suite, a full-corpus bridge scan, or a new Nornic/PG ANN.

But a missing field is not sufficient to prescribe the copy. Two preceding records make target identity and representation a prerequisite:

- The earlier vector-index inventory named Aura **2423a9f4**, a reported vector-optimized 8GB instance with Voyage-3 corpus vectors.
- The latest ingest says it used Aura **5627c34b**, and that PostgreSQL already held **voyage-3-large** vectors for the batch.

Those are reported different instance and model identities. They could reflect a legitimate migration, different stores with different responsibilities, or different snapshots. None of those possibilities is settled by a common `CorpusEntity` label, a 1024-dimensional array, or an Aura-wide node count.

**The next executable discriminator is therefore:** for these exact fragment IDs and content versions, which authorized consumer is supposed to read which embedding representation, on which instance/database/index/property? If no Aura-vector product is required for the declared RETRIEVAL_TEXT product, its absence can be a deliberate deferred product rather than a broken copy. If it is required and the source vectors are valid and compatible, inspect and repair the keyed materialization path.

The report's `DISCOVERY_ONLY:PARTIAL_DEFERRED` ceiling stays intact. The present analysis does not advance it to vector-topology, high-stakes eligibility, shard convergence, or learning closure.

## 2. What the reported run establishes, with its limits

This table records the user's report; it is not a fresh database read or authenticated receipt export.

| Reported item | Retained observation | Do not infer |
|---|---|---|
| Source document | `SOURCE_LEVERAGE_AUDIT_S2026-09-17.md` | Its full content, all fragment IDs, or a validated extractor output were not supplied in this turn. |
| PG upsert | 23/23; `PHASE_RESUME`; existing/new content lengths equal | Equal length is not byte equality, input identity or semantic equivalence. |
| Embedding stage | `EMPTY_ALREADY_SATISFIED`; generated 0; skipped existing 23; PG vectors described as voyage-3-large | Presence alone does not prove freshness against current content, intended input preprocessing, dimensionality, dtype, or target compatibility. |
| Aura node projection | 23 nodes reported | Upsert count is not necessarily 23 newly created nodes or 23 changed payloads. |
| Graph embedding | 0/23 under the reported graph-embedding probe | The probe's actual instance, property and expected representation still need binding. |
| Edge products | 162 SIMILAR_TOPIC attributed to type/domain clustering; one SHARES_FACT | No cosine NN provenance, independent corroboration or verified claim relationships follows from edge count. |
| Vector bridge/5c | Zero, refused under the reported unbounded CorpusEntity scan | A correct refusal is not completion of the intended bridge product. A new keyed access path still needs its own semantics and cost test. |
| Triples | Zero for this document scope | No structured-claim product is demonstrated; unrelated triples elsewhere are not addressed. |
| PG FTS/embedding | 23/23 reported | This does not establish an Aura full-text index or a Nornic BM25/ANN population for those IDs. |
| Shard alignment | 23 PENDING, queue IDs 5168898–5168920 | Queue existence is not processing or target convergence; PENDING also does not itself prove a particular harmful divergence. |
| GDS | Explicitly skipped | No suite write or metric-publication effect may be credited to this run. |
| Reporting census | 90-second timeout; `dwq#3501 REPLAY_REQUIRED` | Repeating the same broad census is not a necessary vector repair or a completed receipt. |
| Nornic | Fallback/mirror status reported OK, 35,530 nodes | Health and total count do not establish this batch's membership, lexical eligibility or vector state. |
| Aura | 23,047,243 nodes reported | A total on one store is not comparable to another store's count without scope and role. |
| TQG | One five-word item failed a ten-word threshold | Its identity and whether it is among the 23 persisted fragments remain unresolved. Do not automatically delete one of those 23. |
| Receipt | `DISCOVERY_ONLY:PARTIAL_DEFERRED`; product `RETRIEVAL_TEXT` | No automatic HIGH_STAKES_ELIGIBLE, semantic-neighbor, triple-authority or beneficial-learning claim. |

The original exact fragment list, original text/vector hashes, receipt ID and raw run log are not present in this turn. They must be recovered from the current owning operation/evidence, not reconstructed from section names or invented from a count.

### 2.1 Equal lengths do not establish unchanged bytes

Two different strings can have the same length. To confirm a re-hit, compare the canonical fragment identity, source version and content digest or actual stored bytes under a declared normalization rule. Preserve raw source identity separately from normalization used by the embedding pipeline.

Embedding reuse needs a stronger join: content/preprocessing digest, provider/model, dimension, representation dtype, input role and generation/version evidence where available. Otherwise, a same-length content edit can leave a stale embedding and the proposed copy would spread the stale value to another store.

The conservative outcome remains that no new embedding or high-level knowledge product was demonstrated. Do not strengthen the narrower equality-of-lengths observation into a cryptographic idempotency witness.

### 2.2 Distinguish reported row writes from newly learned knowledge

A repeated source can become newly usable if a previously missing projection or consumer is repaired. Conversely, many new edge rows can merely repeat one label-driven relation. Count content novelty, representation completion, retrieval availability and qualified later learning separately. These are not interchangeable forms of progress.

The 23 document fragments share one parent source. Their mutual links and repeated copies must not become 23 independent supporting sources or 162 independent pieces of semantic evidence.

## 3. What the Nornic indexing contribution changes

### 3.1 Preserve four functional families, not an asserted physical implementation

The property/constraint lookup, relationship-existence lookup, lexical search and vector retrieval distinction is valuable. It prevents treating all index work as Lucene/HNSW configuration. The proposed implementation labels and richer-than-Aura scorecard remain claims to bind to a particular build.

For each family, the existing owner must distinguish declared schema, supporting structure, effective settings, actual populated membership and observed query behavior. A constraint declaration is not tenant authorization. A name such as MergeSchemaLookupUsed is not proof that all mutation paths enforce the same constraint or that every MERGE key is unique.

For optional constraint features, test exactly the types needed by the selected workload, including creation against existing data, each relevant mutation form, label mutation, transaction rollback and concurrent conflicts. Do not install every reported extension or alter the live schema to match a feature table.

### 3.2 Named vector metadata and automatic search are separate contracts

The upstream guide describes an automatic search service plus named Cypher index metadata. Its lookup description includes NamedEmbeddings, property arrays and managed ChunkEmbeddings. That means absence of one ordinary property is not a universal proof of absent Nornic vectors. It also means a named metadata declaration is not a guarantee that every API routes through the same ANN implementation or eligible population. [N1]

Bind the particular entry point: named `queryNodes`, REST search, hybrid retrieval and gRPC/client-managed vectors can differ in preprocessing, filters, candidate identity, chunk aggregation and output ranking. Multiple vectors per node require an explicit node/chunk deduplication and best-chunk rule in the exact reference. Source's canonical ID joins must not assume the internal vector ID is the document ID.

Consequently, **“Nornic was not in this write path” supports NOT_OBSERVED_FOR_THIS_RUN, not “Nornic cannot retrieve these IDs.”** Existing lexical or vector materialization could predate this run. No such presence is asserted here either. A bounded membership read is needed only if the chosen consumer actually requires Nornic.

The current skill and guide are not perfectly uniform: the guide describes managed/named fallback without a property array, while a skill pitfall describes missing properties as unsearchable. Preserve the ambiguity for a build/entry-point test instead of choosing the convenient sentence as implementation truth. [N1; N3]

### 3.3 Current configuration materially qualifies the fixed-constants claim

The retrieved current configuration reference documents canonical HNSW settings and their environment alternatives, including `db.nornic.vector.hnsw.m`, `db.nornic.vector.hnsw.ef.construction`, and `db.nornic.vector.hnsw.ef.search`. It also documents vector storage choices including file-backed/disk modes. [N2]

These may be ahead of the operator's pinned documentation or Source's installation. The valid correction is not “Source can already tune these now.” It is **do not codify all-RAM or immutable M/ef constants as engine-wide policy**.

The same reference distinguishes persisted configuration from active runtime state, with explicit activation metadata and process-restart requirements for some tuning. A stored value or successful settings response is not proof that the running searcher uses it. No setting, restart or rebuild is authorized here.

### 3.4 Strategy selection needs a witness, not hardware inference

Retain the reported clustered, GPU-exact, CPU-exact, HNSW and compressed candidates. Do not reduce their precedence to “GPU then HNSW” when the guide lists clustering first, or place the compressed profile in the order without inspecting its actual dispatcher. Number of graph nodes is not necessarily the number of indexed vectors used by the strategy predicate. [N1]

A GPU-assisted HNSW build does not mean exact GPU search. An exact distance pass establishes exact neighbors only over the vectors it actually scans, with the same metric, scope, snapshot and result semantics as the reference. Incomplete indexing, late filtering, stale vector state or chunk aggregation can still make end-to-end recall lower than a claimed universal 1.0.

The published small compressed-profile latency/heap snapshot is not a Source memory win. It does not justify enabling compressed mode on this batch. Effective candidate coverage, work, memory, fallback and later task value must be measured on the bound population.

### 3.5 The strongest implication for the new ingest report

Embedding generation, vector serving, lexical serving and warming are independent dimensions, not a single “index on” bit. The retrieved configuration explicitly supports lexical-only responses when vector serving is off. Managed/named vectors can also exist outside an ordinary embedding property. [N2; N3]

Therefore neither Aura's missing graph property nor Nornic's fallback role blocks a hypothetical lexical retrieval path by logical necessity. What the run supports is narrower: Nornic retrieval was not demonstrated, and its representation of these 23 IDs was not reported.

Health must not be confused with membership or search quality. A lazy-search endpoint is not an appropriate incidental liveness probe. The exact source of a warning matters: a warning written to logs but lost by the consumer cannot protect the learner from a false-absence conclusion.

## 4. Repair contract: source satisfaction is not destination satisfaction

The suspected faulty shortcut is:

`source embedding already exists -> skip generation -> accidentally skip required target materialization`

That is a hypothesis, not yet the bound call path. Other explanations include intentionally text-only projection, wrong instance/index, incompatible representation, omitted serialization field, invalid array encoding, skipped-existing graph branch, stale queue payload, wrong canonical ID, or a graph-embedding probe looking at the wrong property.

The existing ingest checkpoint should decide each required postcondition separately. No new checkpoint service or database is required if current records can express this:

- Source content is identified and qualified for the requested product.
- Source embedding exists and matches that exact content/representation contract.
- Required destination entity exists at the correct source version.
- Required destination vector exists in the expected compatible form.
- The destination's actual index/search owner admits that representation.
- Required alignment work reached the correct target version.
- The declared consumer can use the intended product.

A product can legitimately omit triples or Nornic materialization. It cannot claim their completion from a text or node count. Missing optional products remain explicit; missing required products remain unresolved.

### 4.1 First operation: bind the 23-item identity manifest

In an authorized execution session, obtain the exact IDs from the owning run/queue records. Bind parent document, section/source span, content version/digest, quality status, vector representation and the intended target. Read relevant queues by their exact IDs; do not perform a domain-wide census.

Maintain the current source snapshot or expected content version through the repair. If the source changes, reconcile that change rather than copying an obsolete payload under a newer ID. Keep target-before and target-after observations independent of the desired state.

### 4.2 Then inspect the target-specific skip/copy path

Trace the current code that emits PHASE_RESUME, EMPTY_ALREADY_SATISFIED and the graph-embedding result. Determine whether embedding generation status controls projection, whether projection reloads valid source embeddings, and whether exact pre-existing target nodes are checked for missing vector state.

Validate the target model/dimension and actual vector-index property. In particular, do not pour voyage-3-large values into an existing voyage-3 space solely because both can have 1024 dimensions. Provider-documented compatibility or an independently qualified common space is needed. The provider documentation lists multiple dimensions and distinct input roles; the actual stored metadata and values remain decisive. [V1]

“Phase 3.5” is a pipeline-stage label; it must not be mistaken for the model name `voyage-3.5`. Preserve both fields separately. Do not call any newer model simply because the stage name resembles it.

### 4.3 Repair only a demonstrated missing required materialization

If source embeddings are current and compatible, and the target product requires them, prefer the existing copy/projection owner or a bounded authorized repair over the exact IDs. Preserve source provenance and prevent overwriting a newer or conflicting target version. A raw JSON vector hash can change with serialization; define a canonical numeric representation or an explicit comparison tolerance before claiming equality.

If source vectors are stale, incompatible or incomplete, this is not a pure copy repair. Qualify that earlier defect and its required authority instead of making the target appear populated with wrong vectors. Re-embedding is a separate candidate action, not the default response to graph_embedding=0.

The repair must not create duplicates, widen the target population, add a new ANN store, invoke plane B, or retry the refused global bridge scan. Keep existing Search-waist restrictions unchanged.

### 4.4 Process alignment with its actual version and consumer semantics

The suggested 23-row claim/process operation is appropriate only after the queued payload and handler contract are known. Do not drain first merely to make the dashboard green if the handler repeats the same missing-embedding shortcut or contains a stale source snapshot.

For each row 5168898–5168920, preserve its owner, target, payload version, lease/attempt, expected source generation and completion predicate. If correcting the shared consumer is necessary, qualify that change before processing. If a row requests only a separate valid text alignment, it can proceed independently under its existing scope and report that narrower result.

Mark work complete only after the owning target readback. Do not delete pending rows, forge DONE, or introduce a competing queue. Replayed claims must preserve existing idempotency/fencing and must not regress newer target state. A PG/Aura operation does not gain cross-store atomicity merely from one run ID.

### 4.5 Keep broad census and structural extraction separate

`dwq#3501` is a reported deferred reporting obligation. Retain it and its exact failure; do not require the same multi-million-node dump before a 23-ID repair, and do not claim it completed from a bounded slice. Any changed reporting approach needs its own explicitly scoped result.

Zero triples is consistent with a text-retrieval-only product. A structured capability/plane extractor is a separate product with schema, supporting spans, uncertainty and its own evaluator. Another embedding call cannot supply those semantics. The current batch need not wait for every optional extraction product, but its ceiling must remain accurate.

## 5. Edge and fragment quality: preserve meaning, not appearance

### 5.1 Domain glue can be legitimate without being vector evidence

A same-domain SIMILAR_TOPIC relation can be useful navigation when its provenance says domain/type co-membership. Its existence is not inherently false. The error is presenting it as cosine NN, independent evidence, or a factual link that its generator did not establish.

Preserve edge-generation basis, source document, rule/version, directed/undirected multiplicity, creation versus existing-edge match, and applicable consumers. A numeric weight produced by a rule is not a measured cosine. One SHARES_FACT edge does not on its own establish that the other fragments are poor: different sections can legitimately contain different facts.

Do not delete 162 edges from an analytical disagreement. Inspect the generator and the way readers use these edges; classify or correct only the demonstrated semantic mismatch under the owner. A repeated same-document cluster must not manufacture evidence diversity or train a self-reinforcing topology from its own copies.

### 5.2 The five-word rejection needs an identity, not a bypass

Resolve whether the rejected item is one of the persisted 23, a discarded candidate outside them, or a section marker that should be carried with neighboring content. The report leaves this ambiguous.

Preserve the quality gate. A scoped merge can retain source spans and update derived identities through the existing pipeline. Archival retention, active retrieval eligibility and structured-claim eligibility can differ. Do not silently shorten the population to 22, delete a good fragment, bypass the gate, or erase rejection provenance.

The taxonomy concerns should be tested against the actual fragment text and intended extractor. Terms such as patent_ip or gene_protein on a governance document are suspicious but not conclusive: an audit may genuinely mention those domains. Shared parent, heading context, quoted content and body evidence must be examined before changing labels.

A useful parser negative is a governance-only document with irrelevant biomedical headings in quoted examples: the extractor should distinguish the document's own facts from material discussed or rejected. That is an evaluation design, not a test run here.

## 6. The right 23-item fixture

### 6.1 First prove representation and projection integrity

For every intended item, check correct canonical ID, permitted target, matching content version, expected vector model/dimension/dtype, finite numeric values, correct property/managed representation, index eligibility and required target readback. Assert no unintended IDs were changed and no newer target was overwritten.

Useful disposable cases include source-existing/target-missing, target-already-correct, same ID with newer target content, same-length altered source, wrong model/same dimension, invalid numeric encoding, partial copy then resume, stale alignment payload, and rejected fragment outside versus inside the batch.

A successful rerun should need no new embedding generation when the old source vectors remain valid. It should also avoid inventing new knowledge or appending duplicate semantic edges merely because a repair was retried.

### 6.2 Then test retrieval at the correct scope

Exact cosine over 23 valid PG vectors is a useful bounded reference. It is not by itself ANN recall, and comparing the exact routine with itself will not establish an approximate engine's quality. PG full-text relevance has a different objective from nearest-vector agreement.

Use queries with justified expected supporting fragment IDs and negative/near-match cases, not just a source fragment querying itself. Keep parent-document lineage and passage support visible. Do not reuse the old generic voyage-3 query encoder if the actual batch uses another representation without a demonstrated compatibility contract.

If a future admitted Aura reader participates, compare against the same eligible vector universe and canonical IDs. Global ANN on millions of objects is not directly comparable to an oracle restricted to these 23 unless the actual search is equivalently scoped. Post-filtering a global top-k to the 23 IDs can legitimately lose results; do not misdiagnose that as failed copying.

Nornic is an optional independently qualified consumer. Missing Aura embeddings are not a prerequisite for inspecting Nornic's own named/managed vectors or lexical coverage. Conversely, a healthy Nornic process is not evidence of this batch's recall. A full Nornic IR experiment stays out of the current copy repair unless its current owner and required target role are explicitly selected.

The 23-item test can qualify this batch's representation and bounded retrieval behavior. It cannot certify the 3.92M corpus, legal evidence completeness, triple authority or fleet-wide recall. Broader R2/recall acceptance remains separately scoped.

## 7. The learning lesson that deserves promotion

The candidate lesson is **target-aware resume**:

> A producer's satisfied checkpoint does not satisfy a distinct required consumer representation. Reuse valid producer output, but test each selected target's own identity, representation and completion predicate before skipping it.

That lesson is more general than “always copy embeddings to Aura.” It should choose different actions when the target is already correct, intentionally text-only, on another instance, using an incompatible space, serving lexical-only retrieval, or not part of the task.

The paired inhibitory lesson is **do not interpret representation unavailability as factual absence**. A disabled or unpopulated vector path can coexist with valid text, a lexical path, a different managed-vector representation or an intentionally deferred structured product.

Evaluate both on later unseen tasks under the existing WP05/WP06 machinery. Measure repeated-error avoidance, correct no-op, correct refusal on incompatible copies, useful evidence retrieved, no extra model calls when reuse is valid, no collateral target changes and lower operator repair. The learner must preserve the successful positive cases rather than merely refusing more often.

This connects directly to the parent SLP-1 criterion: useful work -> qualified experience -> independently evaluated scoped change -> authorized admission -> actual later consumer -> assessed task benefit. A filled embedding field, a drained queue or a correct partial receipt is an intermediate result.

## 8. Focused continuation for the existing execution session

**EXECUTION CONTINUATION — EXISTING INGEST OWNER, EXACT REPORTED BATCH.**

Retain R2, the aligned root takeover, `DISCOVERY_ONLY:PARTIAL_DEFERRED`, `--skip-gds`, public graph_gds withholding, and all current authority boundaries. This continuation does not grant writes, queue claims, scans, rebuilds, configuration changes, embedding spend or data export.

Begin by resolving the owning run and exact 23 fragment IDs plus queue rows 5168898–5168920. Bind actual content hashes and vector/content lineage rather than accepting equality of lengths as idempotency. Resolve the rejected five-word item's identity without bypassing the quality gate or deleting a guessed row.

Identify the intended semantic reader and the required target representation. Reconcile Aura instance 5627c34b in the ingest report with 2423a9f4 in the earlier vector inventory. Reconcile stored voyage-3-large metadata with the actual target index/model contract. If the product is intentionally retrieval text only, report the unrequested vector product as deferred and do not manufacture a copy obligation.

If graph-vector projection is required, trace the current skip/resume/project implementation. Confirm or falsify the hypothesis that existing PG embeddings skip a required destination SET. Inspect encoding, model, index property, snapshot and canonical ID alternatives. Apply only the demonstrated current defect under valid local/source/release authority; do not blind-patch from this report.

Test the corrected path on disposable targets: source-existing/target-missing; target already current; same-length content change; incompatible vectors; partial copy/resume; newer target conflict; stale queue payload; quality rejection; and no unintended population changes. Preserve the existing producer and consumer, not a second queue or metric store.

Use the owning claim/process flow for only the appropriate pending work after its handler/version contract is qualified. Complete each row against actual target readback. Do not delete queues, force DONE, replay a broken handler unchanged, or make the unrelated global census a prerequisite. Preserve dwq#3501 as an outstanding reporting obligation with its own disposition.

Observe the selected reader retrieving a justified supporting fragment under the correct scope, not merely seeing 23 target rows. Keep exact 23-vector ranking, text relevance, ANN fidelity, structured extraction and later learning as distinct claims. Do not invoke the GDS suite, broad 5c scan, Nornic rebuild, a new PG ANN, or another Voyage model to improve a count.

Where a reserved action lacks valid authority, finish unaffected preparation and produce one exact target/version/hash/operation request with evidence and recovery. Do not retry the denied connector operation or substitute a new credential/endpoint to evade it.

Close only the declared batch representation/retrieval scope supported by fresh owner evidence. Carry the target-aware-resume candidate through the existing learning acceptance path before claiming beneficial reentry. Do not call the full system complete from this repair.

## 9. Source and preparation limits

**Operator evidence:** the latest Nornic-indexing note and 23-fragment ingest report, plus earlier Aura instance/index inventory and R2 acceptance. They are retained as reports; no original current run log, exact source fragment list, target receipts or installed Nornic build was inspected here.

**Mounted parents:** `SOURCE_GRAPH_PLANES_RECONCILIATION_R2_2026-09-17.md` and `SOURCE_LEARNING_TAKEOVER_ALIGNED_2026-09-17.zip`, along with the mounted root directive and R2 disposition/manifest. Their hashes are recorded and remain unchanged.

**R3 availability limit:** files linked as R3 in an earlier response were not present in this active runtime's top-level attachment directory. This new document is not represented as a byte-preserving reissue of R3, and no R3 download or checksum is invented.

### Primary references selectively reviewed September 17, 2026

**N1 — Nornic vector-search guide, mutable main**  
`https://github.com/orneryd/NornicDB/blob/main/docs/user-guides/vector-search.md`  
Use: automatic versus named metadata, vector sources, runtime strategies and published compressed-profile snapshot. Ceiling: documentation, not exact e917408d pin or Source execution.

**N2 — Nornic configuration reference, mutable main**  
`https://github.com/orneryd/NornicDB/blob/main/docs/operations/configuration.md`  
Use: effective/per-database settings, HNSW controls, activation/restart distinction, storage choices and lexical-only operation. Ceiling: possible newer implementation contract; not current Source options or grants.

**N3 — Nornic vector-search skill, mutable main**  
`https://github.com/orneryd/NornicDB/blob/main/docs/skills/vector-search.skill.md`  
Use: Cypher options, full-text and hybrid roles, dimensions, warnings and managed-vector/ordinary-property ambiguity against N1. Ceiling: documentation, not executable handler proof.

**N4 — Nornic environment-variable reference, mutable main**  
`https://github.com/orneryd/NornicDB/blob/main/docs/operations/environment-variables.md`  
Use: name-resolution reference only. No running environment, key or secret was read.

**V1 — Voyage text-embedding contract**  
`https://docs.voyageai.com/docs/embeddings`  
Use: voyage-3-large, voyage-3.5 and voyage-3 are distinct names with representation and input-role parameters; equal dimensions alone do not certify interoperability. Ceiling: provider documentation, not the batch's actual vector provenance.

The exact pinned Nornic guide and attempted implementation/directory pages were unreadable through the available public tool. No implementation absence or feature nonexistence is inferred from that failure. The [401] surfaced in the conversation was not used as a reason to change credentials or continue a denied action.

**Sources ·** Operator reports, mounted parent artifacts and N1–N4/V1 at stated ceilings.  
**Assumptions ·** This remains non-actuating reconciliation. The target may be deliberately text-only; compatible source vectors and the intended reader must be established before prescribing a copy.  
**Next action ·** Bind the exact 23-item identities, source-vector validity and actual destination/consumer; then repair or disposition the missing required materialization through existing owners and assess later useful use.
