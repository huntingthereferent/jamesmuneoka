# Opinions

These are current technical positions.

They are here to be tested.

## Evidence should constrain confidence

A clean explanation is not the same thing as a demonstrated result.

Confidence should not move farther than the evidence.

## Unknown is a valid technical state

Missing evidence is not a blank that needs to be filled.

Sometimes the correct state is still unknown.

Keep it unknown until something earns the next move.

## Real integrations need real-system tests

Mocks can prove isolated behavior.

They cannot prove that an API, browser, filesystem, repository, feed, deployment target, or user workflow actually works.

If the boundary matters, test the boundary.

## Failed experiments belong in the record

A failed branch can remove a possibility, expose a hidden dependency, break an assumption, or show that the boundary was wrong.

That is progress.

## Small proofs beat large speculative architecture

When the difficult part is still uncertain, more infrastructure can hide the problem.

Prove the hard part where it can fail clearly.

Then build around what survived.

## Provenance is part of system quality

A result should carry enough ancestry to answer:

- where did this come from?
- what changed it?
- what evidence supported that change?

Observability is not only metrics.

It is also lineage.

## Representation is not reality

The same state can look different in code, files, APIs, databases, and interfaces.

Different representation does not automatically mean different meaning.

## Automation should preserve context

Making an action happen is the easy part.

The useful part is keeping enough context that the next action still makes sense.

## Tools should reduce translation cost

A person should not have to keep translating the problem into the tool's vocabulary.

The tool should meet the problem closer to where it already exists.

## Existing systems should keep their native meaning

Integration does not require flattening everything into one universal shape.

Local structure can stay local while the useful relations between systems are preserved.

## Research and engineering belong in the same loop

Some questions do not exist until the system is built.

Some implementations do not become clear until they are treated like experiments.

Separate them too early and both get weaker.

## Repositories should make one understandable claim

A larger body of work can stay connected without making every project explain everything.

Each repository should have a job a stranger can understand.

## Positions move when the evidence moves

If a better experiment, implementation, or counterexample breaks one of these positions, change the position.
