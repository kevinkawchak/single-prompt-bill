# 03-mermaid-selection - Stage 3: Mermaid selections (gray-scale)

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Stage](https://img.shields.io/badge/Stage-3%20of%207-orange.svg)](.)
[![Diagrams](https://img.shields.io/badge/Diagrams-9%20gray--scale%20Mermaid-lightgrey.svg)](.)

Stage 3 runs [`../sub-prompts/prompt-3-mermaid-selection.md`](../sub-prompts/prompt-3-mermaid-selection.md):
it converts the colored Mermaid diagram families to **gray-scale** and re-themes
them to the bill's subject, choosing different and most relevant diagram types
throughout. The result is
[`output-3-mermaid-selection.md`](output-3-mermaid-selection.md).

## Diagram set (nine, all gray-scale, all distinct types)

flowchart LR (lineage), paired flowchart TB (timeline), BPMN flowchart (gate
decision), clustered component (statutory layering), component flowchart (section
order), swimlane (pre-introduction path), sequence (handoff), C4 architecture (the
gate as a system), and a hybrid flowchart (prompt and bill-version evolution). Each
is mapped to a bill figure slot in the figure-slot table.

## Sources used from other repositories (Rule 6)

| No. | Used here | Upstream source | Where used |
|:--|:--|:--|:--|
| 03 | Mermaid diagram families (flowchart, sequence, component, swimlane, BPMN, C4, clustered) | `Clinical-AI-Demos/tree/main/ai-outputs/output-01/ChatGPT.md` | Converted to gray-scale and re-themed in `output-3-mermaid-selection.md` |
| 03 | Mermaid rendering/index conventions | `Clinical-AI-Demos/.../ai-outputs/output-01/README.md` | Palette and figure-slot map |
| - | Bill subjects to re-theme onto | `cancer-automated/.../VVUQ-05/final-bill/sections` (lineage, gate, layering, timeline) | Diagram content |

## Output to later stages

The figure-slot map and the nine gray-scale Mermaid sources are the inputs to Stage
4 (figure selection) and to the three bill stages, which render each diagram as a
gray-scale TikZ `mermaidfig` in LaTeX. The palette `g1`..`g5` becomes the TikZ node
styles `mmg1`..`mmg5` in `usctitle.sty`.

## License

Released under CC BY 4.0. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
