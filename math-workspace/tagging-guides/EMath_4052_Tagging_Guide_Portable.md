# E-Math 4052 — Portable Question Bank Tagging Guide

**Portable export: 11 November 2026. Source guide last updated: 21 October 2026.**

This file is self-contained for transfer to another chat: it includes the tagging rules, approval history, source-quality notes and the full 130-SIO reference last verified against the user's uploaded website on 5–6 October 2026. Upload it with the actual question papers. A newer user-supplied website/TOS export or explicit correction takes precedence; check for changes before tagging. The date of this export does not imply a new audit of the website.

## Start here: use this file in a new chat or account

Attach or paste **this full Markdown guide**, then attach the **question paper PDF** in the same chat. Add the marking scheme if available. This guide contains the E-Math 4052 tagging rules, the 130-SIO codebook in section 20, and a complete, copyable DMN Workspace JSON example in section 12. No separate JSON template or earlier chat is needed. These codes are for **E-Math 4052** only.

**Copy-paste prompt**

> Read this E-Math 4052 guide in full and tag the attached exam paper. Preserve its printed question and part labels, use the exact EM codes and the Paper 2 PRWC rule, and reconcile the marks. Return a downloadable DMN Workspace .json file using the example in section 12. Leave every part unreviewed and list uncertainties separately by question and part.

**Source precedence:** Apply explicit teacher corrections to the stated paper/part or rule. For code IDs, wording and chapter assignments, use the newest explicitly supplied authoritative E-Math taxonomy; otherwise use section 20. Older tables and historical package examples do not override it. Do not reassign or invent IDs to fill a gap. If a rule conflicts with the current reference, flag the conflict for review.

**Default deliverable for DMN Workspace:** When a paper accompanies this guide, return one downloadable import JSON per paper and a short list of uncertainties or source issues. If the teacher asks for review only, provide the review table instead. State any missing pages, marks or required metadata. Tags remain provisional until the teacher checks them. Do not claim any paper has been imported or published.

### Tested topics and untested SIO codes

- For a **topics tested** table, group by the primary SIO's strand and chapter. Show the relevant paper/question parts, number of tasks and marks. Allocate each part's marks once; supporting tags may be listed separately and do not add marks to the total.
- For **untested SIOs**, define the scope first: one paper, a named batch, or another set specified by the teacher. Use the active SIO codebook, never a numeric range such as EM-16 through EM-174. The original numbering has deliberate gaps and decimal IDs.
- Default to **untested as a primary skill**: subtract the set of distinct primary IDs used by the papers in scope from the active codebook. List the remaining exact codes with the recorded description, strand and chapter. Flag any of these that appear only as supporting skills. If asked for **bank coverage** or **untested even as a supporting skill**, subtract the union of primary and supporting IDs instead. State which definition you used.
- Keep each code distinct, including existing duplicate descriptions. An SIO attached only as an alternative in a review note is not an assigned tag. Label coverage based on proposed tags as provisional.

### Core rules for the next chat

1. Read this entire guide before tagging. Use the full SIO reference in section 20; do not guess an ID from memory.
2. Read the supplied question papers visually, including mathematical expressions, diagrams, tables and printed marks. Preserve school, year, paper, question and original part labels.
3. Give every marked part/task one primary SIO, optional useful supporting SIOs, AO, difficulty, printed marks and a short reason. Show the SIO description with its ID so the teacher does not need to look up a code.
4. Every Paper 2 final question is **PRWC**, across all its parts. Choose the appropriate existing PRWC SIO, with technical skills supporting where appropriate.
5. Retain the current numbering: **EM-53.5**, **EM-67.5**, **EM-109.5** are approved additions; **EM-172** remains single-event probability. Do not apply the superseded row-renumbering proposal.
6. Reconcile all printed parts and marks against the actual paper total. Do not assume every future paper totals 90 marks because previous batches did.
7. Flag uncertain tags and source defects. Distinguish **user-confirmed**, **proposed for teacher review**, and **source-verified** findings. A previous paper's approval does not approve a new paper automatically.
8. Update this MD after each batch and each teacher correction. Keep tag approval, answer validation, import and publishing separate.

Older companion files named in historical sections are optional examples if actually supplied. Do not claim to have inspected an unavailable file. The taxonomy embedded below is sufficient to identify the recorded SIOs; the actual question paper is still required to assess the demand.

## 1. Source of truth for SIOs

Use the **4Exp5NA Math 4052 (2023) TOS taxonomy** with the current user-uploaded website additions. The recorded effective taxonomy has **130 E-Math SIOs**; section 20 embeds the full codebook, and section 17 records the confirmed corrections. Preserve the original TOS numbering.

- Preserve the **exact SIO wording**, including mathematical expressions and examples.
- Do not shorten an SIO in a way that changes the skill being assessed.
- The mathematical examples in the TOS are part of the scope of the SIO.
- Use the three user-approved local extensions with their current website IDs:
  - **EM-53.5 — Algebraic expressions and formulae → completing the square**
  - **EM-67.5 — Functions and graphs → graphical methods to solve equations**
  - **EM-109.5 — Congruence and Similarity → areas of triangles with common height**

## 2. One primary SIO per question part

Every question part should have **one primary SIO**.

Choose the primary SIO by asking:

> What is the main mathematical skill the examiner is trying to assess in this part?

Do **not** tag every operation used in the solution.

A prerequisite or supporting skill may be recorded as `secondary_sio`, but only when it is genuinely useful for diagnosis or practice matching.

Practice matching should use the **primary SIO first**.

### Examples of this rule

- If a question is mainly a volume problem but trigonometry is needed to find a height:
  - Primary: volume / mensuration
  - Secondary: trigonometry

- If a probability question uses a cumulative-frequency graph to obtain a value:
  - Primary: probability
  - Secondary: cumulative-frequency interpretation

- If a coordinate-geometry problem requires forming an equation:
  - Primary should reflect the main assessed coordinate-geometry demand if that is the central purpose.
  - Equation formulation may be secondary.

## 3. Prefer the most precise official SIO

Do not choose a broad topic if a more precise SIO exists.

Examples:
- “solving quadratic equations by completing the square” is preferable to a generic “quadratic graphs” tag when the task is explicitly solving an equation.
- “angle sum of interior and exterior angles of any convex polygon” is preferable to a broad polygon-properties tag when polygon angle sums are the actual demand.
- “determining whether two triangles are congruent/similar” should be used when establishing similarity/congruence is the main task, rather than tagging only the properties later used.

## 4. Supporting skills do not replace the main assessed skill

A calculation may contain several mathematical techniques. Tag according to the **assessment intention**, not simply the last calculation performed.

Examples already agreed:
- 2024 P1 Q11(b): **Probability** is primary; cumulative-frequency interpretation is supporting.
- 2024 P1 Q27(c): **areas of triangles with common height** is the primary local SIO.
- 2025 P2 Q6(b): **volume/mensuration** is primary; 3D trigonometry is supporting.

## 5. Do not force an uncertain SIO

If two SIOs are genuinely plausible:
- choose the best primary SIO,
- add a secondary SIO if useful,
- mark confidence as Medium/Low for review.

Do not invent a new SIO unless the user explicitly approves it.

The user-approved local extensions are **EM-53.5**, **EM-67.5** and **EM-109.5**, as described in sections 1 and 17. Do not invent further extensions or renumber the original TOS rows.

## 6. Strand and main topic

Derive these from the selected primary SIO.

Use:
- `N&A` = Number & Algebra
- `G&M` = Geometry & Measurement
- `S&P` = Statistics & Probability

The `main_topic` should come from the TOS topic containing the primary SIO.

## 7. Difficulty

Use:
- **Foundation** — direct, straightforward application of one skill
- **Standard** — some interpretation, selection, or combination is required
- **Challenge** — non-routine, multi-step, or substantial reasoning/connection of skills

Do not use marks alone as the difficulty measure.

## 8. AO calibration used in this project

AO depends on the **actual demand of the question**, not the SIO alone.

### AO1
Routine application of a taught method/formula or direct reading/use of information.

Project-specific conventions:
- Direct use of a taught formula is AO1, even in a real-world context.
- Forming a standard direct-proportion equation is AO1.
- A standard construction explicitly requested is AO1.

### AO2
Selection/combination of techniques, interpretation, inference from diagrams, formulation, or non-routine application.

Project-specific conventions:
- Laws of indices involving multiple laws/steps are AO2.
- Questions requiring students to infer mathematical information from a diagram can be AO2.
- “Show that” questions involving analysis of a diagram and mathematical justification can be AO2.
- Interpreting loci/regions from construction conditions can be AO2.

### AO3
Worded mathematical reasoning, explanation, justification, interpretation of meaning, or argument.

Do not classify by a command word alone. A routine geometric proof or “show that” task involving selection and diagram analysis may be AO2 under the agreed calibration. Use AO3 for the assessed explanation, critique, interpretation or argument; flag the choice when AO2/AO3 is genuinely ambiguous.

Project-specific conventions:
- Non-simple statistical interpretation requiring reasoning with mean/median/mode can be AO3.
- Shape classification from a complex diagram can be AO3 when students must reason from properties.
- In general, questions requiring a written mathematical justification, explanation, comparison, or meaning in context are AO3.

## 9. Practice-next matching philosophy

For the reflection app:
1. Exact same **primary SIO** is preferred.
2. Same SIO as a secondary skill may be used as a fallback.
3. Closely related SIO families may fill missing practice slots when pedagogically appropriate.
4. Prefer a progression:
   - Foundation
   - Standard
   - Challenge
5. Exclude the paper the student is currently reflecting on.
6. Prefer different years when equivalent options exist.

Curated related families currently include:
- prime factorisation ↔ applications of prime factorisation
- Pythagoras ↔ basic right-angled trigonometry
- misleading statistical diagrams ↔ statistical inference/interpretation
- polygon angle sums ↔ regular-polygon / shape properties

## 10. Recommended workflow in a new chat

When tagging a new paper:
1. Read the actual question/diagram.
2. Check the exact TOS taxonomy.
3. Compare with user-confirmed examples in this guide and any existing tagged dataset actually supplied; treat provisional examples as review candidates.
4. Assign primary SIO.
5. Add secondary SIO only if useful.
6. Assign AO using the calibrated project rules above.
7. Assign Foundation / Standard / Challenge.
8. Flag genuinely ambiguous cases instead of silently forcing a tag.


## 11. Paper 2 final-question PRWC rule (user-confirmed, 5 October 2026)

- Treat the last question of every Paper 2 in this project as a **PRWC (Problems in Real-World Contexts)** question.
- Record the PRWC classification for the whole question and retain it across all its parts.
- Select the most appropriate existing PRWC SIO for each part; do not assign an unrelated topical primary SIO merely because the solution uses routine arithmetic, percentages, equations or mensuration.
- Number & Algebra PRWC SIOs in the current website are:
  - `EM-86`: solving problems based on real-world contexts (everyday life and personal/household finance; preserve the full existing wording).
  - `EM-87`: interpreting and analysing data from tables and graphs, including distance–time and speed–time graphs.
  - `EM-88`: interpreting the solution in the context of the problem.
- Geometry PRWC uses the relevant existing Geometry PRWC IDs (`EM-146`, `EM-147`, or the existing duplicate `EM-151` where already used). Do not create or silently merge SIOs.
- Keep an existing PRWC SIO primary and add a useful mathematical technique as secondary when needed.
- PRWC does not determine AO or difficulty: direct table calculations may be AO1/Foundation, whereas a justified recommendation may be AO3/Challenge.
- For the DMN 2026 pilot, Paper 2 Q10 is PRWC. Its provisional part tags are Q10(a)(i)/(a)(ii) → `EM-87`, Q10(b) → `EM-86`, Q10(c) → `EM-88`.

## 12. Current workspace and import-package mapping

Historical pilot note: 128 E-Math records were initially extracted from the earlier uploaded website. The later user-uploaded website has 130 records, including the approved additions, with original numbering retained. Use sections 17 and 20 for the current recorded reference. Earlier companion files were not supplied separately during that pilot; do not claim to have checked unavailable files.

- Package format: `dmn-math-package-v1`.
- Use `role: "bank"` for a practice source or `role: "reflection"` for a student reflection paper. Use the metadata in the workspace prompt when supplied. It takes precedence over illustrative or historical metadata in this guide.
- Part fields: `label`, `maxMarks`, `sioId`, `secondarySioIds`, `ao`, `difficulty`, `reviewed`.
- Question fields include `qno`, `images`, `parts`, `matchSioId`, `source`, `answerText`, `answerImages`.
- `sioId` is the primary part SIO; preserve all exact official wording in review displays rather than rewriting the taxonomy label.
- `matchSioId` is a separate whole-question practice anchor and must equal a primary SIO actually present in that question. A question with several skills retains the individual part tags.
- Embedded question images make a prepared package portable. Preserve stems, tables, diagrams, grids and continuation text; keep horizontal source scale consistent and remove blank working space when it serves no question purpose.
- The importer appends questions to the currently open paper and creates new IDs. It does not update matching existing questions and does not create a paper from the package metadata.
- Create fresh draft pilot papers for tests. Set their title, subject, paper number, bank role and total marks before import. Avoid importing the same package twice.
- Imported parts start unreviewed. Review the crops, marks, SIOs, AOs, difficulty and answers before publishing.
- Website bank coverage includes primary and supporting tags, but the current automatic practice matcher accepts primary matches only. The broader fallback philosophy in section 9 is an intended curation policy, not a claim about the current code.

### Complete DMN Workspace JSON example

This is a valid one-question, five-mark example. Replace every example value with the actual paper's metadata, printed labels, marks and tags. Do not copy the example tags to unrelated questions.

```json
{
  "format": "dmn-math-package-v1",
  "paper": {
    "title": "Example E-Math Paper 1",
    "subject": "emath",
    "year": 2026,
    "number": 1,
    "category": "school",
    "role": "reflection",
    "totalMarks": 5
  },
  "questions": [
    {
      "qno": "1",
      "images": [],
      "parts": [
        {"label": "a", "maxMarks": 2, "sioId": "EM-16", "secondarySioIds": [], "ao": "AO1", "difficulty": "Low", "reviewed": false},
        {"label": "b", "maxMarks": 3, "sioId": "EM-17", "secondarySioIds": ["EM-16"], "ao": "AO2", "difficulty": "Moderate", "reviewed": false}
      ],
      "matchSioId": "EM-17",
      "answerText": "",
      "answerImages": []
    }
  ]
}
```

- Use the exact keys above. Question and part labels are strings; marks are numeric. Include each printed mark-bearing part once. Report discrepancies with the cover total instead of changing printed marks.
- Write demand as `Low`, `Moderate`, or `High` in JSON; these correspond to Foundation, Standard, and Challenge in the earlier E-Math calibration rules. AO values are exactly `AO1`, `AO2`, or `AO3`.
- For O Level papers use `"category": "olevel"` and the verified `examSession` (`"J"` or `"N"`). Do not infer an unknown session.
- If actual question crops are unavailable, use `"images": []`; never fabricate images. Keep unverified answers empty. Provide the file as downloadable `.json`, without Markdown fences, plus a short separate uncertainty list. The teacher can attach the PDF and crop in the editor after import.

## 13. Source and completeness audit

1. Read the PDF visually as well as its text layer; diagrams, image-based tables, mathematical symbols and printed marks may be absent or misleading in extracted text.
2. Record every labelled leaf part, including nested labels such as `d(i)` and `c(iii)`.
3. Keep unlabelled composite tasks intact when no subpart mark allocation is printed. Do not invent marks for table rows.
4. Reconcile part totals to each question and then to the cover-page total. When OCR/text extraction duplicates a mark, use the printed page and the total to resolve it.
5. Retain question identity as school + year + paper + question/part, with original source references.
6. Audit existing entries before adding a paper already present. Correct omissions, marks and tags without duplicating it.
7. Keep answer validation separate from tag validation. Do not copy an unverified answer just because it exists in a previous dataset.

## 14. DMN 2026 pilot record (Paper 1 tags approved; Paper 2 pending)

- Source papers: 2026 DMN Mathematics 4052 Paper 1 (24 questions, 90 marks) and Paper 2 (10 questions, 90 marks).
- Both papers were reviewed from the supplied PDFs, including all diagrams and the image-based nutrition data in Paper 2 Q10.
- The uploaded website currently records the DMN bank-paper totals as 59 and 70 marks respectively. The pilot restores the actual 90-mark totals and the missing labelled parts; these corrections have not been applied to the live website.
- Paper 1 Q1 marks are 1, 2 and 2. Paper 1 Q17 is a single 3-mark task despite the duplicate mark in the PDF text layer. Paper 1 Q18 remains one 3-mark table task.
- Paper 1 Q24(b) explicitly tests an obtuse cosine: propose `EM-119` primary with `EM-118` supporting.
- Paper 2 Q9(b)(ii) and Q9(b)(iii) use the approved common-height extension `EM-109.5`; do not classify these only as areas of similar figures.
- Paper 2 Q8(c)(iv) should compare like measures of central tendency. A computed standard deviation in a previous part does not automatically justify `EM-169`.
- Paper 1 tags were approved by the user on 5 October 2026, with Q13(d) corrected to `EM-101`. All other Paper 1 marks, primary/supporting SIOs, AOs and difficulty labels are accepted. Paper 2 remains provisional except the specifically confirmed graphical-solving correction; decisions to vet include Q3(b), Q8(c)(iv), Q9(c).
- In Paper 1 Q19, verify the intended quadrant/domain in the answer stage because distances to axes are non-negative. In Paper 1 Q13(d), verify the intended circular-track radius/tangency reading.
- Pilot outputs: a visual review and one prepared JSON package for each paper. Final-answer fields are blank in this tagging/import pilot, pending a separate answer check.
- Incorporate the user's subsequent corrections into this guide and the pilot data. Do not promote provisional AO/SIO choices into binding examples before the user confirms them.

### Change log

| Date | Status | Change |
|---|---|---|
| 5 October 2026 | User-confirmed | Every Paper 2 final question is PRWC. |
| 5 October 2026 | Source-verified | Audited DMN 2026 P1/P2 question completeness and marks; both total 90. |
| 5 October 2026 | Proposed for vetting | Added the DMN pilot tagging decisions, import mapping and review notes. |

## 15. Confirmed DMN Paper 1 review (5 October 2026)

- User correction: **2026 DMN P1 Q13(d) primary SIO is EM-101** (geometrical constructions), not EM-129. Preserve the existing exact EM-101 taxonomy wording.
- Retain Q13(d) supporting tags EM-29 and EM-107, 2 marks, AO2 and Standard difficulty.
- All other Paper 1 tagging proposals are approved. This includes Q3 → EM-49/AO2, Q6 → EM-86/AO2 and Q21 → EM-111/AO2. These are question-specific decisions, not universal rules for their topics.
- Paper 2 approval is pending. Final answers remain unchecked. The importer still resets parts to unreviewed; teacher approval of tags does not validate answers or publish the paper.

| Date | Status | Change |
|---|---|---|
| 5 October 2026 | User-confirmed | Corrected P1 Q13(d) to EM-101; approved the remaining Paper 1 tags. |

## 16. DMN 2023–2025 six-paper batch (proposals awaiting vetting)

These six packages were rebuilt from the supplied preliminary-examination PDFs. They are not a blind reuse of the older website records. The user’s website adds two teacher-extension SIOs while retaining the original TOS numbering.

| Year | Paper | Questions | Parts/tasks | Marks |
|---|---|---:|---:|---:|
| 2023 | 1 | 27 | 47 | 90 |
| 2023 | 2 | 9 | 42 | 90 |
| 2024 | 1 | 24 | 51 | 90 |
| 2024 | 2 | 10 | 42 | 90 |
| 2025 | 1 | 27 | 51 | 90 |
| 2025 | 2 | 9 | 42 | 90 |

- Total: 106 whole questions and 265 labelled leaf parts or unsplit tasks, 540 marks. All six papers total 90 marks individually.
- Proposed coverage: 91 distinct primary SIOs and 103 distinct primary/supporting SIOs, out of the active 130-SIO E-Math taxonomy. Coverage is provisional until teacher approval.
- Paper 2 PRWC final questions: 2023 Q9 (air medical service), 2024 Q10 (daily energy expenditure), 2025 Q9 (hall fans). Use the most suitable existing number/algebra or geometry PRWC SIO for each part.
- Keep 2023 P2 Q9(a) as one 2-mark task for mean and standard deviation: the paper gives no individual statistic marks. Its PRWC primary is EM-87, with EM-165 and EM-168 supporting.
- The [3] printed on both answer lines of 2023 P2 Q1(a) and 2024 P2 Q1(b) is a repeated task allocation; count 3 marks once, not 6. The paper totals confirm this.
- 2024 P1 Q24(b)(iii) proposes EM-109.5: APO and BOQ are not similar because the two side ratios differ. Use successive common-height area relationships.
- 2025 P1 Q20 proposes EM-109: compare the unpainted upper triangle with the whole lateral face, then subtract slant heights for the painted lower strip.
- 2025 P1 Q10 has constant denominators; EM-47 specifically covers fractional linear expressions. Do not automatically assign EM-56, whose examples have variable denominators.
- For these supplied 2025 preliminary papers, the multi-law indices parts are P1 Q5(a)/(b), not Q3(a)/(b). Earlier examples in this guide may refer to other papers/versions; always check the actual uploaded question and preserve source identity.
- Completed-square expression tasks use the new EM-53.5. A task that explicitly solves a quadratic by completing the square still uses EM-72.
- Graphical equation solving now has a dedicated SIO, EM-67.5. Rational-expression cancellation has no dedicated SIO; use the closest appropriate existing tag and flag uncertainty.
- The 2025 P2 Q7 number grid is partly clipped at the bottom in the original PDF; the cross needed for the question is visible. Preserve it and record the source issue; do not silently reconstruct the graphic.
- The 2025 P2 Q9 airflow formula includes VFR × 70 × number of fans, although the specifications list model RPM values of 60, 50 and 45. Retain the printed source and flag the inconsistency for the teacher before preparing answers.
- Existing website question-count errors include 2023 P1 (28 entries versus 27 source questions), 2023 P2 (10 versus 9), and 2024 P2 (11 versus 10). Import only into fresh review drafts; updating existing records is a separate operation.
- Crops preserve shared stems, tables, diagrams, scales and graph grids at consistent horizontal width. Long blank working gaps, response rows and page separators are omitted. Scale/measurement questions retain the PDF horizontal scale internally; printed worksheet sizing must be calibrated during export.
- Final-answer fields remain blank. Teacher approval of tags must be kept separate from answer validation and publishing.

### Decisions requiring vetting

- 2023 P2 Q1(c): There is no separate cancellation SIO. EM-55 is the closest existing fraction-simplification tag; vet against EM-53 or EM-54 if factorisation is preferred.
- 2023 P2 Q2(b(iv)): The task invokes the cyclic nature of a regular polygon and angle at centre/circumference. EM-98 is a plausible primary alternative.
- 2023 P2 Q4(d(ii)): Proposed EM-67.5 under the new graphical equation-solving SIO. This analogous application remains awaiting teacher review.
- 2024 P2 Q1(e): EM-55 is the closest existing rational-simplification SIO; vet if the assessed focus is instead the identities in EM-53.
- 2024 P2 Q2(d): The grouped-data assumption is implicit: additions near the mean are expected to reduce spread. Exact within-class masses are unspecified; vet the intended interpretation.
- 2025 P1 Q12: Proposed primary is rational simplification; multiple distinct factorisation identities are required. EM-53 is an alternative primary.
- 2025 P1 Q22(c): One combined 2-mark part asks about mean and SD. Primary EM-167 emphasises the change in spread, with central tendency supporting; EM-169 is a plausible broader alternative.
- 2025 P2 Q9(c): The source specifies ×70 in its airflow formula, whereas model RPM values differ. Retain the printed formula in the question crop and flag this modelling inconsistency for the teacher; do not silently edit it.

### Batch change log

| Date | Status | Change |
|---|---|---|
| 5 October 2026 | Source-verified | Rebuilt and reconciled six DMN 2023–2025 papers to 90 marks each. |
| 5 October 2026 | Proposed for vetting | Prepared six portable JSON import packages and three annual visual tagging reviews. |

## 17. Authoritative user website and confirmed corrections (5 October 2026)

The user replaced the earlier website-update request: they have added the SIOs themselves. The newly uploaded `math-workspace.zip`, whose active bundle is `assets/main-BQYii9qv.js`, is authoritative. Its effective E-Math taxonomy has 130 SIOs. Original TOS numbering is unchanged. The earlier row-insertion proposal (EM-54 / EM-69 and probability EM-174) is superseded. Do not apply that renumbering to this website or these packages.

| Current website ID | Chapter | Use |
|---|---|---|
| EM-53.5 | Algebraic expressions and formulae | Express a quadratic in completed-square form. The website label specifies the completing-the-square identity. |
| EM-67.5 | Functions and graphs | Use graphical methods to solve equations, for example by drawing a suitable straight line. |
| EM-172 | Probability | Probability of single events. |

| Paper | Part | User-confirmed correction |
|---|---|---|
| 2026 Paper 2 | Q6(c)(i) | Primary EM-67.5 |
| 2023 Paper 1 | Q11(a) | Primary EM-53.5 |
| 2024 Paper 1 | Q16(a) | Primary EM-53.5 |
| 2024 Paper 2 | Q3(d)(ii) | Primary EM-67.5 |
| 2025 Paper 1 | Q13(a) | Primary EM-53.5 |
| 2025 Paper 1 | Q21(a) | Primary EM-172 |
| 2025 Paper 2 | Q7(a)(iii) | AO3 |

All primary/supporting tags and whole-question practice anchors in all eight DMN packages use the current website numbering. Only the fields listed above are confirmed by this correction; other proposed tags remain pending. The previous approval of all 2026 Paper 1 tags is retained, including Q13(d) primary EM-101. Existing marks, crops, difficulty, supporting tags and other AOs are preserved. Every Paper 2 final question is PRWC. Final answers remain blank pending validation.

The analogous 2023 Paper 2 Q4(d)(ii) remains a proposed application of EM-67.5. Its user approval has not been inferred from the explicit correction list.

Package taxonomy version: `emath-tos-user-2026-10-05`. The bundle contains the eight corrected JSON packages, four visual reviews, this guide, a current TOS reference and import instructions. It does not change or deploy the website. The earlier claim that website review drafts were already installed does not apply to the user’s uploaded website; import these packages once into fresh review drafts. The importer appends questions, creates unreviewed parts and does not update an existing paper. Keep tag approval separate from answer validation and publication.


## 18. AHS 2025, CGSS 2025 and MSHS 2026 six-paper batch (6 October 2026)

All tags in this batch are **proposals awaiting teacher vetting**. They do not inherit the earlier DMN 2026 Paper 1 approval. The current 130-SIO website taxonomy and original row numbering are retained; no website changes have been made.

| School | Year | Paper | Questions | Parts/tasks | Marks |
|---|---:|---:|---:|---:|---:|
| AHS | 2025 | 1 | 23 | 50 | 90 |
| AHS | 2025 | 2 | 16 | 47 | 90 |
| CGSS | 2025 | 1 | 24 | 44 | 90 |
| CGSS | 2025 | 2 | 9 | 42 | 90 |
| MSHS | 2026 | 1 | 27 | 49 | 90 |
| MSHS | 2026 | 2 | 9 | 48 | 90 |

- Total: **108 whole questions, 280 labelled parts/tasks, 540 marks**. Every paper independently totals 90 marks.
- Repeated AHS Paper 2 and CGSS Paper 1 uploads are byte-identical duplicates. Use each unique paper once.
- Each package contains one primary SIO per part, optional supporting SIOs, AO, difficulty, marks, assessment-demand reasoning and confidence. Whole-question practice anchors are selected from that question's primary part tags.
- Every Paper 2 final question is PRWC: **AHS Q16 (cookies), CGSS Q9 (room/home theatre), MSHS Q9 (transport budget)**. Apply the appropriate existing PRWC SIO to each part; record technical skills as supporting when useful.
- MSHS Paper 2 Q9(a) prints separate [1] allocations for petrol cost and EV charging cost. Retain these as two descriptive tasks, `a (petrol cost)` and `a (EV charging cost)`, with one mark each. Do not invent source (i)/(ii) labels. Combined tasks without separate allocations remain intact.
- AHS Paper 1 Q12(i) prints [2] despite a B1 marking note. The package uses the printed 2-mark allocation, consistent with the 90-mark paper total.
- Proposed completed-square expression example: **AHS P2 Q4(a) → EM-53.5**. Explicitly solving by completing the square, **MSHS P1 Q16**, remains **EM-72**.
- Proposed graphical equation-solving examples: **AHS P2 Q13(c), CGSS P2 Q4(d)(i)/(ii), MSHS P2 Q4(c)(ii) → EM-67.5**. Drawing a specified straight line alone remains EM-61; forming the resulting equation is assessed separately.
- Proposed common-height area examples: **AHS P2 Q14(c)/(d)(i)/(d)(ii), CGSS P2 Q5(b), MSHS P1 Q27(c) → EM-109.5**.
- CGSS Paper 1 Q7 asks for **y=3^x and y=3/x**, as one 2-mark task. EM-66 is proposed primary with EM-65 supporting. Do not misread the exponential as y=3x.
- AHS Paper 1 Q15 is a **telescoping fractional pattern**; do not describe it as a geometric series. Finite-sum tasks have no dedicated SIO in the supplied taxonomy; the pattern tag is proposed with medium confidence.
- Multi-law indices tasks use the agreed AO2 convention. Direct calculations use AO1; interpretation, critique and explanation tasks generally use AO3. Routine geometric reasons/proofs continue the agreed AO2 calibration. Each proposal retains its question-specific reasoning.
- Eleven part/task decisions have medium confidence. Review their alternatives and reasoning in the HTML files, especially finite sums, polynomial grouping, rational cancellation, vector/coordinate proof alternatives, the integer-factor search, and MSHS P2 Q7(a)(iv) AO2/AO3 calibration. These are proposals, not new universal rules.

### Source quality and answer separation

- AHS Paper 1 is supplied with worked solutions and marking notes. Remove its solution-table regions from the crops, including continuation rows, while preserving original stems, expressions, diagrams, tables and printed marks. Do not treat those solutions as validated answer content.
- **AHS P1 Q9(a)** is already shaded within its bitmap. Q9(b)'s shading is part of its actual question and must remain. Replace Q9(a) with a clean original before student use.
- **AHS P1 Q19** has detached speed-time axis labels in the supplied source. Preserve the original information and check/replace the graph before student use.
- **AHS P1 Q20** has detached circle-diagram point and angle labels. Replace it with a clean original before student use.
- **AHS P1 Q22** has a matrix X that is not visible in the rendered supplied PDF. Confirm or replace it from a clean original before student use.
- **AHS P1 Q23** contains completed construction lines and misaligned point labels within the bitmap. Preserve and flag it for a clean original before student use; do not silently reconstruct measurement geometry.
- **AHS P2 Q8** states 180 oranges, but its frequencies 10, 28, 51, 45 and 48 total 182. Preserve and resolve the source discrepancy before validating answers.
- **AHS P2 Q15** gives cone diameter 20 cm, height 40 cm and total curved area 150 cm². These are geometrically inconsistent. Preserve and flag the source figures before validating answers.
- **CGSS P1 Q17** states a strict cylinder-volume comparison for all real l and b. Physical lengths must be positive; strict inequality requires l>b, while l=b gives equal volumes. Retain and flag the claim.
- **CGSS P2 Q8(f)** compares revenue while calling it profitability; production costs are unspecified. Vet the modelling assumption.
- Exclude the appended MSHS answer-key pages: Paper 1 PDF page 23 and Paper 2 PDF page 25. Preserve original question stems through PDF pages 21 and 23 respectively.
- Long blank working gaps, response rows and page separators are omitted. Necessary diagrams/grids retain their geometry. Scale-sensitive printed export still requires calibration.
- All final-answer fields stay blank. Keep teacher tag approval, answer validation and publication separate. Import once into fresh review drafts: the importer appends questions and creates unreviewed parts.

### Batch change log

| Date | Status | Change |
|---|---|---|
| 6 October 2026 | Source-verified | Audited six unique AHS/CGSS/MSHS papers and reconciled each to 90 marks. |
| 6 October 2026 | Proposed for vetting | Prepared six portable JSON packages, three self-contained visual reviews, and a 280-row tagging table. |
| 6 October 2026 | Source-issue flagged | Recorded annotated diagrams, detached labels and mathematical/wording inconsistencies for teacher review. |


## 19. Portable tagging workflow and output requirements (11 October 2026)

### Source audit

- Identify the actual school, year, subject and paper number from the source, not a filename alone. Keep school-specific questions separate even when their question numbers match.
- Check repeated uploads for exact duplicates and include each unique paper once.
- List every whole question and every marked leaf part before assigning tags. Preserve nested labels, for example `a(i)`, `c(ii)` and `d(iii)`.
- Preserve one combined task when no separate allocation is printed. If separate allocations are printed without roman-number labels, descriptive task labels may be used while retaining the original parent label; do not invent official subpart numbers.
- Use the question paper's printed allocation. Marking-scheme method marks such as M1/A1/B1 do not replace the question-paper allocation. Repeated answer-line marks do not necessarily represent separate tasks; verify visually and reconcile totals.
- Read image-based mathematics and diagrams visually. OCR may omit fractions, exponents, set symbols, vector arrows, units, graph scales or marks.
- A filename containing “QP” does not guarantee an answer-free paper. Detect embedded solutions and appended answer keys. Keep validated answers in separate answer fields; leave them blank if answer validation is outside the requested task.

### Primary SIO decisions

| Actual assessed demand | Tagging approach |
|---|---|
| Express a quadratic in completed-square form | EM-53.5. |
| Explicitly solve a quadratic by completing the square | EM-72, whose wording includes solving by completing the square. |
| Solve an equation using graph intersections or a suitable line | EM-67.5. |
| Draw only a specified straight line | Use the appropriate straight-line SIO; do not automatically assign graphical equation solving. |
| Infer a triangle-area ratio from equal heights and base lengths | EM-109.5; do not require similarity when it is not established. |
| Calculate a single-event probability | EM-172; distinguish subsequent combined, independent or mutually exclusive events using the exact reference. |
| Select or infer mathematics from a diagram, then calculate | Tag the central assessed skill; diagram inference can make the AO2 demand even when the final calculation is routine. |
| Final question of Paper 2 | Keep whole-question PRWC classification and choose the applicable existing PRWC SIO per part. |
| No exact existing SIO for the assessed demand | Propose the closest appropriate existing SIO, explain the scope mismatch and flag Medium/Low confidence. Do not invent a new extension. |

A secondary tag records a useful supporting demand, not every operation in a solution. The strand and chapter are derived from the primary SIO. A whole-question practice anchor, when required, must be one of that question's actual primary part tags.

### AO and difficulty checks

- **AO1:** Direct reading, routine taught methods, straightforward formula application, standard direct-proportion formulation and explicitly requested standard constructions.
- **AO2:** Selection or combination of techniques, multi-law indices, formulation beyond a direct taught template, inference from diagrams, analysis-based “show that” tasks, or interpreting loci conditions.
- **AO3:** Assessed explanation, contextual interpretation, critique, comparison, justification of a claim or recommendation, and non-simple statistical reasoning.
- The words “show”, “explain” and “justify” are evidence of the demand, not a complete AO rule. Check the mathematics and confirmed examples. Do not classify every multi-step taught algorithm as AO2 simply because it has several written lines.
- A real-world context alone does not raise the AO. Direct compound-interest formula application remains AO1. PRWC classification alone does not determine AO or difficulty.
- Judge difficulty from demand rather than marks or AO alone. Write **Low / Moderate / High** in the DMN Workspace JSON, corresponding to **Foundation / Standard / Challenge** in the calibration rules.

### Review output

Unless the user requests a different format, include these columns:

| Source | Part/task | Marks | Primary SIO ID and exact description | Supporting SIO IDs and descriptions | Strand / chapter | AO | Difficulty | Confidence | Short reason / issue |
|---|---|---:|---|---|---|---|---|---|---|
| School + year + paper + question | Original label | Printed allocation | One primary | Only useful supporting skills | From primary SIO | AO1/2/3 | Foundation/Standard/Challenge | High/Medium/Low | Assessment demand and any ambiguity |

- List uncertain decisions and source defects clearly. Confidence is separate from teacher approval: a High-confidence proposal still awaits approval unless explicitly confirmed.
- Use the self-contained DMN Workspace JSON example in section 12. No separate template is needed for this workflow.
- Do not infer website installation or publication from creating a JSON package. Import into a fresh draft only when using the previously audited append-only importer; check the actual current importer if updating an existing record.
- Provide visual review HTML only when requested or appropriate to the task. If the user asks for JSON only, deliver JSON and a concise uncertainty list; no separate HTML is required.
- If crops are requested, preserve shared stems, necessary grids, source labels and continuation content. Keep diagram geometry and consistent horizontal scale. Remove only response/working content that can be distinguished reliably from the actual question. Never remove a sequence instruction or table entry merely because it contains ellipses.
- Do not silently reconstruct a missing matrix, redraw a measurement diagram, move source labels, change a frequency, or correct a defective mathematical premise. Retain a source-issue flag and identify the clean source or teacher decision needed.

### How to update this guide

After a batch, record its school/year/paper identities, question and part counts, mark reconciliation, duplicates, source issues, uncertain decisions and output status. After a teacher correction, record the exact source part, changed field, previous/proposed value if helpful, final accepted value, date and approval scope. Retain confirmed decisions and mark superseded instructions explicitly.

The AHS/CGSS/MSHS proposals in section 18 remain pending teacher vetting. This portable export does not newly tag or approve the BDS, NASS, RSS, YTSS or other attached papers. Read and tag each requested new paper from its actual source.

### Change log

| Date | Status | Change |
|---|---|---|
| 11 October 2026 | Guide updated | Made the guide self-contained for a new chat, clarified historical taxonomy counts and AO calibration, and embedded the complete recorded 130-SIO reference. |

## 20. Full recorded E-Math SIO reference

Reference version: `emath-tos-user-2026-10-05`. The reference was previously verified against the user's uploaded website and saved as `Current_Emath_SIO_Reference.json`. The IDs, strands, chapters and wording below are retained from that saved reference. This is the recorded E-Math taxonomy, not an A-Math taxonomy. Explicit newer user corrections or a newer supplied taxonomy take precedence.

Only assign IDs present here or in an explicitly newer authoritative user-supplied reference. Preserve mathematical notation and the examples within each SIO; those examples inform scope. Number gaps and decimal insertion IDs are intentional.

### Number & Algebra

#### Numbers and their operations

| SIO ID | Exact recorded description |
|---|---|
| EM-16 | primes and prime factorisation |
| EM-17 | finding highest common factor (HCF) and lowest common multiple (LCM), squares, cubes, square roots and cube roots by prime factorisation |
| EM-18 | negative numbers, integers, rational numbers, real numbers and their four operations |
| EM-19 | calculations with calculator |
| EM-20 | representation and ordering of numbers on the number line |
| EM-21 | use of <, >, ⩽, ⩾ |
| EM-22 | approximation and estimation (including rounding off numbers to a required number of decimal places or signficant figures and estimating the results of computation) |
| EM-23 | use of standard form $A\times10^n$ where $n$ is an integer, and $1 \le A < 10$ |
| EM-24 | positive, negative, zero and fractional indices |
| EM-25 | laws of indices |

#### Ratio and Proportion

| SIO ID | Exact recorded description |
|---|---|
| EM-27 | ratios involving rational numbers |
| EM-28 | writing a ratio in its simplest form |
| EM-29 | map scales (distance and area) |
| EM-30 | direct and inverse proportion |

#### Percentage

| SIO ID | Exact recorded description |
|---|---|
| EM-32 | expressing one quantity as a percentage of another |
| EM-33 | comparing two quantities by percentage |
| EM-34 | percentages greater than 100% |
| EM-35 | increasing/decreasing a quantity by a given percentage |
| EM-36 | reverse percentages |

#### Rate and speed

| SIO ID | Exact recorded description |
|---|---|
| EM-38 | average rate and average speed |
| EM-39 | conversion of units (e.g. km/h to m/s) |

#### Algebraic expressions and formulae

| SIO ID | Exact recorded description |
|---|---|
| EM-41 | using letters to represent numbers |
| EM-42 | interpreting notations:<br>- $ab$ as $a\times b$<br>- $\frac{a}{b}$ as $a\div b$ or $a\times\frac{1}{b}$<br>- $a^2$ as $a\times a$, $a^3$ as $a\times a\times a$, $a^2b$ as $a\times a\times b$, …<br>- $3y$ as $y+y+y$ or $3\times y$<br>- $3(x+y)$ as $3\times(x+y)$<br>- $\frac{3+y}{5}$ as $(3+y)\div5$ or $\frac15\times(3+y)$ |
| EM-43 | evaluation of algebraic expressions and formulae |
| EM-44 | translation of simple real-world situations into algebraic expressions |
| EM-45 | recognising and representing patterns/relationships by finding an algebraic expression for the nth term |
| EM-46 | addition and subtraction of linear expressions |
| EM-47 | simplification of linear expressions such as $-2(3x-5)+4x$ and $\frac{2x}{3}-\frac{3(x-5)}{2}$ |
| EM-48 | use brackets and extract common factors |
| EM-49 | factorisation of linear expressions of the form $ax+bx+kay+kby$ |
| EM-50 | expansion of the product of algebraic expressions |
| EM-51 | changing the subject of a formula |
| EM-52 | finding the value of an unknown quantity in a given formula |
| EM-53 | use of:<br>- $(a+b)^2=a^2+2ab+b^2$<br>- $(a-b)^2=a^2-2ab+b^2$<br>- $a^2-b^2=(a+b)(a-b)$ |
| EM-53.5 | completing the square using $x^2+px=\left(x+\frac{p}{2}\right)^2-\left(\frac{p}{2}\right)^2$ |
| EM-54 | factorisation of quadratic expressions $ax^2+bx+c$ |
| EM-55 | multiplication and division of simple algebraic fractions such as $\left(\frac{3a}{4b^2}\right)\left(\frac{5ab}{3}\right)$ and $\frac{2a}{4}\div\frac{9a^2}{10}$ |
| EM-56 | addition and subtraction of algebraic fractions with linear or quadratic denominator such as:<br>- $\frac{1}{x-2}+\frac{2}{x-3}$<br>- $\frac{1}{x^2-9}+\frac{2}{x-3}$<br>- $\frac{1}{x-3}+\frac{2}{(x-3)^2}$ |

#### Functions and graphs

| SIO ID | Exact recorded description |
|---|---|
| EM-58 | Cartesian coordinates in two dimensions |
| EM-59 | graph of a set of ordered pairs as a representation of a relationship between two variables |
| EM-60 | linear functions (y = ax + b) and quadratic functions   (y = ax² + bx+ c) |
| EM-61 | graphs of linear functions |
| EM-62 | the gradient of a linear graph as the ratio of the vertical change to the horizontal change (positive and negative gradients) |
| EM-63 | graphs of quadratic functions and their properties:<br>- positive or negative coefficient of $x^2$<br>- maximum and minimum points<br>- symmetry |
| EM-64 | Sketching the graphs of quadratic functions given in the form:<br>- $y=(x-p)^2+q$<br>- $y=-(x-p)^2+q$<br>- $y=(x-a)(x-b)$<br>- $y=-(x-a)(x-b)$ |
| EM-65 | graphs of power functions of the form $y=ax^n$, where $n=-2,-1,0,1,2,3$, and simple sums of not more than three of these |
| EM-66 | graphs of exponential functions $y=ka^x$, where $a$ is a positive integer |
| EM-67 | estimation of the gradient of a curve by drawing a tangent |
| EM-67.5 | using graphical methods to solve equations (e.g. by drawing a suitable straight line) |

#### Equations and Inequalities

| SIO ID | Exact recorded description |
|---|---|
| EM-69 | solving linear equations in one variable |
| EM-70 | solving simple fractional equations that can be reduced to linear equations such as:<br>- $\frac{x}{3}+\frac{x-2}{4}=3$<br>- $\frac{3}{x-2}=6$ |
| EM-71 | solving simultaneous linear equations in two variables by:<br>- substitution and elimination methods<br>- graphical method |
| EM-72 | solving quadratic equations in one unknown by:<br>- factorisation<br>- use of formula<br>- completing the square for $y=x^2+px+q$<br>- graphical methods |
| EM-73 | solving fractional equations that can be reduced to quadratic equations such as:<br>- $\frac{6}{x+4}=x+3$<br>- $\frac{1}{x-2}+\frac{2}{x-3}=5$ |
| EM-74 | formulating equations to solve problems |
| EM-75 | solving linear inequalities in one variable, and representing the solution on the number line |

#### Set language and notation

| SIO ID | Exact recorded description |
|---|---|
| EM-77 | use of set language and notation:<br>- union of $A$ and $B$: $A\cup B$<br>- intersection of $A$ and $B$: $A\cap B$<br>- “is an element of”: $\in$<br>- “is not an element of”: $\notin$<br>- complement of set $A$: $A'$<br>- the empty set: $\varnothing$<br>- universal set: $\xi$<br>- $A$ is a (proper) subset of $B$: $A\subset B$<br>- $A$ is not a (proper) subset of $B$: $A\not\subset B$ |
| EM-78 | union and intersection of two sets |
| EM-79 | Venn diagrams |

#### Matrices

| SIO ID | Exact recorded description |
|---|---|
| EM-81 | display of information in the form of a matrix of any order |
| EM-82 | interpreting the data in a given matrix |
| EM-83 | product of a scalar quantity and a matrix |
| EM-84 | problems involving the calculation of the sum and product (where appropriate) of two matrices |

#### Problems in real-world contexts (NUMBER & ALGEBRA)

| SIO ID | Exact recorded description |
|---|---|
| EM-86 | solving problems based on real-world contexts:<br>- in everyday life (including travel plans, transport schedules, sports and games, recipes, etc.)<br>- involving personal and household finance (including simple and compound interest, taxation, instalments, utilities bills, money exchange, etc.) |
| EM-87 | interpreting and analysing data from tables and graphs, including distance–time and speed–time graphs |
| EM-88 | interpreting the solution in the context of the problem |

### Geometry & Measurement

#### Angles, triangles and polygons

| SIO ID | Exact recorded description |
|---|---|
| EM-95 | right, acute, obtuse and reflex angles |
| EM-96 | vertically opposite angles, angles on a straight line and angles at a point |
| EM-97 | angles formed by two parallel lines and a transversal: corresponding angles, alternate angles, interior angles |
| EM-98 | properties of triangles, special quadrilaterals and regular polygons (pentagon, hexagon, octagon and decagon) including symmetry properties |
| EM-99 | classifying special quadrilaterals on the basis of their properties |
| EM-100 | angle sum of interior and exterior angles of any convex polygon |
| EM-101 | construction of simple geometrical figures from given data (including perpendicular bisectors and angle bisectors) using compasses, ruler, set squares and protractor, where appropriate |

#### Congruence and Similarity

| SIO ID | Exact recorded description |
|---|---|
| EM-103 | congruent and similar figures |
| EM-104 | properties of similar triangles and quadrilaterals:<br>- corresponding angles are equal<br>- corresponding sides are proportional |
| EM-105 | enlargement and reduction of a plane figure |
| EM-106 | scale drawings |
| EM-107 | properties of perpendicular bisectors of line segments and angle bisectors |
| EM-108 | determining whether two triangles are:<br>- congruent<br>- similar |
| EM-109 | ratio of areas of similar plane figures |
| EM-110 | ratio of volumes of similar solids |
| EM-111 | solving simple problems involving similarity and congruence |
| EM-109.5 | areas of triangles with common height |

#### Properties of circles

| SIO ID | Exact recorded description |
|---|---|
| EM-113 | symmetry properties of circles:<br>- equal chords are equidistant from the centre<br>- the perpendicular bisector of a chord passes through the centre<br>- tangents from an external point are equal in length<br>- the line joining an external point to the centre of the circle bisects the angle between the tangents |
| EM-114 | angle properties of circles:<br>- angle in a semicircle is a right angle<br>- angle between tangent and radius of a circle is a right angle<br>- angle at the centre is twice the angle at the circumference<br>- angles in the same segment are equal<br>- angles in opposite segments are supplementary |

#### Pythagoras' theorem and trigonometry

| SIO ID | Exact recorded description |
|---|---|
| EM-116 | use of Pythagoras’ theorem |
| EM-117 | determining whether a triangle is right-angled given the lengths of three sides |
| EM-118 | use of trigonometric ratios (sine, cosine and tangent) of acute angles to calculate unknown sides and angles in right-angled triangles |
| EM-119 | extending sine and cosine to obtuse angles |
| EM-120 | use of the formula $\frac12 ab\sin C$ for the area of a triangle |
| EM-121 | use of sine rule and cosine rule for any triangle |
| EM-122 | problems in two and three dimensions including those involving angles of elevation and depression and bearings |

#### Mensuration

| SIO ID | Exact recorded description |
|---|---|
| EM-124 | area of parallelogram and trapezium |
| EM-125 | problems involving perimeter and area of composite plane figures |
| EM-126 | volume and surface area of cube, cuboid, prism, cylinder, pyramid, cone and sphere |
| EM-127 | conversion between cm² and m², and between cm³ and m³ |
| EM-128 | problems involving volume and surface area of composite solids |
| EM-129 | arc length, sector area and area of a segment of a circle |
| EM-130 | use of radian measure of angle (including conversion between radians and degrees) |

#### Coordinate Geometry

| SIO ID | Exact recorded description |
|---|---|
| EM-132 | finding the gradient of a straight line given the coordinates of two points on it |
| EM-133 | finding the length of a line segment given the coordinates of its end points |
| EM-134 | interpreting and finding the equation of a straight line graph in the form $y=mx+c$ |
| EM-135 | geometric problems involving the use of coordinates |

#### Vectors in two dimensions

| SIO ID | Exact recorded description |
|---|---|
| EM-137 | use of notations: $\begin{pmatrix}x\\y\end{pmatrix}$, $\overrightarrow{AB}$, $\mathbf{a}$, $\|\overrightarrow{AB}\|$, $\|\mathbf{a}\|$ |
| EM-138 | representing a vector as a directed line segment |
| EM-139 | translation by a vector |
| EM-140 | position vectors |
| EM-141 | magnitude of a vector $\begin{pmatrix}x\\y\end{pmatrix}$ as $\sqrt{x^2+y^2}$ |
| EM-142 | use of sum and difference of two vetcors to express given vectors in terms of two coplanar vectors |
| EM-143 | multiplication of a vector by a scalar |
| EM-144 | geometric problems involving the use of vectors |

#### Problems in real-world contexts (GEOMETRY)

| SIO ID | Exact recorded description |
|---|---|
| EM-146 | solving problems in real-world contexts (including floor plans, surveying, navigation, etc.) using geometry |
| EM-147 | interpreting the solution in the context of the problem |
| EM-151 | interpreting the solution in the context of the problem |

### Statistics & Probability

#### Data Analysis

| SIO ID | Exact recorded description |
|---|---|
| EM-158 | simple concepts in collecting, classifying and tabulating data (newly added for 2023 syllabus) |
| EM-159 | analysis and interpretation of: <br>∗ tables <br>∗ bar graphs <br>∗ pictograms <br>∗ line graphs <br>∗ pie charts <br>∗ dot diagrams <br>∗ histograms with equal class intervals <br>∗ stem-and-leaf diagrams<br>∗ cumulative frequency diagrams<br>∗ box-and-whisker plots |
| EM-160 | purposes and uses, advantages and disadvantages of the different forms of statistical representations |
| EM-161 | drawing simple inference from statistical diagrams (newly added for 2023 syllabus) |
| EM-162 | explaining why a given statistical diagram leads to misinterpretation of data |
| EM-163 | mean, mode and median as measures of central tendency for a set of data |
| EM-164 | purposes and use of mean, mode and median |
| EM-165 | calculation of the mean for grouped data |
| EM-166 | quartiles and percentiles |
| EM-167 | range, interquartile range and standard deviation as measures of spread for a set of data |
| EM-168 | calculation of the standard deviation for a set of data (grouped and ungrouped) |
| EM-169 | using the mean and standard deviation to compare two sets of data |

#### Probability

| SIO ID | Exact recorded description |
|---|---|
| EM-171 | probability as a measure of chance |
| EM-172 | probability of single events (including listing all the possible outcomes in a simple chance situation to calculate the probability) |
| EM-173 | probability of simple combined events (including using possibility diagrams and tree diagrams, where appropriate) |
| EM-174 | addition and multiplication of probabilities (mutually exclusive events and independent events) |


### Taxonomy metadata

- EM-53.5 and EM-67.5 are recorded as teacher extensions with no original integer TOS row.
- EM-109.5 is the approved common-height triangle-area entry. Preserve this existing ID.
- Keep existing duplicate SIO entries where present; do not merge or renumber them without the user's instruction.
- S&P is the tagging-guide abbreviation for Statistics & Probability. A website's display label may differ; derive the underlying strand from this reference.

## 21. GCE O-Level 2026 Mathematics Paper 1 (21 October 2026)

Status: **proposed tagging for teacher vetting**. The earlier approvals apply only to their named papers. No official AO breakdown or marking scheme was supplied, and no website changes were made.

- Source: supplied scanned `GCE O Levels 2026 Paper 1.pdf`, Mathematics 4052/01, October/November 2026. All 19 supplied pages were visually read; the source has no extractable text layer.
- Coverage: **28 questions, 46 marked parts/tasks, 90 marks**, reconciled to the cover total. The additional page mentioned on the cover is blank; the assessed question sequence Q1-Q28 is complete in the supplied PDF.
- Output: `O_Level_2026_Paper_1_Tagging_and_Topics.md`, containing primary/supporting SIO IDs and exact descriptions, marks, AO, difficulty, confidence, reasoning and a topic/mark summary. This is a review report, not an import package.
- Topic-summary marks are allocated once by primary-SIO chapter; supporting skills do not receive duplicate marks. In particular, Q6(a)(i) is allocated to algebraic-expression translation with average speed supporting.
- Proposed **Q3(a) -> EM-98**, supporting EM-96: equal radii establish an isosceles triangle before central-angle subtraction. Proposed **Q3(b) -> EM-114**: angle at the centre versus angle at the circumference. A circle diagram alone does not make every part a circle-theorem task.
- Proposed **Q4 and Q21 -> EM-55**, Medium confidence, following the existing rational-simplification convention because there is no dedicated cancellation SIO. Q4 supports EM-47/48; Q21 supports EM-53/54. Vet common-factor/identity alternatives before treating these as confirmed examples.
- Proposed **Q10(b) -> EM-165 / AO3**: the new observation is entered into a grouped table, so the change in the estimated mean uses its class midpoint (35), rather than the exact observed time (39). This is not a source error.
- Proposed **Q12 -> EM-161 / AO3**, supporting EM-163/167: contextual comparisons from medians and spread in box plots. Do not use EM-169, whose scope explicitly requires mean and standard deviation.
- Proposed **Q18 -> EM-125 / AO2 / Challenge**, supporting EM-116/113/114: composite area between concentric circles from a tangent chord; relate the difference of squared radii to a right triangle.
- Proposed **Q22 -> EM-70 / AO1 / Standard**: after clearing denominators, the quadratic terms cancel, leaving a linear equation. Do not assign EM-73 simply because squared terms appear initially.
- Proposed **Q23 -> EM-25 / AO2**: multiple index laws with a negative fractional outer power, consistent with the user's indices convention.
- Proposed **Q24(a) -> EM-108 / AO2** for triangle similarity proof; **Q24(b) -> EM-111 / AO2 / Challenge** for the linked-similarity height calculation.
- Proposed **Q25(b) -> EM-126 / AO2 / Challenge**, supporting EM-129/116: a sector is formed into a cone; distinguish sector radius/slant height, arc/base circumference and perpendicular cone height.
- Proposed **Q26 -> EM-167 / AO3**, supporting EM-163: a transformation of one dataset to specified mean and standard deviation, not a comparison of two datasets. Retain the one printed mark; do not invent separate statistic marks.
- Proposed **Q28 -> EM-63 / AO2**, supporting EM-53.5: infer coefficients from a quadratic minimum. Completed-square form is a possible method, not the explicitly requested output.
- The Paper 2 final-question PRWC rule does not automatically apply to Paper 1 Q28. Q17 separately uses the existing finance/currency-exchange SIO EM-86.
- No essential unreadable content or mathematical source defect was identified in this tagging pass. No validated answers were supplied or added. Keep teacher tag approval, answer validation and publication separate.

| Date | Status | Change |
|---|---|---|
| 21 October 2026 | Source-verified | Visually audited 2026 GCE O-Level Paper 1; all 28 questions / 46 parts or tasks sum to 90 marks. |
| 21 October 2026 | Proposed for vetting | Added part tags, exact SIO descriptions, AO/difficulty judgements, topic allocation and two Medium-confidence rational-simplification choices. |
