# Releases

DOIs are left as `10.5281/zenodo.xxxxxxxx`
([https://doi.org/10.5281/zenodo.xxxxxxxx](https://doi.org/10.5281/zenodo.xxxxxxxx))
pending deposit (Rule 15).

---

## v2.0.0 - The Single-Prompt Financial Data Amendment (H. R. 9510 Bill v5.0)

## Summary

H. R. 9510 Bill v5.0, the *Verification Before Generation in Physical AI
Oncology Trials Act of 2026* - **the Financial Data Amendment** - built end to
end from a single Master prompt in `auto-bill-02/`. The agent first generated
all seven of its own sub-prompts (Process A, updated from the v4.0 set), then
ran them in sequence (Process B) through four research stages and three bill
stages, building from the Bill v3.0 measure
(`cancer-automated/papers/VVUQ-05/final-bill`, without its deliverables). The
auto-commit/PR schedule was updated for the single permitted branch: one
commit per file pushed in real time, with the nine prior PRs mapped to nine
labeled stage milestones inside one continuously updated pull request. The two
headline updates over Bill v4.0: a **comprehensive financial-data focus** (the
section 515D(k) verification cost record; the SEC. 5 financial core with
transparency, user-fee treatment, an authorization of appropriations, and the
boxed Statutory PAYGO clause; a twelve-section comparative print adding
§ 379j; and four financial appendices), and **three visual media used
together** - fifteen full-width tables with right-aligned dollar columns, six
centered ASCII figures including the cover, and six gray-scale Mermaid
diagrams (real `mermaid` in Markdown, gray-scale TikZ in the compiled LaTeX) -
with no raster image anywhere.

## Features

- Single Master prompt to a complete, compiling financial bill, across nine
  real-time milestones (bootstrap, four research stages, three bill stages,
  and this release) in one continuously updated pull request.
- Three Overleaf-ready LaTeX bundles: `draft-bill-LaTeX.zip`,
  `full-bill-LaTeX.zip`, and `final-bill-LaTeX.zip`, each compiling with the
  pdfLaTeX recipe.
- The operative amendment carried (new section 515D / 21 U.S.C. 360e-5 and ten
  conforming amendments) plus the v5.0 financial operative core: the
  financial-data record 515D(k), the § 379j zero-fee treatment for a
  verification record filed alone, part 54 disclosure alignment, the
  58-million-dollar (illustrative) five-year authorization with summing
  fiscal-year tables, and the standard PAYGO budgetary-effects clause.
- The financial appendices: a CBO-genre cost estimate (budget authority versus
  outlays at a 60/30/10 spend-out; the statutory user-fee percentage table;
  scorecard and mandates summary), verification economics (4,420 dollars
  illustrative per cleared interaction class; the nineteen-fold program-year
  comparison), the financial-data transparency standard (completeness,
  traceability, periodicity, comparability), the financial research-influence
  matrix, and the development transparency record.
- The merged style `usctitle.sty` v5.x: the v3.0 ASCII primitives and table
  columns, the v4.0 gray-scale Mermaid TikZ primitives and boxed statement,
  and the new right-aligned `R{<width>}` numeric column for dollar series.

## Contributors

@kevinkawchak
@claude
@openai
@google-gemini

## Notes

Independent research draft. Not an enacted law, not pending legislation, and
not legal advice; not endorsed by the FDA, HHS, the CBO, the GAO, the OMB, the
OLRC, CFR, ICH, or any Member of Congress. The illustrative number
"H. R. 9510" is a placeholder; the Clerk assigns the real number only at
introduction. All dollar figures are illustrative or simulation results unless
tied to a cited statute or notice; no formal CBO estimate exists. Reproduced
statutory text is public domain (17 U.S.C. 105); generated content is released
under CC BY 4.0; repository code is under the MIT License.

---

## v1.0.0 - The Single-Prompt Gray-Scale Mermaid Amendment (H. R. 9510 Bill v4.0)

## Summary

H. R. 9510 Bill v4.0, the *Verification Before Generation in Physical AI Oncology
Trials Act of 2026*, built end to end from a single Master prompt by Claude Code
Opus 4.8 (1M context) Max. The agent first generated all seven of its own
sub-prompts (Process A), then ran them in sequence (Process B) to grow the bill from
a draft scaffold to a full bill to a polished final bill, committing and opening
pull requests in real time so branch progress could be monitored without any user
intervention. The two headline updates over Bill v3.0: the twelve submission
deliverables are improved, updated, and converted to LaTeX appendices inside the
bill (each in the clickable table of contents), and every diagram is a gray-scale
Mermaid figure (real `mermaid` in Markdown, gray-scale TikZ in the compiled LaTeX)
with no raster image anywhere.

## Features

- Single Master prompt to a complete, compiling bill, across nine real-time pull
  requests (bootstrap, four research stages, three bill stages, and this release).
- Three Overleaf-ready LaTeX bundles: `draft-bill-LaTeX.zip`, `full-bill-LaTeX.zip`,
  and `final-bill-LaTeX.zip`, each compiling with the pdfLaTeX recipe.
- The operative amendment (new section 515D / 21 U.S.C. 360e-5 and ten conforming
  amendments) with Figures 1 to 5 and Tables 1 to 4.
- Twelve LaTeX deliverable appendices (A to L) with Figures 6 to 9 and Tables 5 to
  11, each a genre-correct conversion of its source deliverable.
- Nine gray-scale Mermaid figure types plus a cover figure; eleven full-width,
  ragged-right tables; white background throughout; single hyphens only; the section
  symbol for codified references; maximal widow and orphan control.
- Appendices, an Authorship, Notices, and Provenance block, and References, all
  present and consistent (Rule 3).

## Contributors

@kevinkawchak
@claude
@openai
@google-gemini

## Notes

Independent research draft. Not an enacted law, not pending legislation, and not
legal advice; not endorsed by the FDA, HHS, the OLRC, CFR, ICH, or any Member of
Congress. The illustrative number "H. R. 9510" is a placeholder; the Clerk assigns
the real number only at introduction. Reproduced statutory text is public domain
(17 U.S.C. 105); generated content is released under CC BY 4.0; repository code is
under the MIT License.
