## Technical range

A skill list tells you what somebody has encountered. An evidence record tells you **what survived a test**. Both are useful, but they are not interchangeable.

### Current practice

| Surface | Work undertaken | What a handoff should contain |
| --- | --- | --- |
| **Unknown behavior** | Recover state, action rules, hidden dependencies, and failure conditions from a live system. | Reproduction steps, a working hypothesis, counterexamples and a bounded next test |
| **Stateful agents** | Examine proposed actions, actual tool execution, returned state, replay and recovery. | Before/action/after trace, acceptance conditions, and refusal-to-claim boundaries |
| **Data / structured inputs** | Inspect, transform, reconcile, validate and track records across formats. | Original and transformed artifacts, record lineage, discrepancy report, tests |
| **Software / automation** | Build Python tools, adapters, validators and focused workflow components. | Source, setup, a real input/output example, runtime verification |
| **Real integrations** | Work across files, repositories, HTTP, APIs, browsers and local processes. | Contract and real-boundary checks; what fails when a dependency disappears |
| **Research communication** | Convert an unclear system into claims that can be challenged. | Evidence, counterexamples, explicit unknowns and a reproducible next question |

### Measured depth

Local ARC interactive environments: **SK48 8/8**, **LS20 7/7**, **FT09 6/6**, with recorded full-game replay tests and off-trajectory FT09 testing. A separate **Qwen 3 4B** canary executed one model-selected native source read through the existing cross-system orchestration evaluator and retained a matching file hash.

These are environment- or step-specific results, **not a blanket claim of general intelligence, general autonomous software delivery, or public production operations**. See [case records](SELECTED_WORK.md).

### Building toward

Complete data/service stacks: Python ingestion, structured data, record reconciliation, PostgreSQL, FastAPI, interfaces, Docker, CI, deployment and monitoring. Physical/measurement boundaries and fabrication-oriented workflows are further research interests rather than implied delivered client work.

### How competence is established

Start with native input, write down what completion would mean, exercise the actual boundary, retain results, then revise only what the evidence permits. Where a dependency cannot be observed, keep it as a named unresolved condition.

[Case records](SELECTED_WORK.md) · [Research](RESEARCH.md)
