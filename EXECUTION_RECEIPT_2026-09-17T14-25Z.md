# Execution receipt — watching seat EX01 handoff

**Ran:** EX01 bind + origin-byte observation of EX02 locators + GitHub issue handoff.  
**Did not run:** CMD02, CMD03, clone-as-checkout, conferral, EX03, epoch apply, deploy.  
**Target:** https://github.com/shaneatlas/the-source/issues/4288  
**Session owner lane:** unbound watching (Grok Build Chamber). Not `6310327d` mutation. Not `da60e026`.

## Observed (origin, not dirty checkout, not installed cache)

- origin/HEAD `1692fdb2d56cc8c0453f59379dc33826af470561` (2026-09-17T14:19:33Z)
- plugin manifests **0.2.5** (claude blob `a6177e7e…`, codex `2d71370b…`, marketplace `085064bb…`)
- skills dirs: 6 (packet expected 4) — extra `source-battery-meta`, `source-skills-manifest`
- command files: 7 (packet expected 5) — extra `source-battery-meta.md`, `source-skills-manifest.md`
- `prepare_connector_delta.py` absent from `the-source` (search total_count=0)
- `plugin_lock.py` and `MANIFEST_LOCK.json` present

## Independently supported

- Wrap checksums unchanged: ONESHOT_DYNAMIC.md sha256 `57457fd32f29beae27c38f2932f2cf7f519395915616b151c51529681185939c`
- `conferral_fired: false`; pair EVIDENCE_INCOMPLETE; R2+ `da60e026`
- Issue #4288 created and assigned to `shaneatlas`

## Remaining blocker

EX02 genuine worktree HEAD+dirty still unbound. Occupied 0.2.5 + moved inventory means CMD02-as-0.2.4 must refuse / reconcile. No apply.

## Next owned action

`6310327d` on the operator checkout: bind HEAD+dirty, then CMD02 no-apply (expect refusal or rebound candidate version ≠ occupied 0.2.5). EX03 stays `da60e026` on a separate surface.
