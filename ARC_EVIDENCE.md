# ARC Research — source and evidence index

*Scope: ARC-AGI-3 native game investigations and separate ARC-like mathematical construction research. Updated October 10, 2026.*

This index links to **actual public code and test entry points**, then states which reported game outcomes do and do not have corresponding public execution data. Source code, a passing test, a recorded score, and a reproducible winning trajectory are different types of evidence.

## 01 / Native ARC-AGI-3 — actual software

| Artifact | Source | What a reader can inspect |
| :--- | :--- | :--- |
| Official game interface and environments | [ARC Prize / ARC-AGI Toolkit](https://github.com/arcprize/ARC-AGI) | External native SDK and game interface; **not** James's solver or scorecard. |
| Native frame observer | [`runtime/arc_native_observer.py`](https://github.com/huntingthereferent/language-network/blob/main/runtime/arc_native_observer.py) | Captures before/after 64×64 native SDK frames, action metadata, selected-state differences, and SHA-256 frame locators. Read-only: it does **not** choose or execute game actions. |
| Execution/evidence comparison | [`runtime/observed_evaluator.py`](https://github.com/huntingthereferent/language-network/blob/main/runtime/observed_evaluator.py) | Reconciles observed native transitions with the existing action/handoff lineage. Not a game-solving policy. |
| Integration tests | [`network/tests/test_arc_native_observer.py`](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_native_observer.py) | Synthetic frame tests and a separately **opt-in** test that invokes an actual FT09 SDK step and passes its observation through the evaluator. One native step is not a completed game. |

**Public test command** (from the `language-network` repository root):

```bash
python -m unittest network.tests.test_arc_native_observer -v
```

The real-SDK FT09 case is skipped unless `CONTINUITY_ARC_NATIVE_TESTS=1` is set and the native ARC dependencies and environment are available. With those prerequisites, its individual test entry is:

```bash
CONTINUITY_ARC_NATIVE_TESTS=1 python -m unittest network.tests.test_arc_native_observer.ARCNativeProviderIntegrationTests.test_actual_ft09_sdk_step_to_service_lineage -v
```

These commands identify inspectable test entry points; the current profile repository does **not** contain a saved successful run of the optional real-SDK test.

## 02 / Native saved routes — actual transferred data and replay code

On October 10, 2026 the uploaded `arc3.rar` supplied game-specific saved action routes. Selected inputs were copied into a versioned [native ARC replay research directory](https://github.com/huntingthereferent/language-network/tree/main/research/arc_native_runs). The files below are **normalized exports of real archived action data**, with original-source references and hashes, not simulated win traces.

| Game | Saved action data | Actual executable replay | Reported local completion | Method/boundary |
| :--- | :--- | :--- | :--- | :--- |
| **FT09** | [75 coordinate clicks in six stages](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/ft09_route.json) | [Native SDK replay](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/replay_saved_paths.py) | **6/6 · 75 actions · score 100** | Source-assisted route; original local report also describes separate visual-agent experiments, not reproduced by this replay file. |
| **LS20** | [309 actions in seven stages](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/ls20_route.json) | [Native SDK replay](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/replay_saved_paths.py) | **7/7 · 309 actions · score 100** | Saved reference-assisted route; not independent first-contact discovery. |
| **SK48** | [280 actions in eight stages](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/sk48_route.json) | [Native SDK replay](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/replay_saved_paths.py) | **8/8 · 280 actions · score 100** | Archived saved-route script uses engine-private state to select ACTION6 coordinates; this is not a public-observation-only policy. |

[Reproduction instructions, original input hashes, and caveats](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/README.md) · [Detailed local case notes](SELECTED_WORK.md#01--interactive-environments) · [Claim and witness ledger](PROVENANCE.md#arc-native-game-experiments).

These newly published **action sequences** are a stronger artifact than narrative completion claims. They are not full per-step observations, independently re-executed scorecards, or the original autonomous policy source. The replay program has not been executed against the native SDK in this transfer environment.

## 03 / ARC-like finite-field mathematical research — public solvers and tests

This is a separate investigation of **constructed finite-state A/B transformation systems**, not execution of ARC-AGI-3 native games.

| Mathematical artifact | Executable source | Tests or contract |
| :--- | :--- | :--- |
| Finite-field state-transition construction | [`math.py`](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/math.py) | [Inverse A/B tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_like_inverse_ab.py) |
| Rooted relational alignment and finite closure | [`alignment.py`](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/alignment.py) | [Alignment tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_like_alignment.py) |
| Bounded inverse construction | [`engine_one.py`](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/engine_one.py) | [Engine 1 contract](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/ENGINE_ONE.md) · [tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_like_engine_one.py) |
| B-action continuation / witness verification | [`cyclic_action_engine.py`](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/cyclic_action_engine.py) | [Cyclic Action Engine contract](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/CYCLIC_ACTION_ENGINE.md) · [tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_like_cyclic_action_engine.py) |
| Constructed-engine continuation and re-entry | [`cyclic_action_continuation.py`](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/cyclic_action_continuation.py) | [Continuation contract](https://github.com/huntingthereferent/language-network/blob/main/work/arc_like_maze/CYCLIC_ACTION_CONTINUATION.md) · [tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_like_cyclic_action_continuation.py) |

The implementation and tests are visible; no statement here upgrades finite-field constructions into an ARC-AGI-3 game solver. Local/CI execution status must be checked separately before claiming a particular test result.

## 04 / Remaining evidence for independent game reproduction

The archive also contains additional experimental policies, alternate replays, local reports, and internal-state probes. Those have **not** all been uploaded into the public repositories. To establish reproducible solver results, the next evidence package still needs:

1. The original game-specific **policy/solver implementations**, exact versions, and dependencies; not only the saved successful routes.
2. Native SDK/environment version, reset rules, supported controls, and permitted observations.
3. Stepwise before/action/after observations or stable hashes tied to the particular run and policy.
4. Native complete-game states, scorecard outputs, and actual validation logs after fresh execution.
5. Separate result labels for source-assisted, reference replay, public-frame policy, and autonomous first-contact tests.

The uploaded archive's autonomous cyclic-agent reports also include unsuccessful native runs. A winning saved replay and a failed autonomous attempt are **different experiments** and must stay separately attributable.

**Current status:** actual saved routes and replay interface **PUBLIC**; public mathematical solvers and observer **PUBLIC**; full original game-specific development policies, per-step traces and fresh externally replicated results **INCOMPLETE**.

[Back to profile](README.md) · [Selected work](SELECTED_WORK.md) · [Provenance](PROVENANCE.md)
