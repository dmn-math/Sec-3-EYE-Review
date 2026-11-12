# A-Math paper tagging rules — portable guide

**Scope:** Singapore Additional Mathematics (4049), for the DMN Math Workspace, reflection papers and topical Ten-Year Series (TYS) worksheets. **Updated:** 11 November 2026.

## Start here in a new chat

Upload **this guide and the actual question paper(s)**. Include a marking scheme if available. For topical TYS, upload the chapter PDFs with the section headings and original exam references visible. If the workspace catalogue or importer has changed, also attach the latest SIO export or a working import template.

Copy this prompt:

> Read the attached A-Math tagging guide in full and use its SIO catalogue, AO rules, C3R demand calibration and TYS section mapping. Tag every printed, mark-bearing part of the supplied paper. Give me a table with the question/part, marks, primary and secondary SIO descriptions with codes, AO, demand and brief reasons or flags. Identify the main concept of each whole question. Let me vet it first, then produce the DMN Workspace JSON using the format in the guide. If I ask for JSON directly, generate it with the flags and leave unvetted parts as reviewed: false.

The guide contains the 52 A-Math catalogue entries and an import example, so another chat can work without this project's history. Use **explicit teacher instructions and the latest supplied A-Math catalogue/import template** when they override this guide. Keep changes specific to the stated paper, cohort or batch. Never apply A-Math codes to E-Math or use the E-Math PRWC convention for A-Math.

## 1. Read and inventory the paper

1. Identify the school/exam, subject, year, paper number and purpose (reflection or question bank) from the cover or teacher. The upload date is not the exam year. If the cover is missing, label the set descriptively and leave unverified metadata unset in the review.
2. Read each question and its continuation, marks, diagram, graph and tables. For scanned PDFs, photo ZIPs or unreliable OCR, inspect the images. Verify easily confused signs, exponents, roots, interval endpoints, labels and constants. A photographed worked solution helps identify the intended method; the question determines what students must do.
3. Make one record for every **independently marked** part. Use the printed question number, with part labels such as `a`, `b(i)` and `b(ii)`. Use `""` for an unlabelled whole question. If two instructions share one printed mark allocation, keep them together; do not invent a split.
4. Record the printed maximum marks, page or image reference, and a short description of the mathematical task. Read or sketch the solution before tagging. Flag missing pages, inconsistent answers, or wording/diagram issues by exact question and reason; continue with the readable parts.
5. Reconcile parts and marks with the printed paper total. If the user excludes a question, preserve the remaining numbering and report both the original total (if known) and the included total. Do not assume every paper is 90 marks.

## 2. Assign SIOs

A **Specific Instructional Objective (SIO)** identifies the skill the examiner is assessing. Use the exact ID and description from the catalogue in section 9, or from a newer teacher-supplied catalogue. The AM numbers are local catalogue IDs; gaps in numbering are intentional.

- **Primary:** Give each mark-bearing part one best-fit SIO. Ask, “What is the main concept or method this part tests?” Choose the most precise supported objective. Derive strand and topic from that SIO: `ALG` = Algebra, `G&T` = Geometry & Trigonometry, `CAL` = Calculus.
- **Secondary:** Add only substantial supporting skills that help diagnose an error or find similar practice. Do not add routine arithmetic, algebraic tidying, a method used only in an earlier part, or every operation a solution happens to contain. Use distinct IDs; never repeat the primary as a secondary.
- **Whole-question match:** Choose a separate `matchSioId` for the question's main assessed concept and best practice match. Consider the central purpose, the main marked work, and how the parts build on one another. It need not be the first part's tag or the tag with the most marks. Preserve the individual part tags for reporting.
- **Alternatives:** Prefer the method required by the wording; then use the mark scheme or a natural syllabus method. If another route changes the classification materially, state the alternative in a note. A solution's optional technique does not prove the question requires it.
- **Uncertainty:** If two tags plausibly fit, choose the better one provisionally and explain why. If **no suitable catalogue match** exists and the teacher has requested next-part fallback, use the next relevant part's supported SIO within that question and record which part it came from. If no defensible fallback exists, use a blank primary when allowed, and flag it for review. Do not borrow a tag from another question or invent an ID. Only the SIO is copied; assess AO and demand for the actual part. A fallback is not evidence of coverage.
- **Teacher changes:** Record the exact paper, question/part, old and new tags and the reason if given. A teacher-confirmed change applies to that item. Keep other classifications unless the correction also affects them.

### Calibration examples

| Assessed work | Tagging decision |
| --- | --- |
| Find conditions on a parameter for a line to intersect or touch a curve using the discriminant | **AM-18 — discriminant and intersection conditions**. Add **AM-20 — quadratic inequalities** only if solving such an inequality is substantial. For proving a quadratic is always positive/negative, **AM-16** can be primary, with AM-18 supporting when the discriminant is used. |
| Complete the square and read a quadratic minimum | **AM-15 — maximum/minimum by completing the square**. Use **AM-17 — quadratic models** where constructing or interpreting the model is the actual target. |
| Substitute a straight-line equation into a nonlinear equation | **AM-19 — simultaneous equations by substitution** if solving the pair is the target. A perpendicular-line or midpoint construction is primarily coordinate geometry (**AM-48** or **AM-49**) when that is the key assessed step. A routine gradient calculation with surd rationalisation can instead be **AM-21**. |
| Resolve an improper rational expression into partial fractions after dividing | **AM-26 — partial fractions**, with **AM-23 — polynomial division** supporting if the division is required. Tag a separate marked polynomial-division part **AM-23**. |
| Solve an exponential or logarithmic equation using log laws | **AM-31 — solving/simplifying exponential or logarithmic expressions**, optionally **AM-30 — functions and log laws**. Use **AM-32** for modelling, or **AM-52** if linearising a relation and finding constants from a straight-line graph is the central task. |
| Prove an identity, then use it to solve a trig equation | **AM-46 — trig identity proof** for the proof, optionally **AM-43 — identities/formulae**; **AM-45 — solve a trig equation in an interval** for the solving part. If explicitly finding principal inverse-trig values/ranges, use **AM-39**. A calculator inverse-tan step alone is incidental; a general inverse function is not AM-39. |
| Differentiate a product, then use a derivative to find a tangent | **AM-63 — product/quotient rule** for the direct derivative; **AM-68 — applications of differentiation** for the tangent equation. Use **AM-66** for finding/classifying stationary points, **AM-67** where the second-derivative test is the focus, and **AM-68** for a contextual optimisation task. |
| Derive a cubic volume by mensuration before maximising it | The derivation has no exact A-Math catalogue match. If instructed to inherit the next part's tag, provisionally copy **AM-68** from the maximisation part and flag the catalogue gap. Do not claim the derivation uses differentiation or a quadratic model. |
| Integrate a standard function with a linear argument; interpret a signed integral | **AM-71 — standard integrals** for the antiderivative; **AM-73 — definite integral evaluation** when the limits/evaluation are the focus; **AM-72 — definite integral as area** for interpreting its sign. Use **AM-74** for a bounded region and **AM-75** for finding an area below the axis as appropriate. For displacement, velocity and acceleration in straight-line motion, **AM-76** is usually the main application. |

## 3. Assign one assessment objective (AO) per part

Judge the work actually demanded, including scaffolding from earlier parts. AO and demand are separate.

| AO | Rule | Examples |
| --- | --- | --- |
| **AO1 — Use and apply standard techniques** | A familiar procedure is clear from the wording, data or previous result. It can still involve several routine calculations. | Differentiate a stated product; complete the square; evaluate a definite integral with the setup supplied; read a turning point from the completed-square form. |
| **AO2 — Solve problems in a variety of contexts** | Students must select a method, interpret conditions, connect representations or techniques, or formulate and solve a model. | Form a line–curve intersection equation and choose the discriminant condition; decide which trig root fits a graph; construct and solve an exponential growth threshold. |
| **AO3 — Reason and communicate mathematically** | The assessed outcome is a mathematical argument, proof, justification or explanation. | Prove a trig identity; justify why a turning point is a minimum; explain why a signed integral gives the difference of two areas. |

A “show that” instruction may be AO1 for a routine calculation, AO2 for choosing and connecting a method, or AO3 when the argument itself earns the marks. Do not assign AO from the command word, marks, SIO or presence of a real-world story alone. If the teacher supplies an AO for the part, use it and note any disagreement for vetting.

## 4. Assign demand: apply the correct rule for the source

### Topical TYS PDFs: transcribe the printed band

| Printed section in the chapter PDF | JSON `difficulty` |
| --- | --- |
| Basic | `Low` |
| Intermediate | `Moderate` |
| Advanced (or Advance) | `High` |

Find the heading governing the exercise, including headings on a preceding page. **Apply that printed band to every assessed part of that exercise**, unless the source separately classifies a part. A routine subpart of an Intermediate item still gets `Moderate`. Do not override printed bands with C3R estimates, marks, question position, the year or a different chapter's heading.

In the audit record, keep the chapter PDF, page, topical exercise number, section heading and original year/paper/question/part. When a heading or reference is missing, inspect the adjacent pages and printed numbering. Flag any remaining gap and keep demand blank if the importer permits it. If two verified reprints disagree on the band for the same part, preserve both source records and flag the conflict before choosing one import value.

### Full exam or revision papers without printed bands: use C3R

Use **Content, Complexity, Context and Response Strategy** as a qualitative profile. Judge demand for the intended students (e.g. Sec 4 A-Math prelim candidates); state the cohort assumption if it matters. The project uses the SEAB discussion in *Assessment in Singapore*, Volume 4, Chapter 6, “Characterising the Demands of Mathematics Items” as a reference. The overall `Low` / `Moderate` / `High` label is this project's judgement, not an official rating for the question.

| Dimension | Lower demand | What can raise demand |
| --- | --- | --- |
| **Content** | One familiar concept or technique | Several ideas must be understood and connected; a less familiar consequence of known content must be recognised. |
| **Complexity** | Direct substitution or a short familiar procedure | Interdependent steps, cases, constraints, or switching between representations. Long routine arithmetic alone is weak evidence. |
| **Context** | Familiar mathematical setting, explicit data and goal | The student has to interpret unfamiliar information or select what is relevant. A story wrapped around a direct substitution does not add much demand. |
| **Response strategy** | Method and response are clear or cued by prior parts | Choose, adapt or devise a method; decide on cases, validate an outcome, or construct a justification. |

- **Low:** The route is familiar and cued. Example: differentiate `x² sin x` directly.
- **Moderate:** Some independent selection, interpretation or linking is required. Example: combine the discriminant with a parameter inequality to find two line–curve intersections.
- **High:** There is substantial unscaffolded reasoning, modelling, strategic choice, or coordination of constraints. Example: derive conditions on two parameters for a global quadratic bound, including distinct cases if a quadratic may degenerate.

Assign the overall band by explaining what the student must figure out. Do not average the four dimensions or map AO1/AO2/AO3 directly to the three bands. A short justification may be AO3/Low; an involved multi-condition problem can be AO2/High. Where requested, show all four C3R dimensions and the overall judgement in the review.

## 5. Handle topical TYS and practice recommendations

**Topical imports.** Inventory the requested `TYS_XX_Chapter name.pdf` sources. For the full project set, reconcile all 16 numbered chapters in section 10. Use the printed original exam reference for identity; topical exercise number is a locator, not the original question number. Group import files by original year and paper (e.g. `YYYY_TYS_AMath_P1_Package.json`). Sort by original Q number and preserve part labels. If the same original Q appears in different chapters, compare the question text, diagrams, marks and covered parts. Merge only verified matches, do not double count a part, and record all source occurrences. Do not add omitted subparts or claim the subset is the full original exam. Keep the source map, demand evidence and uncertainties outside the import schema.

**TYS references for reflection.** When requested, choose **three distinct, verified TYS references per whole exam question**, focused on its main concept. Check the actual parts students will do and prerequisites, not just the chapter name. State a part range if only those parts fit. Respect the cohort's exclusions: for **2026 Sec 3 EYE A-Math**, exclude differentiation, integration, proofs in plane geometry, trigonometry and kinematics from the recommended practice. This is a practice filter for that cohort; tag assessed calculus or trigonometry normally on other papers. A-Math EYE output is the TYS-reference section only, with no “Practice Now” section. Use the existing reference notation, e.g. `N21/I/2` = November 2021 Paper 1 Q2. Flag a shortfall if fewer than three suitable verified matches exist; do not fill the list with unverified citations.

## 6. Produce the teacher review and coverage report

Default to a Markdown review for vetting if the user has not asked for immediate JSON. Use this table:

| Q / part | Marks | Main task | Primary SIO description (ID) | Secondary descriptions (IDs) | AO | Demand | Reason / flag |
| --- | ---: | --- | --- | --- | --- | --- | --- |
| 1(a) | 2 | Differentiate a product | Derivatives of products and quotients of functions (AM-63) | Derivatives of standard functions (AM-62), if useful for diagnosis | AO1 | Low | Direct application of the product rule. |

Use the catalogue's full description in the actual review, or give descriptions alone if the teacher asks to hide the codes. Include a short whole-question overview and list any uncertain parts separately. Give file outputs directly when requested; no HTML preview is required unless asked.

If asked what is **not tested**, compare the mathematical work with **every entry** in section 9, not just primary tags. Distinguish directly assessed, substantially embedded, partially covered, incidental only, not assessed and duplicate catalogue entry. For a broad SIO, name the subskills that did not occur. A provisional fallback, a calculator key, a method in an optional solution or a routine prerequisite does not by itself establish coverage. State what pages/parts the coverage report includes, and group missing outcomes by chapter with **description and ID**. Keep a duplicated row visible as a duplicate, not a second independent untested outcome.

## 7. Create the DMN Workspace JSON when requested

Use the exact shape below for the **DMN Workspace importer** (`dmn-math-package-v1`), unless the teacher supplies a newer working template. The older standalone reflection HTML embeds a different data array; a review JSON or a sidecar source map is also a different format. Do not present any of those as directly importable packages.

The example is illustrative, with one 6-mark question. Use verified paper metadata in a real package.

```json
{
  "format": "dmn-math-package-v1",
  "paper": {
    "title": "Example A-Math Paper 2 (one-question extract)",
    "subject": "amath",
    "year": 2026,
    "number": 2,
    "role": "bank",
    "totalMarks": 6
  },
  "questions": [
    {
      "qno": "1",
      "images": [],
      "parts": [
        {
          "label": "a",
          "maxMarks": 2,
          "sioId": "AM-63",
          "secondarySioIds": ["AM-62"],
          "ao": "AO1",
          "difficulty": "Low",
          "reviewed": false
        },
        {
          "label": "b",
          "maxMarks": 4,
          "sioId": "AM-68",
          "secondarySioIds": [],
          "ao": "AO2",
          "difficulty": "Moderate",
          "reviewed": false
        }
      ],
      "matchSioId": "AM-68",
      "answerText": ""
    }
  ]
}
```

- One package per paper or verified original year/paper group. `paper.role` is `bank` for practice sources and `reflection` for a paper students will reflect on. Use the teacher's intended role; do not use the two interchangeably.
- `qno` and `label` are strings. `maxMarks`, `totalMarks`, `year` and `number` are numbers. `totalMarks` equals the sum of the included `maxMarks`. Use the exact keys and the case-sensitive values `AO1`/`AO2`/`AO3` and `Low`/`Moderate`/`High`. Keep `secondarySioIds` as an array, even when empty.
- Keep `reviewed: false` until the teacher explicitly vets the tags for that part. Checking a scan, finding a solution, generating the JSON or applying a provisional fallback does not count as teacher approval.
- `images` holds real question image data URLs if screenshots are requested and available. Include complete question statements, all assigned parts and required diagrams in reading order. Exclude answers, unrelated questions and blank working space. Use `[]` for a tagging-only package when no images are required; do not fabricate image data. Keep `answerText` empty unless answers are requested and verified.
- Put display descriptions, reasons, source references and flags in the review or a sidecar; the import fields above carry the codes. If a blank tag is permitted, use `""` and explain it in the flags. If a required paper identifier cannot be verified, deliver the tags as a clearly labelled review and obtain the metadata before calling it ready to import. Do not invent a year or paper number to pass validation.
- If the user wants the legacy reflection HTML data, inspect the supplied HTML's embedded records and reproduce that schema instead. Do not edit or publish a site merely because JSON was requested.

## 8. Check before handing over

- Compare the inventory against every supplied page: no missing continuation, duplicate part, renumbered original reference or mark split. Confirm the question count, part count and included marks.
- Check every primary, secondary and whole-question match ID against the applicable A-Math catalogue. Check that primary choices fit the actual assessed skill and that alternative methods, errors and fallbacks are flagged.
- For topical TYS, independently reread the governing heading for each exercise and compare it with the output band **for every included part**. Check the original year/paper/Q reference against the print. A JSON-to-JSON comparison alone cannot catch a misread heading.
- Parse the final JSON and check required keys, types, allowed enum values, sum of marks, uniqueness of question/part pairs and review status. If adding image data, verify that it decodes and shows the right question. Say what was checked; do not claim a live import unless performed.
- Give a compact handover: files, counts, included marks and the specific items still needing review. Keep tagging, teacher approval, import and publication distinct.

## 9. Full A-Math SIO catalogue

The descriptions below are the display text in `reflection-amath.html` → `sio-catalog`. The source is the DMN TOS worksheet `(US) 4Exp AMath 4049 (2021)`. Topic codes are local catalogue groupings. **AM-70 is a repeated differentiation row** in the integration group: use AM-62 for standard differentiation and AM-69/71 as appropriate for integration; do not use AM-70 as a generic integration tag.

| SIO ID | Strand | Topic code | Catalogue chapter | SIO description |
| --- | --- | --- | --- | --- |
| AM-15 | ALG | A1 | Quadratic functions & equations | Finding the maximum or minimum value of a quadratic function using the method of completing the square |
| AM-16 | ALG | A1 | Quadratic functions & equations | Conditions for a quadratic expression to be always positive or always negative |
| AM-17 | ALG | A1 | Quadratic functions & equations | Using quadratic functions as models |
| AM-18 | ALG | A1 | Quadratic functions & equations | Conditions for a quadratic equation to have: (i) two real roots (ii) two equal roots (iii) no real roots and related conditions for a given line to: (i) intersect a given curve (ii) be a tangent to a given curve (iii) not intersect a given curve |
| AM-19 | ALG | A2 | Equations & inequalities | Solving simultaneous equations in two variables by substitution, with one of the equations being a linear equation |
| AM-20 | ALG | A2 | Equations & inequalities | Solving quadratic inequalities, and representing the solution on the number line |
| AM-21 | ALG | A3 | Surds | Four operations on surds, including rationalising the denominator |
| AM-22 | ALG | A3 | Surds | Solving equations involving surds |
| AM-23 | ALG | A4 | Polynomials & partial fractions | Multiplication and division of polynomials |
| AM-24 | ALG | A4 | Polynomials & partial fractions | Use of remainder and factor theorems, including factorising polynomials and solving cubic equations |
| AM-25 | ALG | A4 | Polynomials & partial fractions | Use of the sum and difference of cubes identities |
| AM-26 | ALG | A4 | Polynomials & partial fractions | Partial fractions (linear, repeated linear and irreducible quadratic factors) |
| AM-27 | ALG | A5 | Binomial theorem | Use of the Binomial Theorem for positive integer n |
| AM-28 | ALG | A5 | Binomial theorem | Use of factorial and binomial coefficient notation |
| AM-29 | ALG | A5 | Binomial theorem | Use of the general term in a binomial expansion |
| AM-30 | ALG | A6 | Exponential & logarithmic functions | Exponential and logarithmic functions and graphs, laws of logarithms, equivalence of exponential and logarithmic forms, and change of base |
| AM-31 | ALG | A6 | Exponential & logarithmic functions | Simplifying expressions and solving simple equations involving exponential and logarithmic functions |
| AM-32 | ALG | A6 | Exponential & logarithmic functions | Using exponential and logarithmic functions as models |
| AM-38 | G&T | G1 | Trigonometry | Six trigonometric functions for angles of any magnitude (in degrees or radians) |
| AM-39 | G&T | G1 | Trigonometry | Principal values of inverse trigonometric functions |
| AM-40 | G&T | G1 | Trigonometry | Exact values of trigonometric functions for special angles |
| AM-41 | G&T | G1 | Trigonometry | Amplitude, periodicity and symmetries related to sine and cosine functions |
| AM-42 | G&T | G1 | Trigonometry | Graphs of sine, cosine and tangent functions with amplitude, frequency and translation parameters |
| AM-43 | G&T | G1 | Trigonometry | Use of trigonometric identities, addition formulae, double-angle formulae and R formula |
| AM-44 | G&T | G1 | Trigonometry | Simplification of trigonometric expressions |
| AM-45 | G&T | G1 | Trigonometry | Solution of simple trigonometric equations in a given interval (excluding general solution) |
| AM-46 | G&T | G1 | Trigonometry | Proofs of simple trigonometric identities |
| AM-47 | G&T | G1 | Trigonometry | Using trigonometric functions as models |
| AM-48 | G&T | G2 | Coordinate geometry | Condition for two lines to be parallel or perpendicular |
| AM-49 | G&T | G2 | Coordinate geometry | Midpoint of line segment |
| AM-50 | G&T | G2 | Coordinate geometry | Area of rectilinear figure |
| AM-51 | G&T | G2 | Coordinate geometry | Equations of circles in centre-radius and general forms (excluding problems involving two circles) |
| AM-52 | G&T | G3 | Linear law | Transformation of relationships to linear form to determine unknown constants from a straight line graph |
| AM-53 | G&T | G4 | Plane geometry | Use of: - properties of parallel lines cut by a transversal, perpendicular and angle bisectors, triangles, special quadrilaterals and circles - congruent and similar triangles - midpoint theorem - tangent-chord theorem (alternate segment theorem) |
| AM-59 | CAL | C1 | Differentiation & applications | Derivative of f(x)as the gradient of the tangent to the graph of y=f(x)at a point |
| AM-60 | CAL | C1 | Differentiation & applications | Derivative as rate of change |
| AM-61 | CAL | C1 | Differentiation & applications | Use of standard differentiation notation |
| AM-62 | CAL | C1 | Differentiation & applications | Derivatives of powers, trigonometric, exponential and logarithmic functions, with constant multiples, sums and differences |
| AM-63 | CAL | C1 | Differentiation & applications | Derivatives of products and quotients of functions |
| AM-64 | CAL | C1 | Differentiation & applications | Use of Chain Rule |
| AM-65 | CAL | C1 | Differentiation & applications | Increasing and decreasing functions |
| AM-66 | CAL | C1 | Differentiation & applications | Stationary points (maximum and minimum turning points and stationary points of inflexion) |
| AM-67 | CAL | C1 | Differentiation & applications | Use of second derivative test to discriminate between maxima and minima |
| AM-68 | CAL | C1 | Differentiation & applications | Apply differentiation to gradients, tangents and normals, connected rates of change and maxima and minima problems |
| AM-69 | CAL | C2 | Integration & applications | Integration as the reverse of differentiation |
| AM-70 | CAL | C2 | Integration & applications | Derivatives of standard functions, with constant multiples, sums and differences (repeated entry in TOS) |
| AM-71 | CAL | C2 | Integration & applications | Integration of standard functions with linear arguments |
| AM-72 | CAL | C2 | Integration & applications | Definite integral as area under a curve |
| AM-73 | CAL | C2 | Integration & applications | Evaluation of definite integrals |
| AM-74 | CAL | C2 | Integration & applications | Finding the area of a region bounded by a curve and line(s) (excluding area of region between 2 curves) |
| AM-75 | CAL | C2 | Integration & applications | Finding areas of regions below the x-axis |
| AM-76 | CAL | C3 | Kinematics | Application of differentiation and integration to problems involving displacement, velocity and acceleration of a particle moving in a straight line |

## 10. Topical TYS chapter index

Use these as **chapter-level starting points**, then tag what each part actually assesses. These book chapter numbers are separate from the SIO IDs and topic codes above.

| TYS chapter | Main catalogue candidates |
| --- | --- |
| 1. Quadratic functions, equations and inequalities | AM-15–20 |
| 2. Surds | AM-21–22 |
| 3. Polynomials, cubic equations and partial fractions | AM-23–26 |
| 4. Binomial theorem | AM-27–29 |
| 5. Exponential and logarithmic functions | AM-30–32 |
| 6. Coordinate geometry | AM-48–51 |
| 7. Linear law | AM-52 |
| 8. Trigonometric functions and equations | AM-38–42, AM-45, AM-47 |
| 9. Trigonometric identities and formulae | AM-43–46; AM-38–40 or AM-47 where materially assessed |
| 10. Gradients, derivatives and differentiation techniques | AM-59–64 |
| 11. Applications of differentiation | AM-65–68; AM-59–64 if separately assessed or useful supporting work |
| 12. Differentiation of trigonometric, exponential and logarithmic functions and their applications | AM-62–68; distinguish derivative technique from application |
| 13. Integration | AM-69, AM-71, AM-73 as applicable |
| 14. Applications of integration | AM-72–75; AM-71 if an integration technique is substantively assessed |
| 15. Kinematics | AM-76; supporting differentiation/integration tags as warranted |
| 16. Proofs in plane geometry | AM-53 |

### Reference notes

- **SIOs and scope:** Project `reflection-amath.html` (52 entries), and `2020 G2 and G3 Additional Mathematics Syllabuses.pdf` (G3 content and section 6, Assessment Objectives). A newer supplied catalogue overrides the embedded snapshot.
- **AO and demand calibration:** `2022_DMN_AMath_P1_Tagging_Review.md`; SEAB, *Assessment in Singapore*, Volume 4, Chapter 6, printed pp. 40–48. Printed TYS bands take precedence for the topical collection.
- **Package structure:** Project `import-template (1).json` and the checked A-Math example `2024_DMN_AMath_P2_Prepared_Package.json`.
- **Coverage and practice examples:** `AMath_12_Questions_Tagging_and_Untested_SIOs.md` and `Amath_EYE_2026_Tagging_TYS_Review.md`. These are supporting references; the rules, catalogue and JSON example above are sufficient for use in another chat.
