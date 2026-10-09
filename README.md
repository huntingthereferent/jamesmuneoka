# James Muneoka

**Systems research · Interactive environments · Agent evaluation · Applied software**

I investigate systems that do not come with a reliable specification. The work starts with actual state and behavior, not a description of what the system ought to do. From there: recover the rule, find where it fails, build the instrument, and retain the evidence.

![Three current research surfaces: native interactive environments, cross-system runtime behavior, and model-directed tool use.](assets/working-practice.svg)

**[Research cases](SELECTED_WORK.md)** · **[Technical range](ABILITY.md)** · **[Research notebook](RESEARCH.md)** · **[Working with me](WORK_WITH_ME.md)**

---

## Work in view

### 01 / Interactive systems — recover the rule before writing the solver

**ARC-AGI-3 native game investigations.** Recorded local full-game completions: **SK48 8/8**, **LS20 7/7**, and **FT09 6/6**. The work involved reconstructing state, action effects, collision or movement constraints, and checking predicted outcomes against returned game states.

The FT09 work included a frame-driven policy, successful fresh replays, and an off-trajectory recovery test. These are **specific local game results**, not an ARC Prize ranking or evidence of general performance.

[Read the case record and limits →](SELECTED_WORK.md#01--interactive-environments)

### 02 / Continuity — preserve meaning across real boundaries

An active private runtime connecting task handoffs, source feeds, trace ancestry, agent evaluation, and other local systems without making them pretend to share one data model. The question is not merely whether a connection works; it is what evidence and context survive the crossing.

**Status:** integration and verification work in progress, **not** a claimed production deployment.

[Architecture and current boundary →](PROJECTS.md#continuity--cross-system-runtime)

### 03 / Local agent inference — test the action, not the explanation

A recent bounded canary placed **Qwen 3 4B** inside an existing agent evaluator. The model proposed a native repository read; the evaluator performed that read and recorded a matching SHA-256 witness. The complete contextual evaluation took approximately **54.5 seconds** on CPU. A smaller standalone JSON inference took **8.9 seconds**.

This proves one observed model-directed tool step—not self-directed engineering, autonomous project completion, or general reasoning.

[Exact claim boundary →](SELECTED_WORK.md#02--local-generative-agent-canary)

---

## The kind of work I take on

**Investigate and repair** a failing script, API workflow, data pipeline, or existing application. Reproduce the actual behavior, isolate the first unsupported assumption, repair what can be tested.

**Build a bounded tool** to inspect, validate, reconcile, transform, or monitor real inputs. Typical surfaces: Python, structured files, HTTP, repository workflows, and automation.

**Evaluate a stateful system or agent** using real state transitions, replay, counterexamples, expected-versus-observed results, and recovery tests.

**Delivery standard:** usable artifact or reproducible finding; input/output example; test evidence; limitations and a clear handoff. No invented success state.

[Scope a piece of work →](WORK_WITH_ME.md)

## Research directions

- **Specification recovery:** inferring action rules from an unfamiliar interface.
- **State and representation:** separating changes in the actual system from changes in how it is displayed or encoded.
- **Evidence and provenance:** carrying enough ancestry to distinguish observation, interpretation, and reuse.
- **Agent behavior:** whether an action was performed, what it changed, and where an evaluator must refuse promotion.
- **Construction from constraints:** exploring candidate systems from witnessed relations. **Mathematical proposal; generality not yet established.**

These are connected investigations, not a claim that one method already solves every domain.

[Read the research notebook →](RESEARCH.md) · [Current technical positions →](OPINIONS.md) · [Project map →](PROJECTS.md)

---

**Evidence policy:** Public claims distinguish local tests, private development, proposed work, and independently inspectable artifacts. Some source and replay archives are private; a summary here is not a substitute for public reproducibility. [Claim and witness index →](PROVENANCE.md)
