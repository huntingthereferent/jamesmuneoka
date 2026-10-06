# Ability

Ability is easier to show than describe.

This page is a map of work that can be demonstrated through systems, experiments, traces, tests, and artifacts.

## Technical research

Turn an unclear technical problem into something bounded enough to test.

That includes:

- specification recovery
- unknown-system tracing
- hypothesis formation and falsification
- failure localization
- counterexample-driven refinement
- reproducible experiment design
- evidence preservation
- provenance analysis
- recursive decomposition
- technical documentation

## Systems and software engineering

Carry a problem from source to working application:

```text
public API / scraper
→ Python ingestion
→ validation / reconciliation
→ PostgreSQL
→ FastAPI
→ web UI
→ Docker
→ GitHub Actions
→ deployment
→ monitoring
→ automated tests
```

The stack can change.

The ability is keeping the system coherent across the whole path.

## Data engineering and reconciliation

Work includes:

- structured data transformation
- ETL-style pipelines
- schema-tolerant ingestion
- identity and record matching
- validation
- reconciliation
- lifecycle/history tracking
- incomplete information
- legacy data
- CSV / Excel workflows
- persisted decision records

## APIs, automation, and integration

Systems can be entered and connected through:

- public APIs
- HTTP
- scraping
- browser automation
- command-line tools
- filesystems
- repositories
- external feeds
- existing codebases
- event/state handoffs

## QA and verification

Tests are built around what the system is supposed to preserve.

That includes:

- acceptance-test design
- regression testing
- state-transition checks
- browser/E2E witnesses
- failure and recovery testing
- comparison against source records
- transformation verification

## AI and agent work

AI/agent systems are useful inside evidence-grounded workflows.

The model output is not the proof.

Work includes:

- agent evaluation
- tool-use workflows
- bounded reasoning experiments
- state/provenance capture
- failure analysis
- human/agent handoffs

## Investigation and source work

Technical questions often live across more than one source.

Useful evidence may come from code, public records, documentation, timestamps, repositories, APIs, or runtime behavior.

The work is in keeping observed facts separate from inference while still moving toward an answer.

## Tool construction

When an interface hides the part that needs inspection, build a smaller tool around the missing view.

Common shapes:

- inspectors
- validators
- scanners
- reconciliation utilities
- data converters
- monitoring interfaces
- evidence collectors
- task/workflow tools
- research harnesses

## Cross-domain transfer

A method can move without pretending the domains are identical.

Carry forward what survives.

Relearn what does not.

## Evidence base

Current repositories:

- [Language Network](https://github.com/huntingthereferent/language-network)
- [Eggy](https://github.com/huntingthereferent/eggy)
- [Axioms](https://github.com/huntingthereferent/axioms)

The next step for this file is tighter evidence linking: capability → artifact → test / trace / repo.
