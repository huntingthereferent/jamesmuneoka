# Projects

This repository is the public map of James Muneoka's current engineering and research work.

## Language Network

**Type:** systems platform / web application / research infrastructure

**Focus:** continuity across people, tasks, information, external sources, and software systems.

Current areas include shared web frontage, live feed integration, social/news movement, task and calendar workflows, education workflows, public-data monitoring, project navigation, provenance and traceability, and reusable tools inside larger workflows.

The project is designed so individual systems can keep their own state while still participating in a larger connected workflow.

## Eggy

**Type:** experimental systems research

**Focus:** observing and testing movement across different technical layers.

The repository preserves discovery probes, bounded experiments, implementation history, counterexamples, failures, provenance records, and earlier architectural branches.

It functions as both a laboratory and an evidence archive.

## Axioms

**Type:** minimal research kernel

**Focus:** reducing larger ideas to small rules that can be tested independently.

The project deliberately stays smaller than the surrounding systems so foundational claims can be tested without inheriting unnecessary application architecture.

## Public-data systems

A recurring engineering pattern in this work is:

public API / scraper -> Python ingestion -> validation -> PostgreSQL -> FastAPI -> web UI -> Docker -> GitHub Actions -> deployment -> monitoring -> automated tests

The specific data source may change. The transferable capability is building the complete path from external data to a usable, monitored application.

## Workflow and automation systems

Another recurring area is software that coordinates tasks, schedules, external information, human decisions, state changes, handoffs between tools, and persistent evidence of what happened.

These systems are treated as engineering problems rather than isolated scripts.

## Portfolio rule

Each repository should make one understandable claim.

A reader should be able to understand what a project does without first understanding every other project.

The larger body of work becomes visible through the relationships between the repositories.
