# 02-template-selection - Stage 2: Template bill selection

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Stage](https://img.shields.io/badge/Stage-2%20of%207-orange.svg)](.)
[![Chosen](https://img.shields.io/badge/Chosen-output--03%20(genre--diverse)-blue.svg)](.)

Stage 2 runs [`../sub-prompts/prompt-2-template-selection.md`](../sub-prompts/prompt-2-template-selection.md):
it picks one LaTeX template set for the v4.0 bill and its twelve LaTeX deliverables,
and maps each deliverable to a matching document genre. The result is
[`output-2-template-selection.md`](output-2-template-selection.md).

## Decision

**`Clinical-AI-Demos/ai-outputs/output-03`** (the genre-diverse set) is chosen over
`output-02` (shared-skeleton reskins), because each of the twelve legislative
deliverables is its own document genre with the devices that deliverable needs, and
because the deliverables in v4.0 must be converted faithfully to LaTeX and listed in
the bill's table of contents (Rule 2). The templates' green ORCID logo image is
replaced by a black text ORCID hyperlink, since no images are permitted (Rule 5).

## Sources used from other repositories (Rule 6)

| Used here | Upstream source | Where used |
|:--|:--|:--|
| Template set comparison | `Clinical-AI-Demos/.../ai-outputs/output-02/README.md` and `output-03/README.md` | The decision table |
| Inspected template (Ramseyer) | `Clinical-AI-Demos/.../ai-outputs/output-03/LaTeX-Source-Files-05.zip` (`tmpl05style.sty`, `sections/section-a.tex`) | Confirming genre devices |
| Template-generation prompt | `Clinical-AI-Demos/.../ai-outputs/output-02/prompt.md` | Adapted into `../sub-prompts/prompt-2-template-selection.md` |
| Deliverable list (1-12) | `cancer-automated/.../VVUQ-05/final-bill/deliverables` | Deliverable-to-genre map |
| Bill style ancestor | `cancer-automated/.../VVUQ-05/final-bill/usctitle.sty` | Style basis for all bill stages |

## Output to later stages

The deliverable-to-genre map in `output-2-template-selection.md` is the contract
the `draft-bill`, `full-bill`, and `final-bill` stages follow when they write the
twelve appendix `.tex` files (Appendix A through Appendix L).

## License

Released under CC BY 4.0. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
