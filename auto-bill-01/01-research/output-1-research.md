## output-1-research

# Next Steps Before H. R. 9510 Can Be Submitted to Congress (current for 2026)

*Independent research draft. Not legal advice; not endorsed by the FDA, HHS, the
OLRC, or any Member of Congress. Prepared June 7, 2026 for the 119th Congress, 2d
Session.*

This research underpins H. R. 9510 **Bill v4.0**, which descends from the four
works in `kevinkawchak/cancer-automated/tree/main/papers`: VVUQ-01 and VVUQ-02
(the method, pipeline, and hard engineering proof), VVUQ-03 (the standalone
*VVUQ Physical AI Oncology Trial Bill*), and VVUQ-04 (the same proposal recast as
an amendment to the **Federal Food, Drug, and Cosmetic Act**, adding new § 515D /
21 U.S.C. § 360e-5, the *Verification Before Generation in Physical AI Oncology
Trials Act of 2026*, current through Public Law 119-93). Bill v3.0 (VVUQ-05) added
the visual perspective and the twelve submission deliverables.

## Two reality checks that frame every step

1. **"H. R. 9510" is illustrative, not assigned.** A bill receives no number until
   it is introduced; the Clerk assigns the number at the moment of introduction.
   The styled number is a placeholder throughout this project.
2. **A private project cannot submit a bill to Congress directly.** Only a sitting
   Member of the House may introduce a House bill. (Agencies can transmit draft
   bills by an executive-communication letter, but that route is not open to an
   outside research project.) Every step below therefore has one real goal: get the
   text into final form and into the hands of a Member who will introduce it.

## Phase 1 - Settle on one authoritative text

- **Pick the vehicle.** The FD&C Act amendment form (VVUQ-04, carried into v3.0 and
  v4.0) is the more introduction-ready vehicle: it edits existing law with specific
  amendatory instructions ("Section 515D ... is amended by ...") and conforming
  amendments, which is how device legislation is actually written and referred. The
  standalone VVUQ-03 bill is best used as explanatory and findings backbone. Decide
  which is the bill and which is supporting material; do not introduce both.
- **Freeze and version the text.** Choose the final bill text, lock it, and stop
  editing the introduced version after this point. (In this project that frozen text
  is the `final-bill`.)
- **Human subject-matter and legal review.** Qualified counsel and oncology and
  regulatory experts must review the substance; this is the human-reviewer gate the
  repository itself requires.
- **Currency check.** Re-verify, immediately before introduction, that no newer
  public law has changed Title 21, that the target section number (§ 360e-5 /
  § 515D) is still unused, and that every cross-reference and each of the ten
  conforming amendments still lands correctly. (Deliverable 11 performs this.)

## Phase 2 - Secure a sponsor and build support

- **Find a sponsoring Representative.** The natural committee of jurisdiction is the
  House Committee on **Energy and Commerce** (which holds FDA and FD&C Act
  jurisdiction), with a plausible secondary interest from the Committee on Science,
  Space, and Technology given the AI and autonomy dimension.
- **Prepare the pitch package** the Member's staff expects: a one-page summary, a
  section-by-section analysis, a plain-English problem-and-solution memo, the
  legislative findings, and a Ramseyer comparative print showing changes to existing
  law. (Deliverables 01-05 supply these.)
- **Line up original cosponsors.** Bipartisan support meaningfully improves a bill's
  prospects. (Deliverable 08 is the recruitment packet.)
- **Stakeholder engagement.** Brief FDA and HHS, patient-advocacy groups, industry,
  academic societies, and the standards bodies the bill leans on (ASME V&V 40,
  IEC 80601-2-77, ISO 13482, ISO/TS 15066, ISO 14971, NASA-STD-7009A, IEEE Std
  7009-2024). Keep all outreach consistent with the repository's respectful,
  not-endorsed-by framing. (Deliverable 09 is the engagement plan.)

## Phase 3 - Professional drafting and the 2026 pre-introduction requirements

- **House Office of the Legislative Counsel (HOLC).** The sponsoring office should
  route the text through HOLC (legcounsel.house.gov) to put it in proper legislative
  form. It is not required by rule but is standard, nonpartisan, and confidential,
  and several drafts may be needed before a measure is ready. (Deliverable 10 is the
  routing memo.)
- **Constitutional Authority Statement (CAS).** Required by House Rule XII, clause
  7(c) for every introduced bill. For an FD&C Act amendment the citation is the
  Commerce Clause (Article I, § 8, clause 3), on which the FD&C Act rests.
  (Deliverable 06.)
- **Sponsor signature and cosponsor form** on the Clerk's form.
- **PAYGO and cost statements.** Prepare a Statutory PAYGO statement if the bill has
  budgetary effects and an earmark declaration (here, negative). Informal CBO
  consultation can be sought; formal scoring typically follows introduction.
  (Deliverable 07.)
- **Anticipate committee referral.** Expect primary referral to Energy and Commerce
  (Subcommittee on Health), with possible secondary referral. Drafting to a single,
  coherent subject helps; note there is no federal single-subject rule (the "One
  Subject at a Time Act" remains only a proposal), so this is good practice, not a
  requirement.

## Phase 4 - The actual submission (introduction)

- The Member or staff submits the signed PDF (bill text, CAS, and cosponsor form)
  via the **eHopper**, now the House's primary way of introducing bills (the physical
  hopper on the floor remains available). Submissions are accepted from roughly 15
  minutes before the House convenes through roughly 15 minutes after it adjourns.
- The Clerk assigns the real H.R. number, the Speaker (with the Parliamentarian)
  refers it to committee, and the Government Publishing Office prints it in
  introduced form.

## 2026-specific timing and cautions

- **Calendar window.** The 119th Congress, 2d Session, is calendar year 2026, and
  the Congress ends January 3, 2027. A bill not enacted by then dies and must be
  reintroduced in the 120th Congress, so the realistic target is introduction well
  inside 2026.
- **AI-authored origin.** No House rule requires disclosing that text was AI-drafted,
  but because these drafts were generated autonomously, be transparent with the
  sponsoring office and ensure a named human attorney or expert takes ownership of
  the final text before introduction.
- **Keep the disclaimers true.** Until a Member introduces it, the document remains
  an independent research draft: not pending legislation, not endorsed by the FDA or
  any Member, and not legal advice.

## How this research drives the twelve deliverables (v4.0)

| Phase | Step | Deliverable (LaTeX appendix in v4.0) |
|:--|:--|:--|
| 1 | Consolidate, freeze, summarize | 01 One-page summary; 02 Section-by-section; 03 Policy memo |
| 1 | Findings; show changes to law | 04 Legislative findings; 05 Ramseyer comparative print |
| 1 | Currency check before introduction | 11 Currency and cross-reference matrix |
| 2 | Recruit sponsor and cosponsors | 08 Sponsor and cosponsor packet |
| 2 | Brief agencies and standards bodies | 09 Stakeholder engagement plan |
| 3 | Proper legislative form | 10 Legislative Counsel routing memo |
| 3 | Constitutional basis | 06 Constitutional Authority Statement |
| 3 | Budget and earmark posture | 07 PAYGO and cost estimate |
| 2-4 | Hearing record; emerging-bill influences | 12 Testimony and research-influence brief |

## In one line

Consolidate the drafts into one human-reviewed, currency-checked FD&C Act amendment
-> recruit a House sponsor and cosponsors -> run it through the Office of the
Legislative Counsel -> attach the Constitutional Authority Statement and required
forms -> introduce it via the eHopper, where the Clerk assigns the real number and
refers it to Energy and Commerce.

## Sources

- Introduction and Referral of Bills - House.gov
- How Our Laws Are Made - Congress.gov
- Introducing a House Bill or Resolution - CRS R44001
- Sponsorship and Cosponsorship of House Bills - CRS RS22477
- Office of the Legislative Counsel of the U.S. House - Understanding the Legislative Process
- Constitutional Authority Statements: A Quick Guide - CRS IF12335
- Constitutional Authority Statement - House Rules Committee
- eHopper Quick Guide - Office of the Clerk (House.gov)
- House Rules for the 119th Congress - H. Res. 5
- FDA-Related Congressional Committees: Jurisdiction - FDLI
- House Committee on Energy and Commerce
- Federal Food, Drug, and Cosmetic Act, Title 21 U.S.C. (current through Pub. L. 119-93)
