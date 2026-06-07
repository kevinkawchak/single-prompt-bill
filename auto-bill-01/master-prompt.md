## master-prompt

> This file preserves the single submitted Master prompt word-for-word, filed
> per Rule 14 ("File this submitted prompt and all AI outputs using the prior
> prompt's instructions as a template"). The prior template is the VVUQ-05
> `prompt-draft-bill.md` / `output-draft-bill.md` and `prompt-full-bill.md` /
> `output-full-bill.md` convention: a `## prompt-...` heading followed by the
> prompt verbatim, paired with a `## output-...` file that carries the narrative
> output. Each stage of this run follows the same convention under
> `auto-bill-01/sub-prompts/` (the generated sub-prompts) and the per-stage
> `output-*.md` files (the narrative outputs).

"PROCESS"
Utilize a single prompt to generate H. R. 9510 v4.0 fully autonomously. The two main updates a) consist of the 12 completed deliverables that you improve, update, and convert to LaTeX based on cancer-automated/tree/main/papers/VVUQ-05/final-bill/deliverables b) only use gray-scale  mermaid diagrams to complement the text. This will be accomplished by first A) generating all sub-prompts based on the prior v3.0 user prompt markdowns, and then B) at your later processing time point: running each prompt sequentially as the Bill continues to grow from draft-bill to full-bill to final-bill. You will have to adapt to a self-learning process based on prior user prompt markdowns, while ensuring each Bill creation stage is high quality throughout. Create an auto-commit / auto-PR process in real-time that allows for the user to monitor branch progress without any user intervention. This is an extensive process. A single last update by you provides changelog, versioning, and repositories.
"PROCESS"

Rules:
1. Only commit to the "kevinkawchak/single-prompt-bill" repository with a comprehensive README, with new files going into main/auto-bill-01. Subdirectories also have READMEs. Do not commit to other repositories.
2. Each of the 12 deliverables must be improved, updated, converted to LaTeX, and represented by a properly formatted table of contents in the Bill
3. Appendices, "Authorship, Notices, and Provenance", and References must be present, and correct. Follow the prior improvements from full-bill to final-bill regarding reference appearance regarding white space formatting, and no single words per line
4. Only Claude Code Opus 4.8 (1M Context) Max can be used throughout all of the Master prompt and sub-prompts. Do not stall, ask questions, or go into plan mode
5. No images are allowed, only gray scale Mermaid diagrams
6. Each README.md for each directory must be comprehensive and state which files from other directories were used and where. For instance: No. 03 Mermaid diagram - Clinical-AI-Demos/tree/main/ai-outputs/output-01
7. 1 commit must be used for each distinguishable task (each .tex, .md, etc.)
8. 1 PR must be used for each set of distinguishable tasks
9. All commits and PRs must be submitted to GitHub in real-time the moment they are generated for user viewing. Do not hold commits and PRs from GitHub as they are completed
10. There must be a single last v1.0.0 update that provides the CHANGELOG.md, releases.md, repository updates, (as inspired by cancer-automated/blob/main/papers/VVUQ-05/full-bill/prompt-full-bill.md)
11. You have permission to create the repository, commit, commit to main, merge, and create PRs in GitHub.
12. Do not make shortcuts from prompt to prompt: every stage must be fully developed following prior specified prompts. All files generated from prompts must be present and working. Each set of LaTeX files must compile properly in Overleaf
13. Don't stop until all tasks are completed. The user will continue the session by using the phrase "Continue." if tokens are exhausted. This is a lengthy process
14. File this submitted prompt and all AI outputs using the prior prompt's instructions as a template
15. Leave DOI in the format: 10.5281/zenodo.xxxxxxxx (with Hyperlink: https://doi.org/10.5281/zenodo.xxxxxxxx).
16. Learn and implement the author's /clearpage, table formatting column widths, and other types of /vspace and /hspace formatting methods. Learn from and implement the author's other corrections/proof reading techniques to create the polished final-bill source files. All draft-bill, full-bill, and final-bill developments must have their own .tex outputs and tex zip file that run properly in Overleaf.
17. You will be judged on how well you followed these rules and prompt schedule after you finish by the author and other people

"PROMPT SCHEDULE"
1. Automatic research (perform all necessary research) (1 PR, 1 commit)
cancer-automated/blob/main/papers/VVUQ-05/update-bill/next-steps/prompt-1-next-steps.md
2. Template bill selection (pick 1 appropriate template file set) (1 PR, 1 commit)
Clinical-AI-Demos/tree/main/ai-outputs/output-02 OR Clinical-AI-Demos/tree/main/ai-outputs/output-03
3. Mermaid selections (use different and most relevant mermaid diagrams throughout) (1 PR, 1 commit)
Clinical-AI-Demos/tree/main/ai-outputs/output-01
4. Figure selection (identify correct figure types with mermaid diagrams throughout) (1 PR, 1 commit)
cancer-automated/blob/main/papers/VVUQ-05/update-bill/figures-bill/prompt-figures-bill.md
5. Bill draft template (the new bill's first set of instructions need to be adapted from this prompt) (1 PR, 1 commit)
cancer-automated/blob/main/papers/VVUQ-05/draft-bill/prompt-draft-bill.md
6. Bill full version (the new bill's second set of instructions need to be adapted from this prompt) (1 PR, 1 commit)
cancer-automated/blob/main/papers/VVUQ-05/full-bill/prompt-full-bill.md
7. Bill final version (your Bill context and formatting quality should match and exceed the prior bill-version) (repository version v1.0.0) (1 PR, 1 commit)(learn from and implement corrections previously made by a human from  draft-bill to full-bill)
cancer-automated/tree/main/papers/VVUQ-05/final-bill
"PROMPT SCHEDULE"
