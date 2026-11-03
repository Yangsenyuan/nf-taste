# Section Rules

Scope: how each section of an English vegetation remote sensing research article
is organised in this corpus. Apply after identifying the section; do not apply a
Results rule to a Discussion paragraph.

Evidence format: `N paragraphs / M papers`, plus paragraph IDs.
Confidence: `Confirmed` (≥8 papers, few counter-examples), `Candidate` (repeated but
concentrated), `Contextual` (only in a named section), `Retired`.

---

## RULE-SECT-001 — Introduction follows a four-move sequence

- Category: Section Rules
- Status: Confirmed
- Scope: Introduction
- Rule: Order the Introduction as **field importance → prior work → specific gap →
  aim**. Measured as median relative sentence position across the whole
  Introduction: importance 0.04, prior work 0.32, gap 0.54, aim 0.75.
- Rationale: Readers need the field's stake before they can judge the gap; the gap
  must precede the aim, otherwise the aim reads as unmotivated.
- Application: When drafting or restructuring an Introduction, place the gap
  statement in the last third and the aim after it. Do not open with the gap.
- Evidence:
  - Importance markers: 16 papers, median position 0.04 (e.g. P03-INT-P001,
    P04-INT-P007)
  - Prior-work markers: 18 papers, median position 0.32
  - Gap markers: 13 papers, median position 0.54
  - Aim markers: 16 papers, median position 0.75
  - Gap precedes aim in 8 of the 9 papers where both are detectable
- Exceptions: Short "letter"-style Introductions may compress to three moves
  (importance + gap + aim).
- Confidence: High

## RULE-SECT-002 — The aim is stated before the end, not in the final sentence

- Category: Section Rules
- Status: Confirmed
- Scope: Introduction
- Rule: State the aim at roughly three-quarters of the Introduction, then use the
  remaining sentences for approach, scope, or contribution. Do not save the aim
  for the last sentence.
- Rationale: The final sentences carry the study's positioning; ending on the aim
  leaves the contribution unstated.
- Application: If the draft ends with "The aim of this study was to...", move the
  aim earlier and add one or two sentences on approach/contribution after it.
  Keep the aim in its own sentence so it can be found; do not fold it into the
  gap sentence with "therefore". On a one-paragraph draft, apply only the
  "aim is not the final sentence" part — the three-quarters position cannot be
  measured within a single paragraph.
- Evidence:
  - 16/23 papers contain an explicit aim marker
  - Only 7/23 place it in the final paragraph
  - Explicit aim frames: "the aim/objective/goal/purpose of this study" (20
    paragraphs / 15 papers), "here we" (5/5), "we aim to" (5/5), "this study
    aims" (7 paragraphs / 6 papers)
- Exceptions: Papers whose Introduction ends with a numbered contribution list.
- Confidence: High

## RULE-SECT-003 — The gap is stated with "However" plus a specific limitation

- Category: Section Rules
- Status: Confirmed
- Scope: Introduction; also Discussion when comparing with prior work
- Rule: Introduce the gap with a sentence-initial `However,` and name the
  limitation precisely (species, sensor, scale, transferability, or method), not
  vaguely ("limited research").
- Rationale: A named limitation is checkable; a vague gap reads as boilerplate.
- Application: Replace "However, few studies have focused on X" with the specific
  constraint, e.g. "However, these relationships proved difficult to transfer
  across species or sites."
- Evidence:
  - Sentence-initial "However": 140 paragraphs / 24 papers
  - Explicit gap markers: 49 paragraphs / 20 papers
  - `few studies`: 10 paragraphs / 8 papers; `has not been`: 12 / 9;
    `remains challenging`: 6 / 5
  - Example: P01-INT-P005 ("However, it proved difficult to transfer the empirical
    relationships across species or sites"); P01-INT-P015 ("However, to our
    knowledge, the newly proposed algorithm has not been evaluated for...")
- Exceptions: `However` may also mark a local contrast inside a paragraph; this
  rule concerns the gap move.
- When the author supplies no specific limitation: keep their wording, flag the
  gap as unresolved, and ask for the specific constraint. Never invent a
  limitation to satisfy this rule.
- Confidence: High

## RULE-SECT-004 — Introduction opens on the field, not on the study

- Category: Section Rules
- Status: Confirmed
- Scope: Introduction, first paragraph
- Rule: Open with what the field studies and why it matters, in one or two
  sentences, before any site, sensor, or dataset is named.
- Application: The first paragraph should be readable without knowing the study
  area. Move any site-specific sentence later.
- Evidence:
  - 16/23 papers state field importance in the first paragraph
  - 11 paragraphs / 10 papers use the explicit frame "X is/are critical /
    important / essential / central for ..."
  - Examples: P03-INT-P001, P04-INT-P007
- Exceptions: Methodological papers may open on the method's limitation.
- Confidence: High

## RULE-SECT-005 — Methods runs from setting and data to analysis, and usually closes with evaluation

- Category: Section Rules
- Status: Candidate
- Scope: Materials and Methods
- Rule: Order subsections as **study area / field data → remote sensing or
  spectral data → preprocessing → modelling → evaluation**. A dedicated
  "Model evaluation" or "Validation" subsection at the end is common but not
  universal (9/23 papers).
- Application: When restructuring Methods, keep data description before
  modelling, and put evaluation metrics and validation design after the model.
- Evidence:
  - Study area/site markers: 12 papers, median relative position 0.00
  - Data/sensor markers: 18 papers, median position 0.07
  - Modelling markers: 23 papers, median position 0.20
  - Validation markers: 21 papers, median position 0.24
  - Preprocessing markers: 10 papers, median position 0.35 (often a separate
    subsection after data description)
  - Final subsection named evaluation/validation/accuracy: 9/23 papers
    (P01, P04, P05, P06, P13, P18, P21, P22, P24)
- Exceptions: Papers that organise Methods by analysis step rather than by data
  source (e.g. P22, direct vs indirect inversion).
- Confidence: Medium

## RULE-SECT-006 — Results paragraphs are anchored to a figure or table

- Category: Section Rules
- Status: Confirmed
- Scope: Results
- Rule: Most Results paragraphs begin by pointing at the display item they
  interpret (`Fig. 3 shows...`, `Table 2 reports...`) or by stating the overall
  pattern the item reveals.
- Application: Do not write a Results paragraph with no figure/table anchor
  unless it reports a numerical result that has no display item.
- Evidence:
  - Paragraphs opening with `Fig.` / `Figure` / `Table`: 93 paragraphs / 21 papers
  - Statistical reporting (R², RMSE, MAE, p): 165 paragraphs / 22 papers
  - Overall-trend language: 88 paragraphs / 19 papers
  - Spatial-pattern language: 62 paragraphs / 19 papers
- Exceptions: Results sections that are purely tabular in supplementary material.
- Confidence: High

## RULE-SECT-007 — Discussion compares before it explains

- Category: Section Rules
- Status: Confirmed
- Scope: Discussion
- Rule: Establish agreement or disagreement with published work first, then offer
  a mechanism. Comparison without a mechanism is acceptable; a mechanism without
  comparison reads as speculation.
- Application: For each main finding, write one comparison sentence
  (`consistent with`, `in contrast to`, `compared with`) and then, if evidence
  allows, one mechanism sentence (`may be attributed to`, `likely due to`).
- Evidence:
  - Comparison language: 29 paragraphs / 12 papers
  - Mechanism language: 23 paragraphs / 13 papers
  - Examples: P04-DIS-P001 (comparison), P05-DIS-P019 (mechanism)
- Exceptions: Purely methodological Discussions may compare metrics rather than
  ecological findings.
- Confidence: High

## RULE-SECT-008 — Limitations are brief and local, not a separate essay

- Category: Section Rules
- Status: Confirmed
- Scope: Discussion
- Rule: State a limitation in one or two sentences, tied to a specific result,
  using a hedge (`may`, `could`) and, where relevant, a forward pointer. Do not
  build a standalone "Limitations" subsection unless the journal requires it.
- Rationale: Only 12 paragraphs in 7 of 24 papers contain explicit limitation
  language; the corpus treats limitations as part of the argument, not a section.
- Application: Convert a generic limitations paragraph into one sentence attached
  to the affected finding, e.g. "This may be due to the limitation of the
  PROSPECT model for dry leaves, which does not consider inter-correlations
  between parameters."
- Evidence:
  - Limitation/uncertainty language: 12 paragraphs / 7 papers
  - Example: P01-DIS-P005; P04-DIS-P006 ("However, some caution is called for
    when doing so.")
- Exceptions: Review articles and papers with a dedicated uncertainty section.
- Confidence: High

## RULE-SECT-009 — Conclusion restates findings and adds implications, never new results

- Category: Section Rules
- Status: Confirmed
- Scope: Conclusion
- Rule: Open with what was done and found, then state implications or
  applicability, and optionally one forward-looking sentence. Do not introduce a
  result that was not in Results.
- Application: Keep the Conclusion to roughly 40–130 words (corpus median 75.5).
  If a number appears, it must already appear in Results.
- Evidence:
  - Restatement verbs (`we found/showed/demonstrated`, `this study provides`):
    6 paragraphs / 6 papers
  - Implication/application language: 11 paragraphs / 9 papers
  - Forward-looking language: 4 paragraphs / 4 papers
  - Conclusion paragraph length: median 75.5 words (p25 40, p75 132)
- Exceptions: Journals that merge Results and Discussion often merge Conclusion
  into Discussion as a final paragraph.
- Confidence: High

## RULE-SECT-010 — Respect the paper's actual section combination

- Category: Section Rules
- Status: Confirmed
- Scope: all
- Rule: If the source or target journal uses `Results and Discussion`, do not
  split it into two sections. If Methods is called `Data and Methods`, keep that.
- Application: Section rules describe functions, not required headings. Match the
  target journal's headings.
- Evidence:
  - 3/24 papers use a combined `Results and Discussion` section
  - 13/24 use `Materials and Methods`; others use `Methods`, `Data and Methods`,
    or `Methodology`
- Confidence: High

## RULE-SECT-011 — Abstract: context → aim → result → implication

- Category: Section Rules
- Status: Candidate
- Scope: Abstract
- Rule: Move from context/gap, to what was done, to the key quantitative result,
  to what it implies. Report at least one number; hedge the implication.
- Application: A draft abstract that only describes what was done, with no
  result, is incomplete. One result sentence and one implication sentence are
  usually enough.
- Evidence:
  - 23 abstracts (one per paper), median 281 words
  - Gap/context language: 15/23
  - Explicit aim or "we investigated/evaluated/assessed": 10/23
  - Quantitative result (R², RMSE, MAE, accuracy, %): 15/23
  - Implication or applicability: 13/23
  - Contains digits: 22/23
  - Abstract sentence length: median 22 words
- Exceptions: Structured abstracts (Background/Methods/Results/Conclusions) follow
  the journal's headings instead.
- Confidence: Medium
