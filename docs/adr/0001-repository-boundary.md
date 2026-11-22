<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-RESEARCH — repository foundation
-->

# Decision: give SC-NC Research its own repository in the SC-NeuroCore split

## Context

SC-NeuroCore holds every layer of the stack in one package, so a change to one layer can reach every other, and its import graph has cycles that no single layer can be qualified across. The split gives each layer its own repository, in an order in which a repository imports only those before it.

## Decision

**What SC-NC Research owns:**
- hypothesis manifest;
- scoped experiment.

**What it imports:** SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data, SC-NC Analysis, SC-NC Compiler, SC-NC Hardware, SC-NC Learn, SC-NC Bridges, SC-NC Verify and SC-NC Bench. Its records are read by Experiment Ledger and Scientific Discovery and Experimentation, and it reads those of SC-NC Core, SC-NC Catalogue, SC-NC Engine, SC-NC Data, SC-NC Analysis, SC-NC Compiler, SC-NC Hardware, SC-NC Learn, SC-NC Bridges, SC-NC Verify, SC-NC Bench and Scientific Discovery and Experimentation.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| analysis and statistics | SC-NC Analysis |
| the experiment record | Experiment Ledger |
| qualified capabilities | the SC-NC repository that owns each one |

## Consequences

**What can be qualified now:** repository governance and validation tooling, before any code moves here.

**What it cannot qualify:** unmoved code, unimplemented schemas or results.

**Architectural consequences:**
- code moves here only through SC-NeuroCore's split import gate, unit by unit, with its tests and language counterparts;
- SC-NC Research never imports a repository later in the split order;
- SC-NeuroCore keeps a facade for each moved package until its users have moved.
