# 04-figure-selection - Stage 4: Figure selection

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Stage](https://img.shields.io/badge/Stage-4%20of%207-orange.svg)](.)
[![Figures](https://img.shields.io/badge/Figures-9%20%2B%20cover-lightgrey.svg)](.)
[![Tables](https://img.shields.io/badge/Tables-11-lightgrey.svg)](.)

Stage 4 runs [`../sub-prompts/prompt-4-figure-selection.md`](../sub-prompts/prompt-4-figure-selection.md):
it assigns the correct visual type to every slot in the bill, choosing a gray-scale
Mermaid diagram for each process/lineage/decision/layering and a full-width table
for each schedule/crosswalk/register/matrix. The result is
[`output-4-figure-selection.md`](output-4-figure-selection.md).

## What this stage produced

- A **figure inventory** of nine numbered gray-scale Mermaid figures plus a cover
  figure, each a different diagram type (no pattern overused).
- A **table inventory** of eleven full-width tables across the operative sections
  and the deliverable appendices.
- Placement rules (centering, captions, `\textwidth` ragged-right tables, continuous
  numbering, table-of-contents reachability) the bill stages follow.

## Sources used from other repositories (Rule 6)

| No. | Used here | Upstream source | Where used |
|:--|:--|:--|:--|
| 04 | Visual taxonomy and per-work visual catalogs | `cancer-automated/.../VVUQ-05/update-bill/figures-bill/README.md`, `01RootREADME.md`-`05VVUQ04.md` | Catalog-source column of both inventories |
| 04 | Figure-selection prompt template | `cancer-automated/.../VVUQ-05/update-bill/figures-bill/prompt-figures-bill.md` | Adapted into `../sub-prompts/prompt-4-figure-selection.md` |
| 03 | Gray-scale Mermaid diagram set | `../03-mermaid-selection/output-3-mermaid-selection.md` | Figure types and figure-slot map |
| - | Figure/table inventory model | `cancer-automated/.../VVUQ-05/final-bill/README.md` (figure and table inventory) | Inventory structure |

## Output to later stages

The figure and table inventories are the contract the `draft-bill`, `full-bill`, and
`final-bill` stages implement: which slot gets a `mermaidfig`, which gets a
full-width table, and where each lives in the bill.

## License

Released under CC BY 4.0. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
