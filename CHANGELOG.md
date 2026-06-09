# Changelog

All notable changes to this repository are documented here. The format follows
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres
to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). DOIs are left as
`10.5281/zenodo.xxxxxxxx` pending deposit (Rule 15).

## [2.0.0] - 2026-06-09

The second release: the autonomous, single-prompt build of **H. R. 9510 Bill
v5.0**, the *Verification Before Generation in Physical AI Oncology Trials Act
of 2026* - **the Financial Data Amendment** - generated end to end from one
Master prompt in `auto-bill-02/`, built from the Bill v3.0 measure
(`cancer-automated/papers/VVUQ-05/final-bill`, no `/deliverables`) and adapting
the `auto-bill-01` process (updated sub-prompts and auto-commit/PR schedule; no
shortcuts).

### Added
- **`auto-bill-02/` scaffold and Master prompt.** Comprehensive build
  `README.md` and the submitted Master prompt filed verbatim with the derived
  v5.0 rules and milestone schedule (`auto-bill-02/master-prompt.md`).
- **Process A: seven updated sub-prompts.** `auto-bill-02/sub-prompts/` -
  each adapted from the v4.0 sub-prompt and its VVUQ-05 ancestor, re-targeted
  to the financial-data focus and the three media (tables, ASCII, gray-scale
  Mermaid).
- **Stage 1: financial research.** `auto-bill-02/01-research/` - the scoring
  framework (CBO, Statutory PAYGO, House CutGo, earmark rules), the budget
  vocabulary, the FDA funding structure (MDUFA V, §§ 379i-379j), part 54 and
  Open Payments, UMRA, and the financial-data quality instruments, current for
  the 119th Congress, 2d Session.
- **Stage 2: template selection.** `auto-bill-02/02-template-selection/` -
  the Bill v3.0 file set selected as base; the v4.0 Mermaid TikZ primitives
  and `\billbox` merged in; the new right-aligned `R{<width>}` dollar column.
- **Stage 3: Mermaid + ASCII selection.** `auto-bill-02/03-mermaid-selection/`
  - six gray-scale Mermaid diagrams (no family repeated) and six ASCII forms,
  every one re-themed to the financial-data subject.
- **Stage 4: figure selection.** `auto-bill-02/04-figure-selection/` - the
  three-media plan: eleven figures plus the cover (six ASCII, six Mermaid)
  and fifteen full-width tables of financial data.
- **Stage 5: draft bill.** `auto-bill-02/draft-bill/` - the compiling
  scaffold with bracketed drafting instructions and an Overleaf zip.
- **Stage 6: full bill.** `auto-bill-02/full-bill/` - every slot rendered:
  new section 515D carried with the new **financial-data record (k)**; the
  comparative print widened to **twelve sections** (adding § 379j); the new
  **SEC. 5 financial core** (transparency, user-fee treatment, authorization
  of appropriations, the boxed Statutory PAYGO clause); five financial
  appendices; plus an Overleaf zip.
- **Stage 7: final bill (this release).** `auto-bill-02/final-bill/` - the
  polished bill: fresh-page balancing for SEC. 3-5, the appendices divider,
  caption consistency, re-verified dollar series, plus an Overleaf zip.
- **Release documentation.** This `CHANGELOG.md` entry and the `releases.md`
  v2.0.0 entry (Rule 10).

### Changed
- The bill focus moved from the v4.0 deliverables conversion to a
  **comprehensive financial-data focus**, and the diagram rule widened from
  gray-scale Mermaid only to **three media together**: full-width tables
  (right-aligned dollar columns), centered white-background ASCII figures,
  and gray-scale Mermaid (real `mermaid` in Markdown, TikZ in LaTeX). No
  raster images anywhere.
- The auto-commit/PR schedule was updated for the single permitted branch:
  the prior nine PRs map to **nine labeled stage milestones inside one
  continuously updated pull request**, one commit per file, pushed in real
  time.
- The root `README.md` now covers both builds (`auto-bill-01` v4.0 and
  `auto-bill-02` v5.0).

### Notes
- Independent research draft. Not an enacted law, not pending legislation, and
  not legal advice; not endorsed by the FDA, HHS, the CBO, the GAO, the OMB,
  or any Member of Congress. All dollar figures are illustrative unless tied
  to a cited statute or notice; no formal CBO estimate exists.
- Reproduced statutory text is public domain (17 U.S.C. 105); generated
  content is CC BY 4.0; repository code is MIT.

## [1.0.0] - 2026-06-07

The first tagged release: the autonomous, single-prompt build of **H. R. 9510 Bill
v4.0**, the *Verification Before Generation in Physical AI Oncology Trials Act of
2026*, generated end to end by Claude Code Opus 4.8 (1M context) Max from one Master
prompt, with real-time commits and pull requests.

### Added
- **Repository scaffold and Master prompt.** Comprehensive top-level `README.md`,
  `auto-bill-01/README.md`, and the submitted Master prompt filed verbatim
  (`auto-bill-01/master-prompt.md`).
- **Process A: seven sub-prompts.** `auto-bill-01/sub-prompts/` with `prompt-1`
  through `prompt-7`, each adapted from the prior v3.0 prompt Markdown, plus an index
  README.
- **Stage 1: automatic research.** `auto-bill-01/01-research/` - the four-phase
  pre-introduction path, current for the 119th Congress, 2d Session (2026).
- **Stage 2: template selection.** `auto-bill-01/02-template-selection/` - chooses
  the `output-03` genre-diverse template set and maps each deliverable to a genre.
- **Stage 3: gray-scale Mermaid selection.** `auto-bill-01/03-mermaid-selection/` -
  nine gray-scale Mermaid diagrams of distinct types, re-themed to the bill.
- **Stage 4: figure selection.** `auto-bill-01/04-figure-selection/` - the figure
  and table plan (nine figures + cover, eleven tables).
- **Stage 5: draft bill.** `auto-bill-01/draft-bill/` - the scaffold with bracketed
  drafting instructions and an Overleaf zip.
- **Stage 6: full bill.** `auto-bill-01/full-bill/` - the fully rendered bill with
  all gray-scale Mermaid figures as TikZ and all twelve deliverables as LaTeX
  appendices, plus an Overleaf zip.
- **Stage 7: final bill (this release).** `auto-bill-01/final-bill/` - the polished
  bill, page-balanced with a clean appendices divider and reference white-space
  formatting, plus an Overleaf zip.
- **The twelve deliverables converted to LaTeX** (Appendix A through Appendix L),
  each represented in the bill's clickable table of contents (Rule 2).
- **Release documentation.** This `CHANGELOG.md` and `releases.md` (Rule 10).

### Changed
- The diagram medium moved from the prior bills' ASCII figures to **gray-scale
  Mermaid** diagrams: real `mermaid` blocks in the Markdown and matching gray-scale
  TikZ figures in the compiled LaTeX (Rule 5). No raster images anywhere.
- @kevinkawchak uodated Bill DOIs for main/README.md, single-prompt-bill/blob/main/auto-bill-01/README.md, and single-prompt-bill/blob/main/auto-bill-01/final-bill/README.md on 2026-06-07.

### Notes
- Independent research draft. Not an enacted law, not pending legislation, and not
  legal advice; not endorsed by the FDA, HHS, or any Member of Congress.
- Reproduced statutory text is public domain (17 U.S.C. 105); generated content is
  CC BY 4.0; repository code is MIT.

[2.0.0]: https://github.com/kevinkawchak/single-prompt-bill/releases/tag/v2.0.0
[1.0.0]: https://github.com/kevinkawchak/single-prompt-bill/releases/tag/v1.0.0
