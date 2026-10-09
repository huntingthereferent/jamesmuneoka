## Research method / operational notes

This is a procedure for producing challengeable results, not a universal algorithm that already solves every class of problem.

### The witness

For interactive work, keep a native `state → permitted action → returned state` triple. For data work, keep original record → transformation → resulting record. For software, retain the input, executed process, output, failure and environment constraints.

The evidence-bearing object changes by domain. It is not automatically a hash, a summary, or a favorite internal representation.

### Admission sequence

1. **Locate the referent.** What is the actual system and native observation?
2. **Separate claims.** Observed, supplied, inferred, proposed, and unknown must not collapse.
3. **Find the smallest valid intervention.** It should distinguish at least two possible models.
4. **Predict before running.** State what should change or survive.
5. **Execute against the real boundary** when permitted; use a mock only for the part it actually tests.
6. **Compare returned evidence.** Capture a counterexample rather than smoothing it away.
7. **Promote narrowly.** A passing test means what it tested, under the conditions it tested.
8. **Preserve the next edge.** State what is still missing and what would count as its resolution.

### Navigation and construction are different requests

Inspecting an existing structure usually calls for navigation, comparison, and evidence recovery. Generating alternative structures calls for a construction direction using tested constraints.

Construction is **conditional**, not an expensive automatic inverse at every step. Candidate worlds or simulations must return to the same evaluator. The general construction theory is under investigation; the existence of a candidate is not proof that its rules or solution are valid.

### Outputs

A reproducible observation, narrow tool, state-transition trace, regression test, counterexample, or an explicit unresolved boundary. When the work is not finished, say so.

[Research notebook](../RESEARCH.md) · [Evidence status](../PROVENANCE.md)
