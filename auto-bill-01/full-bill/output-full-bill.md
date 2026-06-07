## output-full-bill

# Narrative output: H. R. 9510 Bill v4.0 full bill

This stage produced the full, rendered H. R. 9510 Bill v4.0 under
`auto-bill-01/full-bill`, by running
[`../sub-prompts/prompt-6-full-bill.md`](../sub-prompts/prompt-6-full-bill.md)
(filed here verbatim as `prompt-full-bill.md`) against the draft-bill scaffold.

## What was built

- **`main.tex`** - the finished assembler: caption (dated June 7, 2026), the cover
  note with the v4.0 DOI placeholder, a rendered gray-scale Mermaid cover figure,
  SECTION 1 with a clickable, page-filling table of contents listing the four
  operative sections and all twelve deliverable appendices, the fifteen `\input`
  lines, the Authorship, Notices, and Provenance block, and the references.
- **`usctitle.sty`** and **`references.bib`** - carried from the draft (the engine
  and the bibliography), so the full bill is self-contained (Rule 16).
- **The operative bill (SEC. 2 to SEC. 4)** - fully rendered:
  - SEC. 2 carries findings (a) to (g), Table 1 (the four works), and two
    gray-scale Mermaid figures: Figure 1 (four-work lineage) and Figure 2
    (accelerated timeline).
  - SEC. 3 carries the operative new section 515D (subsections (a) to (j)), the ten
    conforming amendments, the clerical amendment, the rule of construction, the
    effective date, Table 2 (ten-gate schedule), Table 3 (conforming crosswalk),
    and Figure 3 (gate decision rule) and Figure 4 (statutory layering).
  - SEC. 4 carries Table 4 (per-section change map), Figure 5 (the affected
    sections in order), and the comparative-print reproductions with the strike and
    insert markers.
- **The twelve deliverable appendices (A to L)** - each improved, updated, and
  converted to LaTeX from its source in
  `cancer-automated/.../VVUQ-05/final-bill/deliverables`, using the matching
  output-03 genre, and each listed in the table of contents (Rule 2). Appendices
  carry Tables 5 to 11 and Figures 6 to 9 where a gray-scale Mermaid diagram aids
  the reader (the pre-introduction path, the verification gate as a system, the
  prompt and bill-version evolution, and the evidence-to-introduction handoff).

## The figures and tables (all gray-scale, no images)

Nine numbered gray-scale Mermaid figures plus the cover figure, rendered in TikZ on
a white background inside a thin black frame, and eleven full-width, left-aligned,
ragged-right tables. No raster image appears anywhere (Rule 5).

## Quality checks

- All `.tex`/`.sty` files pass a brace-balance and environment-matching check.
- Single hyphens only; the section symbol § for codified references in tables;
  white background throughout; RaggedRight body; maximal widow and orphan penalties.
- Structured for the Overleaf pdfLaTeX recipe
  (`pdflatex` -> `bibtex` -> `pdflatex` -> `pdflatex`).

## Next stage

The final bill (`auto-bill-01/final-bill`) applies the senior-author polish learned
from the prior draft-to-full-to-final corrections: reference white-space formatting
with no stranded single words, page balancing with `\clearpage`, `\vspace`, and
`\hspace`, and a final consistency pass across every figure, table, and appendix.
That stage marks repository release v1.0.0.
