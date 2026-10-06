# Opinions

These are working technical positions, not permanent doctrine.

They exist because building and researching systems produces judgment. I would rather make that judgment visible than pretend technical work is opinion-free.

## Evidence should constrain confidence

A clean explanation is not the same thing as a demonstrated result.

I prefer claims that remain proportional to the evidence behind them.

## Unknown is a valid technical state

Missing evidence should not be silently converted into certainty.

A system that can preserve uncertainty is often more trustworthy than one that always produces an answer.

## Real integrations should be tested against real systems

Mocks are useful for isolated behavior.

They are not evidence that an API, browser, filesystem, repository, feed, deployment target, or user workflow actually works.

When the boundary matters, test the boundary.

## Failed experiments belong in research

A failed branch can eliminate a possibility, expose a hidden dependency, reveal an invalid assumption, or show that the boundary was drawn incorrectly.

That is useful output.

## Small proofs beat large speculative architecture

When the difficult part is uncertain, infrastructure can hide the uncertainty instead of solving it.

I prefer proving the difficult relation in the smallest environment where it can actually fail.

## Provenance is part of system quality

If a result matters, I want to know where it came from, what transformed it, and what evidence supported the transformation.

Observability is not only metrics. It is also ancestry.

## Representation should not be confused with reality

The same underlying state can appear differently in code, files, APIs, databases, and interfaces.

A representation change is not automatically a semantic change.

## Automation should preserve context

Automating an action is easy.

The harder and more useful problem is preserving enough context that the next action still makes sense.

## Tools should reduce translation cost

A good tool helps a person stay inside the problem.

It should not force them to repeatedly translate their intent into the software's internal vocabulary.

## Existing systems deserve to keep their native meaning

I do not think every source needs to be flattened into one universal schema.

Integration can preserve local structure while still creating useful continuity across systems.

## Research and engineering should not be separated too early

Many useful technical questions only become visible once something is actually built.

Likewise, many implementations improve when treated as experiments rather than finished answers.

I prefer a loop where research and engineering inform each other.

## Repositories should make one understandable claim

A body of work can be connected without requiring a reader to understand everything at once.

Each repository should have a legible job.

## Opinions should be revisable

A technical opinion should survive contact with evidence.

If a better experiment, implementation, or counterexample breaks one of these positions, the position should move.
