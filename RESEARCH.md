# Research

The interesting problems are usually the ones where the category is not obvious yet.

That means entering a system before its shape is clean, finding what is actually present, and recovering enough structure to make the next valid move.

The research is built from working code, bounded experiments, traces, state captures, counterexamples, and reproducible tests.

## Questions

- What is the system actually doing?
- Which parts are state, representation, interface, or interpretation?
- Where does the expected path stop matching the observed one?
- Which difference changes meaning and which one only changes form?
- What has to survive when information moves between tools or layers?
- How much can be compressed before the evidence is no longer recoverable?
- Can a process keep moving without filling missing evidence with invention?
- What survives when a method moves into a different domain?

## Unknown-system tracing

Start with the current state.

Change one thing.

Watch what moves.

Trace the dependency until the first unsupported jump appears.

That pattern has been used across repositories, filesystems, APIs, structured data, runtimes, browser surfaces, command-line tools, and external services.

## Evidence and provenance

A result is stronger when its ancestry is still reachable.

Useful provenance can include:

- source evidence
- state transitions
- timestamps
- transformation history
- test outcomes
- decision records
- failure traces
- cross-layer handoffs

The goal is not to preserve everything forever.

The goal is to preserve enough that the movement can still be inspected.

## Agent and reasoning evaluation

Bounded environments make reasoning failures visible.

The useful trace is:

```text
observed
→ predicted
→ contradicted or supported
→ retained or revised
→ next move
```

A final score is not enough by itself.

The path matters because that is where unsupported assumptions, false confidence, recovery, and actual rule discovery become visible.

## Representation and reconciliation

The same thing can appear differently depending on where it is observed.

Examples:

- code vs runtime behavior
- file vs parsed structure
- API response vs UI
- source record vs reconciled record
- current state vs historical state

The job is to separate meaningful change from representational change.

## Applied systems research

Full systems are useful research instruments.

A public-data application can expose questions about identity, ingestion, reconciliation, failure semantics, recovery, observability, and provenance that do not appear in a toy example.

Building the system is part of finding the question.

## Research movement

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

## Evidence

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

Confidence should not outrun the evidence.

## Research identity

The recurring work is some combination of:

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

The common thread is simple:

recover enough structure to move without losing why the move was valid.
