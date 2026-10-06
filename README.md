# James Muneoka

I build systems around a simple constraint:

> Preserve the referent, preserve the evidence, and do not invent the movement between them.

The work here moves from small mathematical contracts into larger systems without treating a higher layer as permission to erase what was demonstrated below it.

## Current stack

### [Axioms](https://github.com/huntingthereferent/axioms)

The clean mathematical layer.

Axioms starts with one object and one recursively reusable operation:

```text
X0 --A/B--> X1 --A/B--> X2
```

The output must remain admissible as input under the same evidentiary contract. No hidden human orientation is allowed between applications.

**Current question:** what is the smallest relation that survives recursive reuse without adding an unsupported higher-layer operator?

---

### [Eggy](https://github.com/huntingthereferent/eggy)

Preserved implementation history and evidence bank.

Eggy contains working artifacts, counterexamples, failure modes, movement observations, provenance, and experiments accumulated while exploring continuity across native layers.

It is not the mathematical ground. It is evidence.

```text
implemented artifact history
!=
current mathematical justification
```

---

### [Language Network](https://github.com/huntingthereferent/language-network)

The outward systems layer.

Language Network studies how continuity can survive movement through people, conversations, work, time, connected systems, and the wider internet while each source keeps its own native state.

Its core movement is:

```text
current referent
-> required relation
-> enter required layer
-> witness / model / build / measure
-> preserve provenance
-> return result as valid input
-> continue
```

External systems remain external. The network preserves why they were touched, what relation they added, and how the current state descended from prior evidence.

## How the repositories relate

```text
Axioms
  mathematical contract
       |
       v
Eggy
  experiments + witnesses + failure history
       |
       v
Language Network
  translation across domains and operating systems
       |
       v
applications / tools / public proofs
```

Movement can also go backward. A real application may expose a missing relation, which returns the work to the smallest layer where the distinction can actually be justified.

## Working discipline

- Language first, then math one layer up, then implementation.
- Unsupported movement is not promoted into movement.
- UNKNOWN may remain UNKNOWN.
- Similarity is not evidence of continuity.
- Coverage is not automatically preservation.
- Provenance must survive any movement that depends on it.
- A result should become valid input again whenever recursion is claimed.
- Older implementations may remain evidence without defining the next architecture.

## What I publish

This repository maps several different kinds of artifacts:

| Layer | Artifact |
|---|---|
| Ground | mathematical contracts and invariants |
| Evidence | witnesses, counterexamples, traces, experiments |
| Translation | protocols that carry supported movement between layers |
| Systems | applications built without discarding provenance |
| Reviews | audits of what changed, what survived, and what remains unknown |

The goal is not to make every repository look the same. The goal is to make the movement between them inspectable.

## Current repositories

- **[Axioms](https://github.com/huntingthereferent/axioms)** — recursive mathematical ground.
- **[Eggy](https://github.com/huntingthereferent/eggy)** — preserved evidence and implementation history.
- **[Language Network](https://github.com/huntingthereferent/language-network)** — continuity across human, software, organizational, and internet surfaces.

See [PROJECTS.md](PROJECTS.md) for the portfolio map and [docs/RESEARCH_METHOD.md](docs/RESEARCH_METHOD.md) for the working research loop.
