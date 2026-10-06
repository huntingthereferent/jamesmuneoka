# Research

I work as an independent technical researcher at the boundary between software, systems, data, automation, and AI/agent behavior.

The research is practical: I use working code, bounded experiments, traces, state captures, counterexamples, and reproducible tests to investigate how systems behave and where assumptions fail.

## Research questions I tend to pursue

- How do you recover the structure of an unfamiliar system from its observable behavior?
- What information must survive when state moves across tools, representations, or interfaces?
- Where does an expected workflow actually break?
- Which differences are meaningful, and which are incidental representation changes?
- How do you preserve evidence while compressing a complicated process into something usable?
- How can an automated system remain inspectable after many steps?
- What can be generalized from one domain without pretending unlike systems are identical?

## Current research areas

### Unknown-system tracing

I study unfamiliar systems by establishing a current state, observing changes, tracing dependencies, and locating the smallest boundary where expected and observed behavior diverge.

This has included repositories, filesystems, APIs, structured data, runtimes, browser surfaces, command-line tools, and external services.

### Evidence and provenance

A recurring question in my work is how to preserve enough ancestry that a later result can still be inspected.

That includes:

- source evidence
- state transitions
- timestamps
- transformation history
- test outcomes
- decision records
- failure traces
- cross-layer handoffs

### Agent and reasoning evaluation

I use bounded environments to study whether a reasoning process can recover rules, detect contradictions, revise hypotheses, and continue without silently replacing missing evidence with assumptions.

The important artifact is not only the final score. It is the trace of what was observed, predicted, contradicted, retained, and changed.

### Representation and reconciliation

I investigate cases where the same underlying thing appears through different representations:

- code vs runtime behavior
- file vs parsed structure
- API response vs UI
- source records vs reconciled records
- current state vs historical state

The goal is to distinguish meaningful change from representational difference.

### Applied systems research

I also use full software systems as research instruments.

A public-data application, for example, can expose questions about ingestion, identity, reconciliation, failure semantics, recovery, observability, and provenance that are invisible in a toy script.

## Research method

My default loop is:

```text
establish current state
→ separate observed / supplied / assumed
→ identify the unresolved edge
→ form the smallest testable model
→ build or probe
→ compare expected vs observed
→ preserve evidence
→ revise only what the evidence requires
→ continue
```

## What counts as evidence

Depending on the problem:

- reproducible tests
- source code
- logs
- screenshots or browser witnesses
- structured records
- API responses
- file diffs
- runtime events
- state snapshots
- external documentation
- counterexamples
- repeated successful predictions

A claim should stay proportional to the evidence supporting it.

## Research identity

I am interested in problems where the category is not obvious yet.

That means I am often doing some combination of:

- specification recovery
- failure localization
- recursive decomposition
- system-boundary analysis
- representation translation
- constraint-preserving transformation
- reconciliation
- provenance engineering
- tool construction
- cross-domain transfer

The common thread is recovering enough structure to make the next valid move without losing how that move was justified.
