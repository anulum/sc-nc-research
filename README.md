<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-RESEARCH — repository foundation
-->

# SC-NC Research

SC-NC Research is being built as the research layer split out of SC-NeuroCore: the hypothesis manifests and scoped experiments that frame exploratory work, and the research packages that build on every other SC-NC repository. It imports the SC-NC repositories before it in the split order, from SC-NC Core to SC-NC Bench. This checkout contains repository validation tooling and documentation only. Full foundation qualification is in progress. There is no installed experiment runner, hypothesis registry, research package or qualified record schema.

**What does not exist yet:**
- any code moved from SC-NeuroCore;
- a registered runtime record schema;
- an installed experiment runner, hypothesis registry or research package.

## Boundary

**What this project owns:**

| Record | Scope |
|---|---|
| Hypothesis manifest | A hypothesis, its prediction and the evidence that would refute it, stated before the experiment |
| Scoped experiment | An experiment's scope, inputs, method and results, tied to its hypothesis |

**Static imports:** only SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data, SC-NC Analysis, SC-NC Compiler, SC-NC Hardware, SC-NC Learn, SC-NC Bridges, SC-NC Verify and SC-NC Bench.

**Records read without importing their code:** Experiment Ledger and Scientific Discovery and Experimentation read this repository's records.

**Records it reads without importing their code:** those of SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data, SC-NC Analysis, SC-NC Compiler, SC-NC Hardware, SC-NC Learn, SC-NC Bridges, SC-NC Verify, SC-NC Bench and Scientific Discovery and Experimentation.

**Code planned to move here from SC-NeuroCore,** package by package, when SC-NeuroCore's split import gate allows it: `scpn`, `quantum`, `quantum_cognition`, `bio`, `bioware`, `chaos`, `evo_substrate`, `experimental`, `experiments`, `generative`, `hdc`, `neuro_symbolic`, `reservoir`, `sleep`, `swarm`, `world_model`, `control`, `ensembles`, `graphs`, `physics`, `robotics`, `security`, `spatial`, `symbolic` and `transformers`.

**Explicit non-claims and operating boundaries:**
- Research packages are exploratory; none is a qualified capability.
- A hypothesis is not a finding until its experiment supports it.

## Current tooling

Repository controls inspect:
- metadata and source attribution;
- workflows and dependency alignment;
- native documentation and repository inventory;
- preflight orchestration.

Metadata declares architecture-only maturity with empty implemented domain capability and claim inventories.

- Use the exact environment in [Contributing](CONTRIBUTING.md).
- Full CI and preflight belong in CI or in an explicitly admitted pre-push environment.
- See [Validation](VALIDATION.md) for the maintained validation scope.

## Intended evidence

Every future record will carry its source and environment digests, its numeric formats where it has them, and its explicit verification boundary. None of the planned record schemas is registered or qualified by this foundation.

## Documentation and support

Read [Architecture](ARCHITECTURE.md), [support](SUPPORT.md), [security reporting](SECURITY.md) and [citation metadata](CITATION.cff).

**Not claimed:**
- a hosted service, released package or DOI;
- a public CI status;
- a performed simulation, hardware measurement or benchmark result.

## Licence

Source is licensed under [AGPL-3.0-or-later](LICENSE). A commercial licence is available through the contact in [NOTICE](NOTICE.md).

![ANULUM](docs/assets/anulum_logo_company.jpg)

![Fortis Studio](docs/assets/fortis_studio_logo.jpg)

## Text and data mining reservation
The rightsholder, Miroslav Šotek (ANULUM), expressly reserves the use of the
works in this repository for text and data mining, including the collection of
this content for, and its use in, training, fine-tuning or evaluating machine
learning and artificial intelligence models, in accordance with Article 4(3) of
Directive (EU) 2019/790 and the national provisions transposing it.

No permission for such use has been granted beyond what the licence in
`LICENSE` grants. This reservation does not change that licence: uses the
licence permits remain permitted on its terms, including its attribution and
share-alike conditions.

Reservation made on 2026-11-22. Requests for permission: contact the
rightsholder through the contact listed in this repository.
