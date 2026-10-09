![James Muneoka](assets/editorial/name.svg)

**Systems Researcher · Systems Architect · Orchestration Engineer**

<small>Mathematical Foundations · Software Systems · Orchestration</small>

I investigate systems that do not come with a reliable specification. The work starts with actual state and behavior, not a description of what the system ought to do. From there: recover the rule, find where it fails, build the instrument, and retain the evidence.

| Research record | Observed result | Current boundary |
| :--- | :--- | :--- |
| **ARC-AGI-3** | SK48 8/8 · LS20 7/7 · FT09 6/6 | Local game replays; not a competition ranking |
| **Finite-state conjugacy testing** | Restricted B-actions separated at the ninth iterate; separate positive 27-cycle witness | 81-state invariant fibers; reported local tests, public reproduction pending |
| **Cross-system orchestration** | Task, source, agent, and handoff traces across independent systems | Private runtime; integration testing in progress |
| **Qwen 3 4B** | One model-selected repository read with matching SHA-256 | Bounded canary; not autonomous completion |

**[Research cases](SELECTED_WORK.md)** · **[Technical range](ABILITY.md)** · **[Research notebook](RESEARCH.md)**


![Work in view](assets/editorial/work.svg)

![01 / Interactive systems](assets/editorial/arc.svg)

**ARC-AGI-3 native game investigations.** Recorded local full-game completions: **SK48 8/8**, **LS20 7/7**, and **FT09 6/6**. The work involved reconstructing state, action effects, collision or movement constraints, and checking predicted outcomes against returned game states.

The FT09 work included a frame-driven policy, successful fresh replays, and an off-trajectory recovery test. These are **specific local game results**, not an ARC Prize ranking or evidence of general performance.

[Read the case record and limits →](SELECTED_WORK.md#01--interactive-environments)

![02 / Cross-system orchestration](assets/editorial/orchestration.svg)

A private runtime coordinating bounded tasks, agents, external sources and human handoffs across different systems. It preserves native task states and source provenance, letting a result cross a boundary without mistaking a proposed action for an executed one.

**Status:** integration and verification work in progress, **not** a claimed production deployment.

[Architecture and current boundary →](PROJECTS.md#cross-system-orchestration--runtime)

![03 / Local agent inference](assets/editorial/qwen.svg)

A recent bounded canary placed **Qwen 3 4B** inside an existing agent evaluator. The model proposed a native repository read; the evaluator performed that read and recorded a matching SHA-256 witness. The complete contextual evaluation took approximately **54.5 seconds** on CPU. A smaller standalone JSON inference took **8.9 seconds**.

This proves one observed model-directed tool step—not self-directed engineering, autonomous project completion, or general reasoning.

[Exact claim boundary →](SELECTED_WORK.md#02--local-generative-agent-canary)


![04 / Finite-state conjugacy testing](assets/editorial/finite-state.svg)

**Finite-state conjugacy testing.** A bounded mathematical investigation compared two invertible finite-field transformations on a declared 81-state invariant fiber. Periodic-point observations agreed through eight continuations and diverged at the ninth. A separate positive control verified an intertwining bijection between restricted actions. Checkpoint-and-resume tests reportedly preserved the watched space and earlier observations while continuing the same question.

**Status:** locally reported mathematical experiments; the exact laws, witnesses, and executable test suite are not yet available in this public portfolio.

[Research case and limits →](docs/FINITE_STATE_CONJUGACY.md)

![Research directions](assets/editorial/directions.svg)

- **Specification recovery:** inferring action rules from an unfamiliar interface.
- **State and representation:** separating changes in the actual system from changes in how it is displayed or encoded.
- **Evidence and provenance:** carrying enough ancestry to distinguish observation, interpretation, and reuse.
- **Agent behavior:** whether an action was performed, what it changed, and where an evaluator must refuse promotion.
- **Construction from constraints:** exploring candidate systems from witnessed relations. **Mathematical proposal; generality not yet established.**

These are connected investigations, not a claim that one method already solves every domain.

[Read the research notebook →](RESEARCH.md) · [Current technical positions →](OPINIONS.md) · [Project map →](PROJECTS.md)


**Evidence policy:** Public claims distinguish local tests, private development, proposed work, and independently inspectable artifacts. Some source and replay archives are private; a summary here is not a substitute for public reproducibility. [Claim and witness index →](PROVENANCE.md)
