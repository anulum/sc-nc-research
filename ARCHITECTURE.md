<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-RESEARCH — repository foundation
-->

# Architecture

## Current executable surface

The checkout contains:
- repository validation tooling;
- dedicated tests;
- workflow definitions;
- native documentation.

No domain component of SC-NC Research is implemented yet, and no code has moved here from SC-NeuroCore. The metadata keeps domain capabilities, claims and qualified record formats empty.

## Intended records

1. **Hypothesis manifest:** A hypothesis, its prediction and the evidence that would refute it, stated before the experiment.
2. **Scoped experiment:** An experiment's scope, inputs, method and results, tied to its hypothesis.

## Ownership

**This project owns** the planned SC-NC Research records and boundary rules.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| analysis and statistics | SC-NC Analysis |
| the experiment record | Experiment Ledger |
| qualified capabilities | the SC-NC repository that owns each one |
| the public package, documentation and releases of the monolith | SC-NeuroCore |

## Interpretation

- **Research.** An experiment's result is bounded by its manifest.
- **Moves.** Code arrives only through SC-NeuroCore's split import gate, unit by unit; a planned move is not a moved capability.

Read [the documentation architecture](docs/ARCHITECTURE.md) for the planned records, rules and schema identifiers.
