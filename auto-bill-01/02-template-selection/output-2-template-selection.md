## output-2-template-selection

# Template selection for H. R. 9510 v4.0 and its twelve LaTeX deliverables

*Independent research draft. Not legal advice. Diagrams are gray-scale Mermaid
only; no images.*

Stage 2 chooses one LaTeX template file set to base the v4.0 bill body and the
twelve LaTeX deliverable appendices on. The two candidates are
`Clinical-AI-Demos/tree/main/ai-outputs/output-02` and `.../output-03`.

## The two candidates

| | output-02 | output-03 |
|:--|:--|:--|
| Count | 30 single-column templates | 30 single-column templates |
| Per-type variation | One shared skeleton per type; templates vary by **title and color** only | **Each template is a distinct document genre** with its own cover, body structure, and devices |
| Legislative deliverables 01-12 | Built on one bill-caption skeleton | One bespoke genre each (one-pager labeled blocks, findings-of-fact, Ramseyer redline, fiscal note, testimony Q&A, ...) |
| Preview PDF | Yes (30-page cover preview) | No |
| Best for | Quick uniform reskins | Faithful, genre-correct conversion of each deliverable |

I unzipped and inspected `output-03/LaTeX-Source-Files-05` (the Ramseyer
comparative print). Its `tmpl05style.sty` is rebuilt directly from
`papers/VVUQ-05/final-bill/usctitle.sty` conventions (Times statute look,
white background, RaggedRight, `L`/`C`/`Y` ragged-right columns, `\cprstrike` and
`\cprinsert` redline markers, a `\billline` header, `\keywords`, `\bmhead` back
matter, and a font-independent `\cboxx` checkbox), confirming that output-03's
twelve legislative templates already carry the genre-specific devices each
deliverable needs.

## Decision: output-03 (the genre-diverse set)

**output-03 is selected.** Rule 2 requires each of the twelve deliverables to be
improved, updated, and converted to LaTeX, and represented in the bill's table of
contents. A genre-correct conversion (a fiscal note that looks like a fiscal note,
a Ramseyer print that shows strike and insert, testimony that reads as an opening
statement plus Q&A) is materially better than twelve reskins of one skeleton.
output-02's shared-skeleton approach is better suited to rapid uniform templating,
which is not this build's goal. The output-02 cover-preview PDF is moot here
because no images are permitted (Rule 5) and the deliverables live inside the bill
rather than as standalone cover-page documents.

**One adaptation for Rule 5:** output-03's templates ship a green ORCID logo image
(`orcid_icon.png`). In v4.0 that image is replaced everywhere by a **black text
ORCID hyperlink** (`\href{https://orcid.org/0009-0007-5457-8667}{ORCID
0009-0007-5457-8667}`), matching the final-bill `main.tex` and keeping the build
image-free.

## Deliverable-to-genre map (the twelve LaTeX appendices)

Each deliverable in `cancer-automated/.../VVUQ-05/final-bill/deliverables` is
converted using the matching output-03 genre and devices, and placed as a bill
appendix (Rule 2).

| # | Deliverable | output-03 genre | Appendix | Key LaTeX devices |
|:--|:--|:--|:--|:--|
| 01 | One-page summary | Executive one-pager (labeled blocks) | App. A | labeled blocks, body-width summary table |
| 02 | Section-by-section analysis | Per-section annotation/gloss | App. B | section/subsection glosses |
| 03 | Plain-English policy memo | Policy memorandum (TO/FROM/RE; Q&A) | App. C | memo header, Q&A |
| 04 | Legislative findings | Findings of fact (numbered) + authorities | App. D | numbered findings, authority cites |
| 05 | Ramseyer comparative print | Ramseyer redline (strike/insert) | App. E | `\cprstrike`, `\cprinsert` |
| 06 | Constitutional Authority Statement | Formal statement (boxed operative sentence) | App. F | boxed operative sentence |
| 07 | PAYGO and cost estimate | Fiscal note (budget table + earmark declaration) | App. G | fiscal table, earmark declaration |
| 08 | Sponsor and cosponsor packet | Recruitment packet (checklist + signature lines) | App. H | checklist (`\cboxx`), signature lines |
| 09 | Stakeholder engagement plan | Engagement plan (register + phases) | App. I | register table, phase list |
| 10 | Legislative Counsel routing memo | Routing memo (amendatory table + numbered questions) | App. J | amendatory table, numbered questions |
| 11 | Currency and cross-reference matrix | Audit matrix (verification table + sign-off) | App. K | verification matrix, sign-off |
| 12 | Testimony and research-influence brief | Hearing testimony (opening statement + Q&A + influences) | App. L | testimony blocks, influence table |

## How the choice flows into later stages

- The bill body (`main.tex`, `usctitle.sty`, `references.bib`, the four operative
  sections) is adapted from `papers/VVUQ-05/final-bill`, the common ancestor of
  output-03's style.
- The twelve deliverable appendix `.tex` files adopt output-03's genre devices, so
  each appendix is visually distinct yet shares the bill's white-background,
  RaggedRight, single-hyphen, section-symbol conventions.
- Every appendix carries one gray-scale Mermaid (TikZ) figure where a diagram aids
  the reader, per Stage 3 and Stage 4.
