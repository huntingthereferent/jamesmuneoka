# Selected work

Technical work is more useful when the claims, the test, and the limits are visible together.

This page distinguishes **measured local results**, **active development**, and **next builds**. The working source for some projects is private; a private repository is not presented here as public proof.

## Interactive environments — agent evaluation and state recovery

**Status:** Measured in local ARC-AGI-3 environments, October 2026. Research/test artifacts are not yet published in this repository.

An unfamiliar interface does not begin with a trustworthy instruction manual. I inspect which actions change the observable state, compare predictions with the next observation, and keep counterexamples when the model breaks.

| Environment | Verified local result | What the work tested |
| --- | --- | --- |
| SK48 | 8/8 levels, 280 actions; two fresh-game winning replays | State compression, moving structures, collision rules, controller switching |
| LS20 | 7/7 levels, 309 actions; two fresh-game winning replays | Route recovery, move budgets, pickups, launchers, moving switches |
| FT09 | 6/6 levels, 75 actions; two fresh visual-agent winning runs | Pixel-decoded controls, color constraints, click effects, re-planning |

The local SDK reported a 100.0 game score for each of these runs. **These are individual public-game results, not an ARC Prize competition score or a claim of general agent performance.**

The FT09 visual policy was also tested after an extra exploratory action on each level: two fresh runs still won, in 81 and 76 actions. It correctly declined nine unrelated public game observations. The working policy used rendered frames during execution; earlier investigation was source-assisted. That distinction matters.

**What survives:** observable change, state, constraints, predicted-versus-actual outcomes, useful failed experiments, and reproducible tests. The implementation changes by environment.

**Evidence access:** The replay and test records are currently in local research archives. This page records measured outcomes, but does not substitute for public source code. Publication and reproducibility packaging are separate work.

## Continuity and cross-system applications

**Status:** Ongoing development; source repository private.

A shared runtime for passing bounded work between systems while keeping each system's local meaning intact. Areas under development include human/agent handoffs, event history, task and calendar workflows, public-data feeds, education workflows, and traceable research outputs.

This work crosses data formats, interfaces, persistent state, and execution boundaries. Architectural descriptions are not production deployment claims.

## Experimental systems research

**Status:** Private research archives.

Smaller experiments trace specification gaps and state transitions across code, filesystems, repositories, HTTP, command-line tools, and browser surfaces. The point is to reduce a large unknown into a testable difference and keep enough evidence to repeat it.

## Currently building toward

**Status:** Work direction, not a claim of a finished production deployment.

A complete public-data monitoring application: Python ingestion, source validation, record reconciliation, PostgreSQL, FastAPI, a usable web interface, Docker/CI, deployment, and monitoring. Each boundary needs an end-to-end test rather than a box on a stack diagram.

The next public work examples should show the actual input, failure or requirement, implementation, test, and usable output.

See [Capabilities](ABILITY.md), [Research](RESEARCH.md), and [Working with me](WORK_WITH_ME.md).
