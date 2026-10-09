# Selected work / case records

Each case keeps the **question, intervention, returned result, and unresolved boundary** together. A recorded local result is not silently promoted into a public reproduction or a general capability claim.

## 01 / Interactive environments

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

**Witness status:** summaries of local replays; the underlying game traces, tool outputs, and implementation are not published in this repository. [Provenance index](PROVENANCE.md#arc-native-game-experiments).

## 02 / Local generative agent canary

**Referent:** existing Continuity agent evaluator, with local Qwen 3 4B inference. **Status:** observed single tool movement, October 8, 2026.

The question was whether a generative model could supply an actual next movement **inside the existing evaluation lineage**, rather than producing a plan in a separate chat.

- **Proposal:** model returned `MOVE` and selected a whitelisted native source, `runtime/http/index.html`.
- **Execution:** evaluator performed the permitted repository read.
- **Returned evidence:** SHA-256 `1755cc2e0613381a3f004ca46595aa13b12962ddd15e39499823b7d8af4caf9f`, independently matched against the file at the time.
- **Performance:** 54.453 s for the agent-context observation on CPU; 8.87 s for a short standalone JSON inference (approximately 9.86 generated tokens/s in that shorter run).
- **Boundary:** the original task list stayed `READY`. No code modification, autonomous build, or task completion was demonstrated.

**What the result proves:** model inference can propose a source, the native evaluator can execute a bounded read, and an evidence record can return to the same lineage.

**What it does not prove:** reliable long-running autonomy or a completed end-to-end construction loop.

**Witness status:** local runtime observation and matching hash; source and journal remain private. [Provenance index](PROVENANCE.md#local-qwen--continuity-canary).

## 03 / Continuity and cross-system work

**Referent:** one runtime spanning task flows, agent handoffs, external information, traceable movement, and linked local systems. **Status:** active private development.

The engineering problem is preserving system-specific state while allowing a shared workflow to move between boundaries. A source feed is not the same as a task journal; an agent's proposed move is not a verified completion; an interface displaying something is not evidence that the backend performed it.

Current work includes task and source tracing, handoff states, feed projection, evidence-preserving grouping, and local evaluator integration. These are **development and test activities**, not independent proof of production readiness.

**Next validation:** more real-system boundary tests, action/recovery checks, and independently inspectable case artifacts. [Project map](PROJECTS.md).

## 04 / End-to-end public-data application

**Referent:** planned complete application, **not yet a shipped project**.

The target stack is ingestion, validation/reconciliation, PostgreSQL, FastAPI, usable UI, containerization/CI, deployment, and observability. The useful question is whether records, failures, and provenance survive each handoff—not whether a diagram can name each technology.

Future evidence must include an actual running system, reproducible input/output, end-to-end acceptance checks, and operational boundaries.

---

[Research notebook](RESEARCH.md) · [Back to profile](README.md)
