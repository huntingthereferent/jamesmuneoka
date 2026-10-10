## Claim and witness index

A reader should be able to distinguish a measured local observation from a publicly reproducible artifact. This index states the evidence **available in the public repository**, not just the confidence of the person who ran the test.

| ID | Claim | Native witness held where | Publicly reproducible here? | Limit |
| --- | --- | --- | --- | --- |
| ARC-01 | SK48 full 8/8 local completion, recorded fresh replays | Private/local ARC run and replay records | **No** | One known public game, not a competition result |
| ARC-02 | LS20 full 7/7 local completion, recorded fresh replays | Private/local ARC run and replay records | **No** | One known public game, not unseen-task generalization |
| ARC-03 | FT09 full 6/6 local completion; off-trajectory tests | Private/local visual policy and frame traces | **No** | Source-assisted investigation preceded frame-based execution |
| AGENT-01 | Qwen 3 4B selected one source; native evaluator read it | Private cross-system orchestration canary journal, source and hash | **No** | Single read step, no edit or autonomous completion |
| SYS-01 | Cross-system orchestration connects task, feed, and trace-related runtime components | Private development repository and local tests | **No** | Not evidence of production reliability |
| STACK-01 | Complete public-data application | Architecture and intended acceptance chain | **Not applicable — planned** | No shipped deployment claimed |
| MATH-01 | Finite-state transformation continuation and re-entry | Local mathematical witnesses and reported regression tests | **No** | Restricted B-actions; scoped observation budgets; reproducible bundle pending |

### ARC native game experiments

**Public implementation links:** [source and evidence audit](ARC_EVIDENCE.md) · [ARC native frame observer](https://github.com/huntingthereferent/language-network/blob/main/runtime/arc_native_observer.py) · [native observation integration tests](https://github.com/huntingthereferent/language-network/blob/main/network/tests/test_arc_native_observer.py) · [official ARC toolkit](https://github.com/arcprize/ARC-AGI). The observer records an already-executed frame transition; the tests primarily use synthetic frames and include a separately opt-in real FT09 single-step test. **They do not contain the SK48/LS20/FT09 winning policies, full action traces, or native completion scorecards.** Finite-field A/B construction source and tests are [indexed separately](ARC_EVIDENCE.md#03--arc-like-finite-field-mathematical-research--public-solvers-and-tests) and do not represent native-game execution.

The recorded October 2026 outcomes are:

- SK48 — 8/8 levels, 280 actions, two fresh winning replays.
- LS20 — 7/7 levels, 309 actions, two fresh winning replays.
- FT09 — 6/6 levels, 75 actions, two fresh visual-agent winning runs; 81 and 76 actions in separate exploratory-path tests.

The native game SDK reportedly returned 100.0 scores in these specific local runs. **Saved full-game action routes and replay code are now public** in [language-network/research/arc_native_runs](https://github.com/huntingthereferent/language-network/tree/main/research/arc_native_runs), with source-file hashes and the recorded limitations. This does not provide original frame-by-frame traces or verified fresh runs, and reported native scores have not been independently reproduced for this transfer.

### Local Qwen / orchestration canary

On October 8, 2026, a local `qwen3:4b-instruct` model produced a proposed `MOVE` selecting the native source `runtime/http/index.html`. The bound cross-system orchestration evaluator read the permitted file and recorded SHA-256:

```text
1755cc2e0613381a3f004ca46595aa13b12962ddd15e39499823b7d8af4caf9f
```

The independently checked local file hash matched at the time of the test. The observed evaluation took 54.453 seconds; a shorter standalone JSON inference took 8.87 seconds, generating about 9.86 tokens per second.

**Limits:** the local files, model inference logs, and canary journal are not in this public repository. The private source may evolve, so this hash identifies the file **as observed then**, not its current contents or its scientific correctness. The original queued tasks remained `READY`; no autonomous build was completed.

### Finite-state conjugacy testing

Local reports from October 2026 describe an 81-state \(B\)-invariant fiber. The negative pair has nine 9-cycles versus three 27-cycles; their fixed-point counts first diverge at \(B^9\) under the declared restricted observation. A separate positive case reportedly constructs and verifies an intertwining bijection for restricted \(B\)-actions. A later reported checkpoint experiment retains the underlying comparison while serializing and restoring it.

**Reported local checks:** 13/13 continuation tests and 17/17 re-entry tests. **Not published here:** exact laws, fiber predicates, source code, positive bijection, serialized checkpoint fixtures, or runnable tests. No full two-generator equivalence or general method is implied.

[Mathematical case](docs/FINITE_STATE_CONJUGACY.md).

### What stronger publication would require

Native replay traces and execution scripts, environment/version details, reproducible entrypoints, negative cases, and a way for someone else to execute the same checks. Those are future publication steps—not materials implied to exist in this public repository.

[Cases](SELECTED_WORK.md) · [Research](RESEARCH.md) · [Profile](README.md)
