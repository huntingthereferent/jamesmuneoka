# Opinions

These are working technical positions, not permanent doctrine.

They are here because building things produces opinions, and making those opinions explicit makes it easier to see what I optimize for and what evidence would change my mind.

## Software should preserve why something happened

A result is more useful when you can still tell where it came from, what changed, and which earlier state or source it depended on.

I prefer inspectable movement over opaque convenience.

## Real integrations should be tested against real systems

Mocks are useful for isolated behavior.

They are not evidence that an API, browser, filesystem, repository, feed, deployment target, or user workflow actually works.

When the boundary matters, test the boundary.

## Failed experiments are part of the product

Deleting every failed branch makes research look cleaner and makes the next decision worse.

A failed experiment is useful when it removes a possibility, exposes a hidden dependency, or shows that the boundary was drawn incorrectly.

## Small proofs beat large speculative architecture

When the hard part of a system is still uncertain, adding more infrastructure usually makes the uncertainty harder to see.

I prefer proving the difficult part in the smallest environment where it can actually fail, then expanding around evidence.

## Tools should reduce translation cost

A good tool should let a person keep moving through the problem instead of forcing them to repeatedly translate their intent into the internal structure of the software.

Interfaces should organize complexity without pretending the complexity disappeared.

## External systems should stay themselves

I do not think every source needs to be copied into one universal internal model.

A useful integration can preserve the source's native state and still maintain enough context to connect it to the larger workflow.

## Automation should carry evidence, not just actions

Automating an action is easy.

The more interesting problem is preserving enough state, provenance, and decision context that the next action still makes sense.

## Repositories should make one understandable claim

A large body of work can be connected without making every project depend on understanding the whole theory first.

Each repository should have a legible job.

## I expect these opinions to change

A technical opinion should survive contact with evidence.

If a better implementation, experiment, or counterexample breaks one of these positions, the opinion should move.
