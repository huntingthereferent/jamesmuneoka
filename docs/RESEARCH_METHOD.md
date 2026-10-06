# Research Method

My default workflow is evidence-first and implementation-driven.

problem -> observe the real system -> record the current state -> identify the smallest useful question -> form a testable model -> build the smallest useful implementation -> test against real or bounded evidence -> compare expected and observed behavior -> keep what survives -> iterate

## Start from the real thing

Whenever possible, I prefer to test against actual APIs, repositories, files, runtime behavior, web surfaces, and user workflows.

Mock data is useful for isolated testing, but it should not silently become evidence that a real integration works.

## Keep evidence separate from interpretation

What happened is not the same thing as what I think it means.

Logs, traces, state snapshots, test results, and reproducible examples should remain available independently of the interpretation built around them.

## Make failures useful

Failed experiments are retained when they narrow the problem.

A failed branch can establish that an assumption was wrong, an interface is insufficient, a dependency is missing, a model does not generalize, or a system boundary was drawn in the wrong place.

That is useful research output.

## Prefer small proofs before large architecture

Before adding a large framework, I try to prove the difficult part in the smallest environment where it can actually fail.

This reduces the chance of hiding uncertainty behind infrastructure.

## Preserve provenance

When a result depends on an external source, prior state, experiment, or transformation, enough provenance should survive to reconstruct why the result exists.

The goal is not maximal logging. The goal is inspectable movement from source to result.

## Promote only what survives

A pattern becomes reusable only after it survives repeated use or testing.

Temporary discoveries can remain local.

Stable discoveries can become tests, utilities, protocols, documentation, reusable components, or project-level rules.
