# James Muneoka

**Independent Technical Researcher · Systems Investigator · Software / Data / Automation Builder**

I work on problems that cross software, data, automation, AI/agent behavior, and real-world system boundaries.

I usually start where the structure is unclear: establish what is actually present, trace what changes, locate where expectations stop matching reality, and build the smallest useful thing that makes the next step testable.

## Research

Research is a primary part of my work, not an afterthought to software development.

I investigate unfamiliar systems through working code, bounded experiments, traces, counterexamples, state captures, and reproducible tests.

Current interests include:

- unknown-system tracing
- specification recovery
- evidence and provenance
- agent/reasoning evaluation
- failure localization
- representation translation
- reconciliation
- state and dependency tracing
- recursive decomposition
- cross-domain transfer
- applied systems research

See **[RESEARCH.md](RESEARCH.md)**.

## Ability

My work spans more than application development.

I have demonstrated work in:

- technical research and experimental design
- Python and backend/API development
- data ingestion, transformation, validation, and reconciliation
- PostgreSQL and persisted application state
- FastAPI and web interfaces
- Docker and CI/CD
- automated and acceptance testing
- browser/E2E verification
- public APIs, scraping, and external integrations
- filesystems, repositories, HTTP, structured data, and runtime investigation
- AI/agent tooling and evaluation
- provenance and evidence systems
- OSINT-style technical investigation
- legacy-data and existing-code analysis
- tool construction and workflow automation

See **[ABILITY.md](ABILITY.md)** for the fuller capability map.

## Opinions

I think researchers and engineers should be allowed to have visible technical judgment.

My opinions are working positions earned from building and testing things, not permanent doctrine.

A few:

- evidence should constrain confidence;
- unknown is a valid technical state;
- failed experiments are part of research;
- real integrations should be tested against real systems;
- provenance is part of system quality;
- representation should not be confused with reality;
- research and engineering should inform each other;
- automation should preserve context, not only perform actions.

See **[OPINIONS.md](OPINIONS.md)**.

## Current projects

### [Language Network](https://github.com/huntingthereferent/language-network)

A continuity and systems project spanning live external feeds, task/planning systems, education workflows, public-data tooling, research navigation, provenance-preserving handoffs, interfaces, and cross-system state.

### [Eggy](https://github.com/huntingthereferent/eggy)

An experimental systems-research repository preserving probes, implementations, tests, movement traces, failure cases, provenance, and earlier technical branches across filesystems, repositories, HTTP, structured data, runtimes, browser surfaces, CLI tools, and version control.

### [Axioms](https://github.com/huntingthereferent/axioms)

A minimal research repository used to reduce larger system questions to small, testable foundations before surrounding architecture is allowed to grow.

## End-to-end engineering

One recurring project shape is:

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

I care about the whole path: acquisition, transformation, persistence, interfaces, failure behavior, recovery, verification, and operation.

## Working method

```text
establish state
→ separate observed / supplied / assumed
→ trace relevant relations
→ locate the unresolved boundary
→ build or probe
→ compare expected vs observed
→ preserve evidence
→ revise
→ continue
```

## More

- [RESEARCH.md](RESEARCH.md) — research identity, questions, and methods
- [ABILITY.md](ABILITY.md) — demonstrated capability map
- [OPINIONS.md](OPINIONS.md) — current technical positions
- [PROJECTS.md](PROJECTS.md) — project map
- [docs/RESEARCH_METHOD.md](docs/RESEARCH_METHOD.md) — detailed working process
