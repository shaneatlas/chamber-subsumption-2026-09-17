# Source plugin connector meta — prepared integration package

**Prepared:** September 17, 2026.  
**Delivery:** connector-owned content, packaging contracts, patch-preparation tool, synthetic tests, and owner handoff.  
**Not delivered:** a rebuilt, lock-recorded, installed, or native-host-accepted Source plugin.  
**State:** `NOT_REPOSITORY_IMPLEMENTED`.

## What this packages

This is the thin-front interpretation of “package all”: reusable selection and evidence semantics, the dated master-path record, and the boundaries that prevent the plugin from pretending to own native execution. It is not a copy of the Source estate.

The expected base is the operator-reported **plugin 0.2.4**. **0.2.5** is the requested candidate version, not a released version created here. The current 0.2.4 source bodies were not obtainable: targeted file retrieval found older patch fragments, and two pinned GitHub reads failed. No replacement manifest or hook runtime was invented.

| Component | Package treatment |
|---|---|
| Four skills | Keep `source-mcp-usage`, `source-levers`, `source-frontier-battery`, `cross-session-orchestration` |
| Five command files | Keep `source-ask`, `health`, `search`, `levers`, `frontier` |
| Battery meta | Append a compact reference directory to the existing frontier skill; load detail only for the relevant task |
| MCP usage | Append result/identity and owner-boundary instructions to the existing usage skill |
| Frontier helper | Append comments only; preparation checks that its Python AST is unchanged |
| Hooks | Keep the existing SessionStart/UserPromptSubmit registrations and helper unchanged; runtime behavior must still be tested by the native owner |
| Plugin manifests | Prepare only the version-field edits to both existing manifests and the Source marketplace entry, after the actual base passes validation |
| Lock | Leave it untouched in preparation; only the inspected existing lock recorder may produce the release lock |
| Native tasks | No pair execution, backend flip, corpus repair, deployment, epoch install, timer, or drain is added |

`contracts/SKILLS_MANIFEST.json` is an **expected inventory for packaging review**, not a new host manifest or Source skill registry. `contracts/HOOKS_CONTRACT.json` is **not executable hook configuration**.

## The interruption is incorporated

The historical master-plan record says round 1 already ran on Source:

- R0 #18770 / `288a70f6…`: publication witness, SUSTAIN/affirmed, 10/13, not the master-plan conferral and not a `bash:git-mutation` witness.
- 3pass r1 `4246cd7c…`: DEFERRED, last symmetric difference 4.
- confer r1 #18772 / `37ac62ee…`: REFUSE/refuted on D_1, 11/13.

The source label DISAGREEMENT is retained; the operator's corrected effective ceiling is **EVIDENCE_INCOMPLETE**. D_2 has no confirming pair in this record. Rounds 2+ belong to **da60e026**. The package invocation itself is **NOT_FIRED**.

The dated D_2 order is preserved: existing-effect readback; conditional API release after the lock check; client breadth; first qualified learning proof; deferred F001/CAP-008/F075/F052; operator hygiene. This is not an executable six-step startup routine.

## Files

```text
CONNECTOR_OWNER_ONESHOT.md          Existing-owner integration handoff
contracts/                         Inventory, hook boundaries, change plan
authoring payloads:
  payloads/frontier-skill.append.md
  payloads/mcp-usage.append.md
  payloads/frontier-script.comments.txt
  payloads/plugins/source/skills/source-frontier-battery/references/connector-meta/
    battery-meta.md
    recursive-pair.md
    graph-plane.md
    master-path.md
    master-path.snapshot.json
    operator-handoffs.md
    geometry-and-products.md
    runtime-boundary.md
    enhancements.md
tools/prepare_connector_delta.py    Reads actual base; emits a review patch outside it
tools/check_package.py              Offline content/integrity checks
tests/test_prepare_connector_delta.py
HOST_ACCEPTANCE.md                  Real-host checks that remain unrun
evidence/                          Source map, test log, validation result
SHA256SUMS                         Package-byte integrity, not authenticity
```

## Run the local package checks

These commands execute only the code supplied in this packet. The tests create and remove temporary synthetic Git fixtures; they do not contact Source, import its code, or run its hooks.

```bash
python3 tools/check_package.py
python3 -m unittest discover -s tests -v
```

**35 synthetic tests passed, 0 failed, 0 skipped** in the preparation run recorded in `evidence/unit-tests.txt`. They validate this package's constraints and stager, not Source's native pair protocol, backend resolver, hook suppression, lock recorder, installed cache, or runtime.

## Prepare a real review patch through the existing connector owner

Use only a real, currently authorized Source checkout. The expected head must be its actual full hash. The command below is a template; neither path nor hash has been inferred for this environment.

```bash
python3 tools/prepare_connector_delta.py \
  --repo /absolute/path/to/the-source \
  --expected-head FULL_CURRENT_HEAD \
  --out /absolute/path/outside-repository/source-plugin-meta-candidate
```

The script has **no apply option**. It does not call a service, read secrets from the environment, import repository modules, run the lock recorder, change Git state, or edit repository files. It produces a patch and changed-file preview in a new, disjoint output directory only after base checks and a second preimage/HEAD check.

It refuses a moved version, incomplete or unexpected base inventory, relevant dirty files, symlinks in inspected files, extra gateway, unexpected hook events, inline manifest hook references, repeated supplement, literal auth header, and an output inside the repository. Unrelated files remain untouched. These are bounds of this stager, not new universal Source policy. An incompatible actual layout is a specific owner-rebind gap, not proof that the plugin is broken.

The emitted state is **PATCH_PREPARED_LOCK_PENDING_NOT_INSTALLED**. The changed-file preview is not a complete plugin. The proposed manifest versions and unchanged old lock are deliberately not a release. The connector owner must review/integrate, use the existing lock recorder, qualify repository tests and host validation, then install only under its applicable authority.

## What remains unproved

Actual 0.2.4 package bytes; current custody/version allocation; real `plugin_lock.py` behavior and coverage; loaded Claude/Codex hook behavior; cache refresh; cross-session skill presence in the installed cache; authenticated serving identity; native evidence/reader behavior. `HOST_ACCEPTANCE.md` records these obligations without marking them passed.

No raw transcript, credential, font, Source executable, native skill estate, or copied host-hook configuration is included in the distributable reference payload. Source hashes and transcript citation ranges are retained in the preparation evidence.

**Sources:** operator contract and latest correction; supplied September 17 transcript, especially its final keyed corrections; targeted official plugin documentation. See `evidence/SOURCES.json`.  
**Assumptions:** none about current installed bytes or host uptake. Base expectations are explicit preconditions, not inferred observations.  
**Next step:** connector owner consumes `CONNECTOR_OWNER_ONESHOT.md`; r2+ remains with da60e026 and does not run as part of packaging.
