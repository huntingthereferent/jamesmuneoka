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

## 02 / Native game completion reports

The following are **locally reported outcomes**, not independently repeatable results from the public materials linked above.

| Game | Recorded local outcome | Game-specific solver/policy in public repositories? | Full action/frame trace or scorecard published here? |
| :--- | :--- | :--- | :--- |
| **SK48** | 8/8 levels; 280 actions; two fresh winning replays | **Not located** | **No** |
| **LS20** | 7/7 levels; 309 actions; two fresh winning replays | **Not located** | **No** |
| **FT09** | 6/6 levels; 75 actions; two fresh visual-agent winning runs; exploratory paths of 81 and 76 actions | **Not located** | **No** |

The reported local SDK scores were 100.0 in the cited runs. These numbers are carried forward as **local reports**, not independently verified game results. The native observer, its one-step SDK test, and the mathematical engines below must **not** be presented as the missing game-specific solvers or replay data.

[Detailed local case notes](SELECTED_WORK.md#01--interactive-environments) · [Existing claim and witness ledger](PROVENANCE.md#arc-native-game-experiments)

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

## 04 / Missing evidence for independent game reproduction

To substantiate SK48, LS20, and FT09 **as public solver results**, the next evidence package should connect, for each game:

1. The actual solver/policy source and its exact version or commit.
2. The SDK/environment version and configuration, including allowed observations and controls.
3. A serialized action sequence with native observations or verifiable frame hashes, including any reset, seed, and replay conditions.
4. Complete-game completion states and native scorecard output.
5. A runnable replay script and validation report whose recorded provenance matches the published solver and trace.

No substitute traces, synthetic scorecards, or inferred solver links should be created to fill those gaps. Where raw game data cannot be distributed, stable identifiers/hashes and a lawful reproduction method should be supplied instead.

**Current evidence status:** native observer and mathematical source: **PUBLIC**. Game-specific full-run solvers and replay records: **LOCAL / NOT LINKED**. Independent verification of the reported full-game outcomes: **NOT ESTABLISHED IN THIS REPOSITORY**.

[Back to profile](README.md) · [Selected work](SELECTED_WORK.md) · [Provenance](PROVENANCE.md)
