<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-RESEARCH — repository foundation
-->

# Repository architecture

## Current executable tooling

**What it contains:** the repository's metadata, source-provenance, workflow, dependency-alignment, documentation, inventory and preflight controls.

**What each control does:** it inspects its fixed, declared local scope.

**What received metadata cannot do:** select another acceptance policy or grant domain authority.

Foundation qualification is in progress.

## Intended domain boundaries

| Record | Responsibility | Required evidence |
| --- | --- | --- |
| Hypothesis manifest | A hypothesis, its prediction and the evidence that would refute it, stated before the experiment | The manifest is recorded before the experiment runs |
| Scoped experiment | An experiment's scope, inputs, method and results, tied to its hypothesis | Results reported against the manifest's prediction, including refutation |

## Planned record schemas

- `sc_nc_research.hypothesis_manifest.v1`
- `sc_nc_research.scoped_experiment.v1`

These are planned identifiers. None of them is registered or qualified here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
