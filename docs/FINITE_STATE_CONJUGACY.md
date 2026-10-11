# Finite-state conjugacy testing

*Research report · October 2026 · locally reported mathematical experiments; public reproduction pending*

## Question

When two invertible actions on the same declared space cannot yet be distinguished, can an investigation continue the **same transformation**, retain its previous observations, and return either an obstruction, an explicit correspondence, or an honest UNKNOWN at its budget boundary?

The experiment uses two-input finite-field transformation laws on $\mathbb F_3^5$. Its watched space is a declared **81-state invariant fiber**, preserved by the action $B$. This fiber is an essential witness condition: the full state space contains 243 states and gives different observation thresholds.

The investigator continues $B, B^2, B^3,\ldots$, counting $\#\mathrm{Fix}(B^n)$ on the watched fiber.

## Negative control: a distinction at the ninth observation

Two laws share the lower-coordinate rules and differ by one admissible next-coordinate coupling.

| Continuation | First action: fixed states | Second action: fixed states | Result |
| --- | ---: | ---: | --- |
| $B^1$–$B^8$ | 0 | 0 | Inconclusive |
| $B^9$ | 81 | 0 | **Distinguished** |
| $B^{27}$ | 81 | 81 | Both return; earlier obstruction persists |

The first restricted action has **nine cycles of length 9**; the second has **three cycles of length 27**. Conjugacy of permutations preserves cycle lengths, so the restricted $B$-actions are nonconjugate. Their unequal ninth-iterate fixed-point counts give an exact obstruction.

**Scope:** On the whole 243-state space, the systems can already be distinguished by $B^3$. The ninth-step observation result is *fiber-specific*, not a statement of full-space minimality.

## Positive control: a verified restricted-action correspondence

A separate positive pair has matching three 27-cycles on its declared 81-state fiber. The report describes an explicit bijection $F$, checked against all relevant states, satisfying

$
F\circ B_{\mathrm{left}}=B_{\mathrm{right}}\circ F.
$
This is evidence of **conjugacy of the restricted $B$-actions**, not simultaneous full-space $A$/$B$ conjugacy. Matching a few invariant counts alone would not suffice; the bijection is the essential positive witness.

## Observation budgets

| Comparison | Budget | Outcome |
| --- | ---: | --- |
| Negative control | 8 | **UNKNOWN** |
| Negative control | 9 | **DISTINGUISHED** |
| Positive control | 26 | **UNKNOWN** |
| Positive control | 27 | **EQUIVALENT FOR THE DECLARED B-RELATION** |

An early stop means the permitted observation procedure has not gathered sufficient evidence. It does not prove that no other valid proof technique exists.

A separate local checkpoint-and-resume experiment reportedly serialized the current observation, restored it, and continued without changing the transformation, watched fiber, previous counts, or restricted-$B$ interpretation. The negative case progressed from UNKNOWN at budget 8 to a fixed-point obstruction at 9. The positive case progressed from UNKNOWN at 26 to an explicit restricted-action correspondence at 27.

The result is an evidence-preserving research record, not merely a final classification label.

## Evidence boundaries

The researcher reported **13/13** local native-continuation regression checks and **17/17** local re-entry checks. The complete executable experiment is not included in this public repository, and external replication has not yet been established.

This report does not claim a universal relation-construction operation, unrestricted equivalence checking, simultaneous $A$/$B$ conjugacy for the positive case, live ARC execution, or production readiness.

**For public reproduction:** publish the exact generating laws, fiber condition and invariance proof, full periodic-point tables and cycle decompositions, explicit positive bijection, serialized checkpoints, test source, and runtime instructions.

[Selected case](../SELECTED_WORK.md) · [Research notebook](../RESEARCH.md) · [Evidence status](../PROVENANCE.md)
