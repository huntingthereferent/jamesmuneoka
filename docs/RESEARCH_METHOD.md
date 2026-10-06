# Research Method

The working loop is evidence-first.

```text
problem
→ observe the real system
→ record the current state
→ separate observed / supplied / assumed
→ identify the smallest useful question
→ form a testable model
→ build the smallest useful implementation
→ test against real or bounded evidence
→ compare expected and observed behavior
→ keep what survives
→ continue
```

## Start from the real thing

Use actual APIs, repositories, files, runtime behavior, web surfaces, and user workflows whenever the boundary itself matters.

Mocks are useful for isolated behavior.

They are not proof that the real integration works.

## Keep evidence separate from interpretation

What happened and what it means are different layers.

Logs, traces, state snapshots, test results, and reproducible examples should survive independently of the interpretation built around them.

## Make failures useful

Keep a failed experiment when it narrows the problem.

A failure can establish:

- an assumption was wrong
- an interface is insufficient
- a dependency is missing
- a model does not generalize
- a boundary was drawn in the wrong place

That is useful output.

## Prove the hard part small

Before adding a large framework, isolate the difficult part in the smallest environment where it can actually fail.

Do not use architecture to hide uncertainty.

## Preserve provenance

When a result depends on an external source, prior state, experiment, or transformation, enough ancestry should survive to reconstruct why the result exists.

Not maximal logging.

Enough to inspect the movement.

## Promote only what survives

A pattern becomes reusable after repeated use or testing.

Temporary discoveries stay local.

Stable discoveries can become:

- tests
- utilities
- protocols
- documentation
- reusable components
- project-level rules
