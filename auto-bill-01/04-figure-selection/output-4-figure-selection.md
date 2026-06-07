## output-4-figure-selection

# Figure and table plan for H. R. 9510 v4.0

*Independent research draft. Figures are gray-scale Mermaid (Markdown) reproduced
as gray-scale TikZ (LaTeX); tables are full-width, left-aligned, ragged-right. No
images (Rule 5).*

Stage 4 decides the correct visual type for every slot in the bill, drawing the
gray-scale Mermaid set from Stage 3 and the visual taxonomy from the
`papers/VVUQ-05/update-bill/figures-bill` catalog (the master `README.md` and the
five catalogs `01RootREADME.md`, `02VVUQ01.md`, `03VVUQ02.md`, `04VVUQ03.md`,
`05VVUQ04.md`). The rule of thumb, carried from the figures-bill prompt: a
**diagram** for a process, lineage, decision, or layering; a **table** for a
schedule, crosswalk, register, or matrix; a comprehensive **repository structure**
in place of file-name lists in prose.

## Figure inventory (gray-scale Mermaid -> TikZ)

| Fig. | Title | Type | Bill location | figures-bill catalog source it visualizes |
|:--|:--|:--|:--|:--|
| Cover | The v4.0 single-prompt build process | flowchart TB | `main.tex` cover | "Building process" diagrams (01 root) |
| 1 | Four-work evidence-to-law lineage | flowchart LR | SEC. 2 | "lineage" boxes (01 root; 04, 05) |
| 2 | Accelerated timeline vs conventional | paired flowchart TB | SEC. 2 | "Accelerated timeline" (01 root; 02) |
| 3 | Ten-gate decision rule and funnel | BPMN flowchart | SEC. 3 | gate funnel / decision surface (02, 03) |
| 4 | Statutory layering through Title 21 | clustered component | SEC. 3 | "How the amendment threads through Title 21" (05) |
| 5 | Comparative-print section order | component flowchart | SEC. 4 | section-order chain (05) |
| 6 | Pre-introduction path by actor | swimlane | App. C, echoed App. J | next-steps path (Stage 1) |
| 7 | Evidence to introduction handoff | sequence | App. L | prompt/handoff evolution (04, 05) |
| 8 | The verification gate as a system | C4 architecture | App. C | data-and-control-flow architecture (03) |
| 9 | Prompt and bill-version evolution | hybrid flowchart | App. K | "Building process within the work" (03, 04) |

Nine numbered figures plus the cover figure, each a different Mermaid type, so no
diagram pattern is overused (the figures-bill prompt's anti-repetition preference).

## Table inventory (full-width, ragged-right)

| Tbl. | Title | Bill location | figures-bill catalog source |
|:--|:--|:--|:--|
| 1 | The four works at a glance | SEC. 2 | "four works at a glance" (01 root) |
| 2 | Ten-gate threshold schedule (standards-bound) | SEC. 3 | standards_map / gate spec (03) |
| 3 | Ten conforming amendments crosswalk | SEC. 3 | conforming crosswalk (05) |
| 4 | Per-section comparative-print change map | SEC. 4 | retained/excluded tables (05) |
| 5 | One-page summary block table | App. A | section map (04) |
| 6 | Numbered legislative findings -> authority | App. D | findings (04) |
| 7 | PAYGO and cost line items; earmark | App. G | fiscal table (output-03 genre) |
| 8 | Stakeholder register and phases | App. I | engagement register (output-03 genre) |
| 9 | Amendatory instruction table | App. J | amendatory table (05; output-03 genre) |
| 10 | Currency and cross-reference verification matrix | App. K | currency matrix (05) |
| 11 | Research-influence matrix (emerging bills) | App. L | research-influence tables (05 instruct-bill) |

## Repository-structure visuals (preferred over file-name prose)

Per the figures-bill preference, the bill READMEs and the transparency material use
a comprehensive repository-structure tree (the `auto-bill-01/` tree and each bill's
file map) rather than naming files inline in paragraphs.

## Placement rules carried into the bill stages

1. Each operative section (SEC. 2-4) carries one to three figures and the tables
   above; the twelve deliverable appendices carry a figure only where a diagram
   genuinely aids the reader (App. A, C, G, I, J, K, L), so figures complement,
   never crowd, the text.
2. Every figure is centered on a white background inside a thin black frame, sized
   to its content, with a small italic caption (matching the prior `asciifig` look,
   now `mermaidfig`).
3. Every table is set to `\textwidth` with `>{\raggedright\arraybackslash}p{...}`
   columns, so it matches the body measure with no large interword gaps.
4. Figure and table numbering is continuous across the bill and each entry is
   reachable from the clickable table of contents through its section.
