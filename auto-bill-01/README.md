# auto-bill-01 - Autonomous build of H. R. 9510 Bill v4.0

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Bill](https://img.shields.io/badge/Bill-H.%20R.%209510%20v4.0-darkblue.svg)](.)
[![Engine](https://img.shields.io/badge/Engine-Claude%20Code%20Opus%204.8%20(1M)%20Max-blue.svg)](.)
[![Diagrams](https://img.shields.io/badge/Diagrams-Gray--scale%20Mermaid%20only-lightgrey.svg)](.)
[![Bill DOI (v4.0)](https://img.shields.io/badge/Bill%20DOI%20(v4.0)-10.5281%2Fzenodo.xxxxxxxx-blue.svg)](https://doi.org/10.5281/zenodo.xxxxxxxx)

This directory holds the entire autonomous build of **H. R. 9510 Bill v4.0**, the
*Verification Before Generation in Physical AI Oncology Trials Act of 2026*. The
build was driven by the single [`master-prompt.md`](master-prompt.md): Process A
generated every sub-prompt under [`sub-prompts/`](sub-prompts), and Process B ran
those sub-prompts in order, producing the four research stages (`01`-`04`) and the
three bill stages (`draft-bill`, `full-bill`, `final-bill`). Every stage is a
separate pull request; every distinguishable file is a separate commit; all are
pushed in real time (Rules 7, 8, 9).

## What is new in v4.0

1. **The twelve deliverables are LaTeX, inside the bill.** In Bill v3.0 they were
   standalone Markdown; here each one is improved, updated, and converted to a
   LaTeX appendix that compiles in the bill and appears in its clickable table of
   contents (Rule 2).
2. **Gray-scale Mermaid diagrams only, no images.** Markdown files carry real
   gray-scale `mermaid` blocks; the LaTeX bill reproduces each as a gray-scale
   TikZ figure (Rule 5).

## Directory map

```
auto-bill-01/
  README.md                 (this file)
  master-prompt.md          (the single submitted Master prompt, verbatim - Rule 14)
  sub-prompts/
    README.md
    prompt-1-research.md            prompt-5-draft-bill.md
    prompt-2-template-selection.md  prompt-6-full-bill.md
    prompt-3-mermaid-selection.md   prompt-7-final-bill.md
    prompt-4-figure-selection.md
  01-research/              (Stage 1)  README.md + output-1-research.md
  02-template-selection/    (Stage 2)  README.md + output-2-template-selection.md
  03-mermaid-selection/     (Stage 3)  README.md + output-3-mermaid-selection.md
  04-figure-selection/      (Stage 4)  README.md + output-4-figure-selection.md
  draft-bill/               (Stage 5)  main.tex, usctitle.sty, references.bib,
                                       sections/, deliverables/, zip, prompt, output, README
  full-bill/                (Stage 6)  same set, fully rendered + 12 LaTeX deliverables
  final-bill/               (Stage 7)  same set, polished to v1.0.0 + 12 LaTeX deliverables
```

## Sources used from other repositories (Rule 6)

Each entry below names the upstream file or directory and the exact place it is
used in this build. Per-directory READMEs repeat the relevant rows in detail.

| No. | Asset used | Upstream source | Used in |
|:--|:--|:--|:--|
| 01 | Pre-introduction research and 2026 process facts | `cancer-automated/.../VVUQ-05/update-bill/next-steps/prompt-1-next-steps.md`, `output-1-next-steps.md` | `01-research/` |
| 02 | LaTeX template set (genre-diverse, 12 legislative genres) | `Clinical-AI-Demos/.../ai-outputs/output-03` (chosen over `output-02`) | `02-template-selection/`; deliverable `.tex` genres in all bills |
| 03 | Mermaid diagram families (flowchart, sequence, component, swimlane, BPMN, C4, clustered) | `Clinical-AI-Demos/.../ai-outputs/output-01/ChatGPT.md` | `03-mermaid-selection/`; every bill diagram |
| 04 | Visual catalog and figure-type taxonomy | `cancer-automated/.../VVUQ-05/update-bill/figures-bill/` (`README.md`, `02VVUQ01.md`-`05VVUQ04.md`) | `04-figure-selection/`; figure placement in all bills |
| 05 | Draft scaffold conventions (bracketed drafting instructions, cover ASCII -> Mermaid) | `cancer-automated/.../VVUQ-05/draft-bill/` (`prompt-draft-bill.md`, `main.tex`) | `draft-bill/` |
| 06 | Full-bill rendering conventions (figure/table inventory, DOI, deliverables split) | `cancer-automated/.../VVUQ-05/full-bill/` (`prompt-full-bill.md`, `main.tex`) | `full-bill/` |
| 07 | Final polish, `usctitle.sty`, `references.bib`, the 12 deliverables, white-space and reference formatting | `cancer-automated/.../VVUQ-05/final-bill/` | `final-bill/`; `usctitle.sty` and `references.bib` of every bill |

## Build status

**Status: complete (v1.0.0).** All nine pull requests are merged into `main`. The
authoritative record is the git history of the `claude/amazing-wozniak-gRjdM` branch
and the merged pull requests. Each bill directory has its own README with the
compile recipe, the figure and table inventory, and the deliverable-to-appendix map.

| PR | Stage | Result |
|:--|:--|:--|
| 1 | Bootstrap + Process A | README, Master prompt, seven sub-prompts |
| 2 | Stage 1 research | `01-research/` |
| 3 | Stage 2 template selection | `02-template-selection/` (output-03 chosen) |
| 4 | Stage 3 Mermaid selection | `03-mermaid-selection/` (9 gray-scale diagrams) |
| 5 | Stage 4 figure selection | `04-figure-selection/` (9 figures + cover, 11 tables) |
| 6 | Stage 5 draft bill | `draft-bill/` (scaffold + zip) |
| 7 | Stage 6 full bill | `full-bill/` (rendered + 12 LaTeX deliverables + zip) |
| 8 | Stage 7 final bill | `final-bill/` (polished, v1.0.0 + zip) |
| 9 | Release (Rule 10) | `CHANGELOG.md`, `releases.md`, repository finalization |

## License

Released under CC BY 4.0; reproduced public-domain U.S. Government statutory text
is used under 17 U.S.C. § 105. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
