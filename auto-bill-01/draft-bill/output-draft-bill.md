## output-draft-bill

# Narrative output: H. R. 9510 Bill v4.0 draft (scaffold)

This stage produced the draft scaffold for H. R. 9510 Bill v4.0 under
`auto-bill-01/draft-bill`, by running
[`../sub-prompts/prompt-5-draft-bill.md`](../sub-prompts/prompt-5-draft-bill.md)
(filed here verbatim as `prompt-draft-bill.md`).

## What was built

- **`usctitle.sty`** - the v4.0 style engine, adapted from the VVUQ-05 final-bill
  `usctitle.sty`. It keeps the United States Code reproduction commands and the
  congressional amendment apparatus, and replaces the ASCII figure primitive with a
  gray-scale **`mermaidfig`** environment that renders a TikZ diagram on a white
  background inside a thin black frame, centered and sized to its content. A
  `treelisting` verbatim box is retained for repository-structure trees only (file
  listings, not diagrams). New helpers were added for the deliverable genres:
  `\billbox` (boxed operative sentence), `\cboxx` (checkbox), and `\sigline`
  (signature line). The five-step gray palette `mmg1`..`mmg5` and the TikZ node
  styles `mmin`, `mmstep`, `mmdec`, `mmlaw`, `mmgoal`, `mmperson`, and `mmlane`
  reproduce the Stage 3 Mermaid roles in gray-scale only.
- **`references.bib`** - the provenance and research sources, carried from the
  final-bill so every `\cite` key in the operative sections resolves.
- **`main.tex`** - the caption page (condensed House and Senate statements, dated
  June 7, 2026), the cover note with the v4.0 DOI placeholder, a rendered cover
  figure (the single-prompt build process as a gray-scale Mermaid TikZ flowchart),
  SECTION 1 with a clickable, page-filling table of contents that lists the four
  operative sections and all twelve deliverable appendices, the sixteen `\input`
  lines, the Authorship, Notices, and Provenance block, and the references.
- **Fifteen section files** - `s2-findings`, `s3-amendment`, and `s4-comparative`
  (operative), plus `a-one-page-summary` through `l-testimony-influence` (the twelve
  deliverable appendices). In this scaffold each file carries its heading, a short
  framing sentence, and a bracketed `[DRAFTING INSTRUCTIONS]` block naming the exact
  upstream file to process and the gray-scale Mermaid figure and tables to render in
  the full bill.

## How the scaffold encodes the two main updates

1. **Twelve deliverables as LaTeX appendices in the table of contents (Rule 2).**
   SECTION 1(b) lists Appendix A through Appendix L, each linked; each appendix file
   exists and names its source deliverable `.md` and output-03 genre.
2. **Gray-scale Mermaid diagrams only (Rule 5).** The cover figure is a rendered
   gray-scale TikZ Mermaid diagram; every other figure slot names the gray-scale
   Mermaid type the full bill will render. No raster image is used.

## Quality checks

- All seventeen `.tex`/`.sty` files pass a brace-balance and environment-matching
  check.
- The document is structured for the Overleaf pdfLaTeX recipe
  (`pdflatex` -> `bibtex` -> `pdflatex` -> `pdflatex`).
- Single hyphens only; the section symbol § for codified references; white
  background throughout; `RaggedRight` body; maximal widow and orphan penalties.

## Next stage

The full bill (`auto-bill-01/full-bill`) executes every bracketed instruction:
rendering each gray-scale Mermaid figure as TikZ, filling every table, carrying the
full operative text, and writing all twelve deliverable appendices in full LaTeX.
