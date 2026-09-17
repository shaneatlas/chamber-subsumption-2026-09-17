# SOURCE ONESHOT RUNBOOK — S2026-09-17 (final polish)

**Bound at:** origin/main `e6802946ae` (19:3xZ), seat 78e1699c, actor shaneatlas.
**Supersedes:** every "0.2.4 base → 0.2.5 candidate / 4 skills / 5 commands" anchor in the prompt pack, the connector-owner oneshot, the reconciled handoff and the Chamber wrap. Those are lookup anchors; the live base below is authority.
**Disposition:** runbook. It authorizes nothing by itself; each lane executes only inside its owner's existing custody and release path.

---

## 0. One law, one shape

Every lane today failed the same way: **a remedy whose own precondition cannot hold in the regime it exists for** — a reaper that refuses to run when space is short, a kill switch with no expiry, a protocol requiring a receipt its script cannot write, a directive requiring a base that is already occupied.

Before any step: *can this step's precondition hold in the state it is meant to fix, and who is paged if it silently does nothing?*

Operating posture (verbatim, keep): **Breadth across the objective. Depth at consequential uncertainty. Protected capacity within the wave. Decisive transitions between stages. Independent evidence at acceptance. Learning from observed results.**

---

## 1. Live state (measured this seat, not inherited)

| Surface | Observed | Basis |
|---|---|---|
| `origin/main` | `e6802946ae` | `git log -1 origin/main` |
| Plugin `source` | **0.2.5**, 6 skills, 7 commands, **0** `connector-meta/` refs | `plugins/source/.claude-plugin/plugin.json` @ main; #4272 `4333b946a0` |
| PR #4320 (conferral `decision_text` lossless) | MERGED `e6802946ae`, witness 19053 apex PASS | `gh pr view 4320` |
| PR #4323 (disk remedies reachable) | MERGED `b647be04eb`, witness 19078 apex PASS | `gh pr view 4323` |
| Drainer runtime pin | repinned to `b647be04eb`; prior hand-edit preserved on `wip/graph-first-read-path-pin-S2026-09-17` | `git -C ~/.thesrc/worktrees/graph-first-read-path rev-parse HEAD` |
| Drainer guarded tick | **OBSERVED 19:21:09Z** — `headroom_regime: floor`, reaped 156 scopes / 1,068 files, errors `[]`, 90.4 GB free | `state/ops/hook_effect_intent_spool_drain.jsonl` last line |
| Reclaim belt (daily launchd) | still runs the **unguarded** primary copy | plist `ProgramArguments[1]` = `~/projects/the-source/scripts/ops/...` |
| Disk | 90 GiB free (was 467 MiB); operator ran the belt: 63 removed, 17 salvaged; fleet 186→122 | `df`, `~/.thesrc/receipts/worktree_bank_and_reclaim_S2026-09-17.jsonl` |
| 4,000-char result loss | THREE sites: reader cap `core/api` (peer fix `e0f364350`), writer `run_provider_legs.py` (#4320), envelope `source-mcp/protocol/turn.py:326` (**open, peer lane**) | memory 09-17 |
| Master path D₁ | 3pass 4246cd7c DEFERRED · confer #18772 REFUSE · ceiling EVIDENCE_INCOMPLETE · no D₂ pair · r2+ owner da60e026 | Chamber wrap (carried, not re-fired) |
| Connector CMD02 (prep package) | **UNAVAILABLE** — stager absent at the 2nd publication identity; 0.2.5 occupied | seats 98f3c3a0 / 5ef552cb |

---

## 2. Lanes — first cut, exact command, acceptance, falsifier

WIP = 1 per owner. Four releases stay four (plugin · local MCP install · API deploy · hook epoch). A card outside your closure stays in the map.

### 2.1 Disk / host (this seat — DONE except one packet)
- **Done:** #4323 merged; drainer repinned. **Witness pending:** next 600 s tick writes `headroom_regime` (background wait armed).
- **Operator packet (host-config class, agent-denied):** repoint the belt to the guarded copy and reload:
  ```
  ! plutil -replace ProgramArguments.1 -string /Users/shaneatlas/.thesrc/worktrees/graph-first-read-path/scripts/ops/reclaim_idle_worktrees_all.sh ~/Library/LaunchAgents/com.thesrc.worktree-reclaim-daily.plist
  ! launchctl bootout gui/501/com.thesrc.worktree-reclaim-daily; launchctl bootstrap gui/501 ~/Library/LaunchAgents/com.thesrc.worktree-reclaim-daily.plist
  ```
  Readback: `launchctl print gui/501/com.thesrc.worktree-reclaim-daily | grep program`.
- **Producer bound SHIPPED:** PR #4327 (merge `ecd94a4dacd`, witness 19152 apex PASS) — `scripts/ops/worktree_intake_guard.py`, cap 150 / floor 20 GiB, wired in 9 minting surfaces, 36 tests. **Adoption packet (operator):** `cp` the merged `.claude/hooks/session-worktree-provision.py` over `~/.claude/hooks/session-worktree-provision.py`; `launchctl bootout gui/501/com.thesrc.graph-first-read-path && launchctl bootstrap gui/501 <merged plist>`. Readback: a line in `~/.thesrc/receipts/worktree_intake_guard.jsonl` whose `caller` is a real hook, not `smoke-*`/`parent-proof`.
- **Falsifier:** a fresh `~/.thesrc/reaper.disable` older than 12 h with no line in `~/.thesrc/receipts/reaper_kill_switch_alarm.jsonl` → guard not deployed.

### 2.2 Connector packaging (owner: current holder of row 6310327d — 9403ebc2 claimed 16:00Z)
- **Bind:** `git rev-parse HEAD` in the owner checkout; `plugin.json` version; `ls plugins/source/skills plugins/source/commands`.
- **First cut:** the approved reference delta as **0.2.6** on top of #4272 — 8 Markdown + 1 dated JSON under `plugins/source/skills/source-frontier-battery/references/connector-meta/`, compact supplements to the frontier + MCP-usage skills, comments-only helper change (AST unchanged). **Not** CMD02: the prep package is UNAVAILABLE; author the delta from the approved content, not from the missing stager.
- **Do not:** downgrade to 4 skills / 5 commands; reuse 0.2.5; import native skills, PreToolUse/Stop hooks, B8/epoch, conferral execution, selectors, timers.
- **Acceptance (separate levels):** package checks → `pytest plugins/source` → `plugin_lock.py --record` readback → installed-cache identity → loaded-host skills/commands → gateway catalog/schema identity → on-demand reference consumption.
- **Falsifier:** `git ls-tree -r origin/main plugins/source | grep -c connector-meta/` still `0` after "shipped" → nothing shipped.

### 2.3 Master path / API (owner da60e026)
- **First cut:** EX03 admitted-client readback on production (`/api/build` == main, real route 401 / fake sibling 404).
- **Rule:** ancestry is not consumer behavior; no blind replay of `fullsend /x`; D₁'s REFUSE is not a verdict on D₂.
- **Falsifier:** claiming D₂ without a new `governance.witness_receipt` whose `decision_text` names the D₂ candidate.

### 2.4 Result completeness (owner: peer lane on turn.py)
- **First cut:** `source-mcp/protocol/turn.py:326` silent `json.dumps()[:4000]` → typed bounded continuation or explicit `truncated` flag; test 3999/4000/4001 + multibyte at the MCP envelope, then reconstruct in a real client (T08).
- **Falsifier:** witness `18994` replayed through MCP still yields unparseable nested JSON with a `clean` outer envelope.

### 2.5 Product-answer receipt join (R01–R06, unowned — this seat scoped, did not start)
- **First cut:** `/api/answer` (`core/api/server.py:1722` → `source_contract.answer`) returns edges with no operation receipt. Reuse `_persist_receipt` + `source.operation.readback` in `core/api/substrate_operations.py` (result snapshot ≤ 256 KiB, sha256, `REFERENCE_ONLY` for readback) — precedent #4034 added `source.skills.*` in three files: adapter, contract spec, capabilities.
- **Rule:** never mint a UUID from an edge id (`r-5:…`), never substitute the invocation UUID.
- **Falsifier:** Q02 — search `clopidogrel` Drug limit=1 → `metabolizers` → follow the returned receipt id into a *separate* readback; bytes/sha must match.

### 2.6 FGCS 17-phase program — ALREADY IMPLEMENTED (peer finding, 09-17)
- Peer seats measured it: **36/36 registries populated, 0 trigger gaps over 28 keys, 42/42 skills on main**; the mission's "build order" reads as POPULATE/WIRE. The one real residual: the close gate could not see three of its own classes (hyperedge / manifold / curvature) — M9044 shadow-counts them, LOCAL ONLY, apply denied; and `fn_fgcs_close_contract` is prover-owned by accident (one `ALTER FUNCTION … OWNER TO governance_prover_vm` + a policy row). Runtime defects are filed (ad268306, b8c17787, 4bc637a7, d1ad7f06). **Do not** start Phase 0; cite `finding_the_field_governed_cognitive_substrate_is_already_implemented_…` and `crystallization_fgcs_the_close_gate_could_not_see_three_of_its_own_classes_…`.

---

## 3. Corrections that control execution (carry verbatim)
1. Consider broadly under `/unified-router`; select sufficiently; reroute only on frontier / prerequisite / residual / owner change — never on a timer.
2. `/confer` + `/3pass` discharge only what the installed protocol can; a favorable review manufactures no release, credential, migration or cross-session authority. `apex=PASS + polarity=refuted` is not a pass; the verdict of record is `MAX(created_at)` in `governance.witness_receipt`, never the by_id file.
3. A classifier denial binds every seat; hand the operator the exact command + readback. Do not re-form it (laundering). Attempt likely-denied actions **last**.
4. Merge ≠ deploy ≠ consumer effect. Name which checkout each launchd/plist actually runs.
5. OAuth: scope advertising ≠ registration ≠ enrollment ≠ consumer success. `resources/subscribe` and `listChanged` are independent optional capabilities (local policy may couple them; MCP does not).
6. Rank 3 only against the installed ladder (`governance.fn_3ortho_actualized`); never inferred from the word.
7. Learning is claimed only after a later eligible consumer demonstrably changed behavior.
8. Counts keep their scope: 35+24 synthetic tests ≠ native acceptance; 10/13 with 4 absences ≠ one population until the roster is read.

---

## 4. Return format (every lane, every stop)
```
owner / seat · bound HEAD · candidate/release ids
effect witnessed (surface + query) · highest proven state (SELECTED_NOT_INVOKED … DURABLE)
first unmet acceptance · exact next action · denied actions with the operator packet
residuals (blocked / deferred / adverse / learning) with owner + re-entry condition
```
Never finish with only another plan when an authorized action exists. Never claim an action when only this document was produced.

---

*Inputs hashed in this seat: directive `e0f00ff6…` (59,823 B) · OWNER_REPAIR_HANDOFF `0614d40e…` · api evidence `1a966e0a…` · transcript subsumption `ebe1049f…`. The Chamber wrap (`57457fd3…`, 39 files) and the recombined ZIP were not re-hashed here.*
