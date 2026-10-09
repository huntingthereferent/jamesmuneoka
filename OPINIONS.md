## Working positions

These are positions I use to make engineering decisions. They are not laws. A contradictory witness should change the position.

#### A convincing result is not necessarily an executed result

A model can describe a correct action while the tool never runs. A UI can show a state that the backend never reached. A passing mock can hide a broken real connection.

**Test:** preserve the native action and returned result. If that boundary is missing, don't promote the claim.

#### The first false assumption matters more than the prettiest explanation

An unfamiliar system is easiest to misunderstand when a convenient representation begins standing in for the whole state.

**Test:** change the environment, not just the wording of the theory. Find a case where the model should make a different prediction.

#### A local win has a local scope

Finishing known games is useful evidence of rule recovery, but not evidence that the same policy handles unseen games. Getting one generative tool step right is not proof of autonomous task completion.

**Test:** fresh starts, changed trajectories, unseen conditions, and explicit failure cases.

#### Interfaces should carry their source context

If a feed, database record, file, or agent message is transformed, the result should still have enough ancestry to recover what it came from and which parts were inferred.

**Test:** follow the output back to the actual source, not merely to a friendly summary.

#### Unknown is a result, not a writing defect

When a dependency, evidence source, or action boundary is missing, filling the gap with confident language makes the system worse.

**Test:** leave the missing condition visible and name the next observation that could resolve it.

#### Building a system can be a research experiment

Some questions are only exposed by making the parts communicate. But a completed diagram is not a completed integration.

**Test:** cross the real boundary, inspect the returned behavior, and keep what failed.

#### Reuse should preserve the parts that differ

A useful method can cross games, data, automation, and software without pretending that their native states are the same.

**Test:** name what the method preserves in the new domain. When that relation breaks, stop generalizing.


[Research notebook](RESEARCH.md) · [Case records](SELECTED_WORK.md) · [Back to profile](README.md)
