# sub-prompts - Process A output

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Prompts](https://img.shields.io/badge/Sub--prompts-7-blue.svg)](.)
[![Engine](https://img.shields.io/badge/Engine-Claude%20Code%20Opus%204.8%20(1M)%20Max-blue.svg)](.)

This folder is the output of **Process A**: from the single
[`../master-prompt.md`](../master-prompt.md), Claude Code generated all seven
sub-prompts that **Process B** then runs in sequence. Each sub-prompt is adapted
from the corresponding prior v3.0 prompt Markdown and re-targeted for the
single-prompt v4.0 build (the `kevinkawchak/single-prompt-bill` repository,
`auto-bill-01/`, gray-scale Mermaid diagrams only, and the twelve deliverables
converted to LaTeX inside the bill).

## The seven sub-prompts

| # | Sub-prompt | Runs in stage | Adapted from (prior v3.0 source) |
|:--|:--|:--|:--|
| 1 | [`prompt-1-research.md`](prompt-1-research.md) | `01-research/` | `VVUQ-05/update-bill/next-steps/prompt-1-next-steps.md` |
| 2 | [`prompt-2-template-selection.md`](prompt-2-template-selection.md) | `02-template-selection/` | `Clinical-AI-Demos/ai-outputs/output-02/prompt.md`; `output-02`/`output-03` |
| 3 | [`prompt-3-mermaid-selection.md`](prompt-3-mermaid-selection.md) | `03-mermaid-selection/` | `Clinical-AI-Demos/ai-outputs/output-01/ChatGPT.md` |
| 4 | [`prompt-4-figure-selection.md`](prompt-4-figure-selection.md) | `04-figure-selection/` | `VVUQ-05/update-bill/figures-bill/prompt-figures-bill.md` |
| 5 | [`prompt-5-draft-bill.md`](prompt-5-draft-bill.md) | `draft-bill/` | `VVUQ-05/draft-bill/prompt-draft-bill.md` |
| 6 | [`prompt-6-full-bill.md`](prompt-6-full-bill.md) | `full-bill/` | `VVUQ-05/full-bill/prompt-full-bill.md` |
| 7 | [`prompt-7-final-bill.md`](prompt-7-final-bill.md) | `final-bill/` | `VVUQ-05/final-bill` (+ human draft->full corrections) |

## Convention (Rule 14)

Every sub-prompt opens with a `## prompt-<name>` heading followed by the prompt
text, mirroring the prior repository's `prompt-draft-bill.md` /
`prompt-full-bill.md` convention. Each stage that runs a sub-prompt writes a paired
`output-*.md` narrative file, and the three bill stages additionally re-file their
own `prompt-*.md` verbatim inside their directory, exactly as the prior bills did.

## Self-learning note

The sub-prompts encode the lessons carried forward from the prior builds: the
white-space and reference-formatting corrections made from full-bill to final-bill,
the table column-width convention, the `\clearpage`/`\vspace`/`\hspace` page
balancing, the single-hyphen and section-symbol rules, and the move from ASCII
figures to gray-scale Mermaid (rendered as TikZ in LaTeX).

## License

Released under CC BY 4.0. Author: Kevin Kawchak, CEO ChemicalQDevice
([ORCID 0009-0007-5457-8667](https://orcid.org/0009-0007-5457-8667)).
