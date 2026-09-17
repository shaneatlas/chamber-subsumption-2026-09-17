# Commands and binding gaps

**Not a batch script. Do not execute this document top to bottom.** Commands have different owners, permissions and effects. A copied current-sounding template does not establish its parser, checkout or authority. Missing commands are intentionally not invented.

The only commands executed for this recombination are local package validators and disposable test fixtures, recorded in the validation evidence. Native Source commands below remain templates for their existing owners.

<a id="cmd01"></a>
## CMD01 — LOCAL_PACKET_CHECKS

**Owner:** Artifact recipient · **Status:** `EXECUTED_IN_LOCAL_PREPARATION_SCOPE_ONLY`

```bash
python3 tools/validate_recombination.py
python3 -m unittest discover -s tests -v
```

**Limits:** Runs only this new reference validator and disposable tests. Its success does not validate Source code or native hosts.

**Source:** [S02](source_views/S02.html#L1) · [S15](source_views/S15.html#L1)

<a id="cmd02"></a>
## CMD02 — PREPARATION_ONLY_TEMPLATE

**Owner:** Connector owner · **Status:** `REAL_CHECKOUT_NOT_RUN`

```bash
python3 inherited/SOURCE_PLUGIN_CONNECTOR_META_2026-09-17/tools/prepare_connector_delta.py \
  --repo /absolute/path/to/the-source \
  --expected-head FULL_CURRENT_HEAD \
  --out /absolute/path/outside-repository/source-plugin-meta-candidate
```

**Limits:** Actual full HEAD and path required. No apply option. Expected 0.2.4 base and proposed 0.2.5 must remain available; incompatible base must be reconciled, not downgraded.

**Source:** [S02](source_views/S02.html#L1) · [S03](source_views/S03.html#L1) · [S14](source_views/S14.html#L1)

<a id="cmd03"></a>
## CMD03 — NATIVE_LOCK_RECORDER_TEMPLATE

**Owner:** Connector release owner · **Status:** `NOT_RUN`

```bash
python3 plugins/source/scripts/plugin_lock.py --record
```

**Limits:** Only after reading actual current script/tests and integrating the qualified candidate. Use the actual repository interpreter and normal release authority. This command mutates the lock; not permitted by an artifact-only read.

**Source:** [S03](source_views/S03.html#L1)

<a id="cmd04"></a>
## CMD04 — HISTORICAL_NATIVE_PREPARE_TEMPLATE

**Owner:** Epoch release dc64363e, current custody to bind · **Status:** `NOT_RUN`

```bash
python3 scripts/governance/install_hook_epoch_persistent.py \
  --epoch EPOCH_SHA --bundle BUNDLE_SHA
```

**Limits:** Reported wrapper template; actual parser, pinned installer and candidate must be inspected. Publishes no missing epoch code and does not reload a host. Prepare is host-file read-only, not a universal no-local-file side-effect guarantee.

**Source:** [S38](source_views/S38.html#L1)

<a id="cmd05"></a>
## CMD05 — RESERVED_NATIVE_APPLY_TEMPLATE

**Owner:** Exclusive release/operator configuration owner · **Status:** `NOT_RUN`

```bash
python3 scripts/governance/install_hook_epoch_persistent.py \
  --epoch EPOCH_SHA --bundle BUNDLE_SHA --apply --provenance PROVENANCE_DIR
```

**Limits:** Separate current apply authority and config custody required. Journal APPLYING goes to existing recover_install contract, not retry. No supported recovery CLI was supplied; inspect owner function instead of inventing a flag.

**Source:** [S38](source_views/S38.html#L1)

<a id="cmd06"></a>
## CMD06 — HISTORICAL_HARNESS_TEST_TEMPLATE

**Owner:** Current harness implementation owner · **Status:** `NOT_RERUN_ON_SOURCE`

```bash
PYTHONPATH=.:source-mcp python -m pytest \
  source-mcp/tests/test_async_lifecycle_ownership.py \
  source-mcp/tests/test_harness_continuity_boundaries.py \
  tests/lifecycle/test_g4_g5_g6_hardening.py \
  tests/lifecycle/test_membrane_facade.py \
  tests/lifecycle/test_harness_policy_admission.py -q
```

**Limits:** Recorded historical suite. Reconcile files/dependencies/current changes first. Tests characterizing orphan non-recovery are not positive recovery acceptance; do not claim current 81 passes from this template.

**Source:** [S28](source_views/S28.html#L1)

## Supported locators without a supplied current invocation

Native router-body reader; admitted activation fixture for `fullsend /x`; actual async/CAP-004 client fixtures; release recovery gateway; utility-evaluator required arguments; canonical claim flow; native plugin host update/readback; installer recovery entrypoint; corpus reuse flag; real entity selector; effective GUC/ANN owner; native recursive-pair command/decision packet; graph resolver and applicable template; task-specific verifier; and candidate-harness enrollment are **owner binding gaps** until inspected.

The record supplies names, source paths, predicates or historical commands. It does not support fabricating a current command for each. The execution cards state the exact output the binding must establish. No placeholder is silently filled with a credential, user identity, corpus ID, branch, schema hash, bundle, endpoint or native decision hash.
