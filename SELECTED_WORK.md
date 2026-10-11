## Selected work / case records

Each case keeps the **question, intervention, returned result, and unresolved boundary** together. A recorded local result is not silently promoted into a public reproduction or a general capability claim.

### 01 / Interactive environments

**Public source and evidence map:** [ARC native code, mathematical solvers, run records and missing artifacts](ARC_EVIDENCE.md) · [native SDK frame observer](https://github.com/huntingthereferent/language-network/blob/main/runtime/arc_native_observer.py) · [observer integration tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_native_observer.py). The observer tests include synthetic frames and an opt-in real FT09 **single-step** test; neither constitutes a full-game solving policy or replay of the completion reports below.

**Referent:** native ARC-AGI-3 games. **Status:** measured local outcomes, October 2026; full source/test bundles are not public here.

The challenge was an unfamiliar interactive environment whose useful specification had to be recovered from what actions actually changed. Investigation proceeded from native state captures and bounded experiments, then tested predictions against the next returned state. Failed hypotheses stayed in the record rather than being converted into a story of uninterrupted success.

| Game | Recorded full-game result | Distinguishing investigation |
| --- | --- | --- |
| **SK48** | 8/8 levels; 280 actions; two fresh winning replays | Moving structures, collision rules, controller switching, state compression |
| **LS20** | 7/7 levels; 309 actions; two fresh winning replays | Route recovery, move budget, pickups, launchers, moving switches |
| **FT09** | 6/6 levels; 75 actions; two fresh visual-agent winning runs | Frame-derived controls, color constraints, click prediction, replanning |

The local SDK reported a **100.0 game score** on each completed run. FT09 was additionally tested after an extra exploratory action per level: two fresh runs still completed in **81** and **76** actions. Its policy also declined **nine unrelated public-game observations** rather than pretending to know them.

**What the evidence supports:** these specific local interactive tasks were completed and replayed under the stated conditions.

**What it does not support:** an ARC Prize leaderboard result, an unseen-game generalization rate, or a broadly capable autonomous agent. FT09's execution used rendered frames; earlier investigation was source-assisted. Those are different evidence conditions.

**Witness status:** [Actual saved actions for SK48, LS20, and FT09](https://github.com/huntingthereferent/language-network/tree/main/research/arc_native_runs) and a [native replay entrypoint](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/replay_saved_paths.py) are now public. [Archived LS20](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/original_ls20_complete_replay.py) and [SK48](https://github.com/huntingthereferent/language-network/blob/main/research/arc_native_runs/original_sk48_complete_replay.py) replay source transcriptions are also linked. This is route/replay evidence, **not** publication of every original solver, native frame trace, or independent fresh SDK verification. [Provenance index](PROVENANCE.md#arc-native-game-experiments).

### 02 / Local generative agent canary

**Referent:** existing cross-system orchestration agent evaluator, with local Qwen 3 4B inference. **Status:** observed single tool movement, October 8, 2026.

The question was whether a generative model could supply an actual next movement **inside the existing evaluation lineage**, rather than producing a plan in a separate chat.

- **Proposal:** model returned `MOVE` and selected a whitelisted native source, `runtime/http/index.html`.
- **Execution:** evaluator performed the permitted repository read.
- **Returned evidence:** SHA-256 `1755cc2e0613381a3f004ca46595aa13b12962ddd15e39499823b7d8af4caf9f`, independently matched against the file at the time.
- **Performance:** 54.453 s for the agent-context observation on CPU; 8.87 s for a short standalone JSON inference (approximately 9.86 generated tokens/s in that shorter run).
- **Boundary:** the original task list stayed `READY`. No code modification, autonomous build, or task completion was demonstrated.

**What the result proves:** model inference can propose a source, the native evaluator can execute a bounded read, and an evidence record can return to the same lineage.

**What it does not prove:** reliable long-running autonomy or a completed end-to-end construction loop.

**Witness status:** local runtime observation and matching hash; source and journal remain private. [Provenance index](PROVENANCE.md#local-qwen--orchestration-canary).

### 03 / Cross-system orchestration

**Referent:** one runtime spanning task flows, agent handoffs, external information, traceable movement, and linked local systems. **Status:** active private development.

The engineering problem is preserving system-specific state while allowing a shared workflow to move between boundaries. A source feed is not the same as a task journal; an agent's proposed move is not a verified completion; an interface displaying something is not evidence that the backend performed it.

Current work includes task and source tracing, handoff states, feed projection, evidence-preserving grouping, and local evaluator integration. These are **development and test activities**, not independent proof of production readiness.

**Next validation:** more real-system boundary tests, action/recovery checks, and independently inspectable case artifacts. [Project map](PROJECTS.md).

### 04 / End-to-end public-data application

**Referent:** planned complete application, **not yet a shipped project**.

The target stack is ingestion, validation/reconciliation, PostgreSQL, FastAPI, usable UI, containerization/CI, deployment, and observability. The useful question is whether records, failures, and provenance survive each handoff—not whether a diagram can name each technology.

Future evidence must include an actual running system, reproducible input/output, end-to-end acceptance checks, and operational boundaries.


### 05 / Finite-state conjugacy testing

**Referent:** the continued observation of restricted invertible transformations. **Status:** local mathematical experiments reported in October 2026; public source and witness bundle pending.

Two systems over $\mathbb F_3^5$ differ by one admissible next-coordinate coupling. Restricted to a specified 81-state $B$-invariant fiber, the first action has nine cycles of length 9 and the second three cycles of length 27. Their periodic-point counts agree through $B^8$, then differ at $B^9$: 81 fixed states versus zero. Their restricted $B$-actions are therefore nonconjugate. On the full 243-state space, a distinction appears earlier, at $B^3$.

A separate positive control reports an explicit verified bijection intertwining the restricted $B$-actions of two distinct laws with matching 27-cycle structures. In the declared observation procedure, the negative case remains UNKNOWN at budget 8 and becomes DISTINGUISHED at 9; the positive case remains UNKNOWN at budget 26 and yields a verified restricted-$B$ correspondence at 27.

Reported tests: **13/13** for native continuation and **17/17** for serialization, re-entry, and continued observation. The results do not assert simultaneous $A$/$B$ conjugacy, an unrestricted construction method, or independent public reproducibility.

[Detailed mathematical record](docs/FINITE_STATE_CONJUGACY.md) · [Witness status](PROVENANCE.md#finite-state-conjugacy-testing)

[Research notebook](RESEARCH.md) · [Back to profile](README.md)
