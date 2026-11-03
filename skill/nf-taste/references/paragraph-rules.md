# Paragraph Rules

Scope: how paragraphs are sized, opened, developed, and closed in this corpus.
Derived from 1,609 prose paragraphs across 24 papers.

---

## RULE-PARA-001 — One paragraph carries one analytical unit

- Category: Paragraph Rules
- Status: Confirmed
- Scope: all sections
- Rule: Each paragraph should make one point: one comparison, one mechanism, one
  dataset description, or one result block. If a paragraph contains two
  independent claims that do not share evidence, split it.
- Application: When revising, identify the paragraph's single claim in a phrase.
  If you cannot, split at the sentence where the subject changes.
- Evidence:
  - Corpus median paragraph: 88 words (p25 54, p75 138, p90 191)
  - Section medians: Introduction 107, Methods 71, Results 83, Discussion 113,
    Conclusion 76
- Exceptions: Methods paragraphs describing a multi-step procedure may run to
  150+ words when steps are sequential.
- Confidence: High

## RULE-PARA-002 — Paragraph length tracks the section's job

- Category: Paragraph Rules
- Status: Confirmed
- Scope: all sections
- Rule: Discussion and Introduction paragraphs run longest (median 107–114
  words); Methods is the shortest (median 71), then Conclusion (76); Results
  sits in between (median 83).
- Application: A 40-word Discussion paragraph usually lacks its mechanism or
  comparison; a 180-word Methods paragraph usually mixes two procedures.
- Evidence:
  - Introduction 107 (p25 64, p75 165)
  - Methods 71 (p25 44, p75 111)
  - Results 83 (p25 61, p75 117)
  - Discussion 113.5 (p25 72, p75 162)
  - Conclusion 75.5 (p25 40, p75 132)
- Confidence: High

## RULE-PARA-003 — Open with a sentence that announces the paragraph's job

- Category: Paragraph Rules
- Status: Confirmed
- Scope: all sections; strongest in Methods and Results
- Rule: The first sentence should state what the paragraph will establish, not
  begin with a data point that only makes sense after the second sentence.
- Application: If the opening sentence is a number or a citation, move the
  framing sentence in front of it.
- Evidence:
  - Methods paragraph openings: "The" 82, "We" 23, "In" 18, "For" 13
  - Results paragraph openings: "Fig." 57, "The" 50, "Table" 17
  - Discussion paragraph openings: "The" 41, "Fig." 27, "In" 11, "Our" 9
- Exceptions: Results paragraphs that intentionally lead with the figure when the
  figure itself is the topic of the paragraph.
- Confidence: High

## RULE-PARA-004 — "This/These" carry the previous sentence forward

- Category: Paragraph Rules
- Status: Confirmed
- Scope: all sections, especially Discussion
- Rule: Use `This`/`These` + noun (or alone) to link a sentence to the previous
  one, rather than repeating the full noun phrase.
- Application: Replace "The recalibrated PROSPECT model has higher accuracy. The
  recalibrated PROSPECT model also..." with "This recalibrated model also...".
  Make sure the referent is unambiguous.
- Evidence:
  - Sentences opening with This/These: 304 paragraphs / 24 papers
  - Examples: P01-RES-P008 ("This can provide information on identifying the
    sensitive bands..."); P01-DIS-P003 ("This holds promise for building a general
    model across a large variety of species...")
- Exceptions: Do not use bare `This` when two candidate referents exist in the
  previous sentence.
- Confidence: High

## RULE-PARA-005 — Close with the consequence, not with a new fact

- Category: Paragraph Rules
- Status: Candidate
- Scope: Introduction, Results, Discussion
- Rule: The final sentence should interpret, qualify, or transition — not
  introduce a new dataset or a new citation.
- Application: If the last sentence adds new evidence, either move it earlier or
  open a new paragraph.
- Evidence:
  - Discussion paragraphs frequently close on a hedge or implication
    (`may`, `could`, `holds promise`): 237 paragraphs / 24 papers contain
    may/might/could somewhere; closings concentrate them
  - Example: P01-DIS-P003 closing on "holds promise for building a general model"
- Exceptions: Results paragraphs that end on a reported statistic when the
  statistic is the point.
- Confidence: Medium

## RULE-PARA-006 — Methods paragraphs are procedural, not narrative

- Category: Paragraph Rules
- Status: Confirmed
- Scope: Methods
- Rule: Describe what was done in the order it was done, in past tense, with the
  instrument, dataset, or parameter named. Avoid justifying the method inside the
  procedure paragraph; justification belongs in the Discussion.
- Application: Convert "We thought it would be better to use PLSR because..."
  into the procedure plus, if needed, one citation supporting the choice.
- Evidence:
  - Methods contains the highest density of data-source (79 paragraphs / 17
    papers), preprocessing (77 / 22), modelling (163 / 22), and validation
    (110 / 22) markers
  - Methods median paragraph is the shortest of all sections (71 words)
- Exceptions: A short "rationale" sentence is acceptable when a non-standard
  choice would otherwise confuse the reader.
- Confidence: High

## RULE-PARA-007 — Do not stack citations without a claim

- Category: Paragraph Rules
- Status: Candidate
- Scope: Introduction, Discussion
- Rule: A sentence with citations should still assert something. Avoid
  "Several studies have investigated X (ref1; ref2; ref3; ref4)." with no
  statement of what they found or why it matters.
- Application: Turn citation lists into a claim plus examples: "Empirical models
  have been applied across species (ref1; ref2), but transferability remains
  limited (ref3)."
- Evidence:
  - Prior-work markers: 32 paragraphs / 17 papers
  - Gap markers follow prior-work sentences in the Introduction sequence
    (median position 0.32 vs 0.54)
- Exceptions: A deliberately compact literature-list sentence in a review.
- Confidence: Medium
