## Research notebook

The object of study is often a system whose rules are **not available at the level where the work begins**.

That may be a game returning frames, a program with inconsistent runtime behavior, an API that changes shape, a repository with competing versions, or an agent reporting success without performing the action. The first job is to recover enough of the native structure to ask a question that can actually fail.

### 01 / State before interpretation

An observation is not yet a rule. For a stateful environment, the useful evidence unit is:

```text
observed state  →  permitted action  →  returned state
            prediction ↗      ↘ discrepancy
```

The returned whole state is the witness. Features—hashes, counts, bounding boxes, source tags, summaries—can help find relations, but a convenient projection should not silently replace what the environment actually returned.

In the ARC investigations, this meant distinguishing a visual pattern from an earned action rule, then checking the rule under fresh replay and deliberately changed action histories.

### 02 / Recovering unknown specifications

A practical sequence:

1. Identify the current referent and the controls available at its native interface.
2. Separate observed, supplied and assumed conditions.
3. Change one bounded relation and capture the returned whole state.
4. Test whether the model predicts a second case, rather than merely describing the first.
5. Preserve a breaking case. Narrow the model or move to the missing boundary.

A failed candidate that eliminates an interpretation is useful; a neat explanation that cannot predict anything is not.

### 03 / What transfers across unlike systems

The same tracing discipline has been applied to interactive environments, code/runtimes, repository state, files and structured records, HTTP/API surfaces, and software interfaces.

The native structures are **not** declared equivalent. Transfer is earned at the relationship that can actually be tested. The underlying task may change from navigation to reconciliation, data transformation, automation, or controlled construction.

**Current construction question:** Can tested constraints and relations generate candidate environments that the same evaluator can inspect? Inverse-category expansion has evidence in the particular ARC investigations; a general world-construction operation remains a **mathematical proposal requiring its own tests**. No general maze-generation success is claimed here.

### 04 / Agents: claimed movement versus executed movement

Agent output is easy to mistake for action. The record must distinguish:

| Layer | Required distinction |
| --- | --- |
| Proposed | What did the model recommend? |
| Authorized | Was that action within the allowed interface? |
| Executed | Did a tool or environment actually perform it? |
| Returned | What native state or artifact came back? |
| Evaluated | What is supported, contradicted, or still unknown? |

A recent local Qwen canary verified **one** model-proposed repository read inside an existing evaluator, including the returned file hash. It did not write code or finish the agent's queued tasks. [Case record](SELECTED_WORK.md#02--local-generative-agent-canary).

### 05 / Provenance without turning research into paperwork

Keep the minimum information necessary to reconstruct what a result depended on: native source locator, earlier state, action or transformation, actual output, tests and failure records, and any unresolved conditions. The aim is replayable reasoning, not maximal logging.

A summary is an index into evidence. It is not the evidence itself.

### 06 / Finite-state conjugacy testing

An inconclusive observation is not permission to change the mathematical question. On a declared 81-state invariant fiber, the first eight fixed-point observations of two restricted actions agree; the ninth separates their cycle structures. A distinct positive case verifies an intertwining bijection. Observation budgets that end too early preserve UNKNOWN, rather than implying equivalence.

A checkpoint experiment reportedly serialized an unfinished comparison, restored it, and continued the original action without changing its domain or losing earlier observations. That tests the continuity *of a particular mathematical investigation*, not a general universal method.

[Mathematical case and evidence limits](docs/FINITE_STATE_CONJUGACY.md)

### Questions still open

- Which state relations survive a change of representation?
- How does an agent discover a dependency it cannot yet observe?
- When can successful local rules be promoted beyond one environment?
- What is the smallest interface that exposes autonomous failure clearly?
- Can construction generate useful candidates without smuggling in their solution?
- What data must survive when work crosses independent systems?

[Selected investigations](SELECTED_WORK.md) · [Evidence status](PROVENANCE.md) · [Working method](docs/RESEARCH_METHOD.md)
