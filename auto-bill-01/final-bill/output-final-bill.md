## output-final-bill

# Narrative output: H. R. 9510 Bill v4.0 final bill (polished; repository v1.0.0)

This stage produced the polished, final H. R. 9510 Bill v4.0 under
`auto-bill-01/final-bill`, by running
[`../sub-prompts/prompt-7-final-bill.md`](../sub-prompts/prompt-7-final-bill.md)
(filed here verbatim as `prompt-final-bill.md`) against the full bill, and applying
the senior-author corrections learned across the prior draft-to-full-to-final
cycle.

## What changed from the full bill (the polish)

- **Page balancing.** SEC. 3 and SEC. 4 now begin on fresh pages, and a clean
  `\clearpage` divider opens the appendices, so each major part is self-standing.
- **An appendices divider.** A centered cross-head, "APPENDICES: THE TWELVE
  SUBMISSION DELIVERABLES," with a one-line framing, presents the twelve LaTeX
  deliverables as a package, each in the clickable table of contents (Rule 2).
- **Reference white-space formatting.** The bibliography is set `RaggedRight` inside
  its own group with URL-on-any-character breaking and a tightened lead space, so no
  reference line is left with a single stranded word and no link runs off the margin
  (Rule 3).
- **Consistency pass.** Figures 1 to 9 and Tables 1 to 11 are uniquely numbered
  across the whole bill; the one table-numbering collision found in the full bill
  (Appendix F) was resolved by making that supporting table unnumbered; single
  hyphens only; the section symbol § appears only in tables; white background
  throughout; maximal widow and orphan penalties.

## What it contains

The same complete bill as the full version: the caption and cover figure, SECTION 1
with the clickable page-filling table of contents, the operative SEC. 2 to SEC. 4
(findings, the new section 515D and ten conforming amendments, and the comparative
print) with Figures 1 to 5 and Tables 1 to 4, and the twelve deliverable appendices
A to L with Tables 5 to 11 and Figures 6 to 9, followed by the Authorship, Notices,
and Provenance block and the references. Every diagram is a gray-scale Mermaid
figure rendered in TikZ; there are no images (Rule 5).

## Quality checks

- All 17 `.tex`/`.sty` files pass a brace-balance and environment-matching check.
- Structured for the Overleaf pdfLaTeX recipe
  (`pdflatex` -> `bibtex` -> `pdflatex` -> `pdflatex`).
- `final-bill-LaTeX.zip` is the Overleaf-ready bundle.

## Release

This stage marks **repository release v1.0.0**. The single last update that follows
adds `CHANGELOG.md` and `releases.md` at the repository root and finalizes the
repository documentation (Rule 10).
