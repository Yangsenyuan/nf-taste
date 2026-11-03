# Figure & Results Description Rules

Scope: how figures, tables, and numerical results are introduced and described
in the running text.

---

## RULE-FIG-001 — Point at the display item, then say what it shows

- Category: Figure & Results Description Rules
- Status: Confirmed
- Scope: Results
- Rule: Open with the figure/table reference and the finding it supports, in that
  order: `Fig. 3 shows ...`. Do not make the reader hunt for the figure number at
  the end of a long sentence.
- Application: "Fig. 3 shows that the recalibrated model reduced RMSE..." — not
  "The recalibrated model reduced RMSE ..., as can be seen in Fig. 3."
- Evidence:
  - Results paragraphs opening with Fig./Figure/Table: 93 paragraphs / 21 papers
  - 57 Results paragraphs open with "Fig.", 17 with "Table"
- Exceptions: A paragraph that synthesises several figures may name them in the
  second sentence.
- Confidence: High

## RULE-FIG-002 — Report the statistic with its unit and its comparison

- Category: Figure & Results Description Rules
- Status: Confirmed
- Scope: Results
- Rule: Every reported metric carries its value, its unit or scale, and the
  comparison that makes it meaningful (model vs model, fresh vs dry, site vs
  site).
- Application: "R² = 0.45 and RMSE = 3.16 × 10⁻⁴ g/cm² for protein, compared with
  R² = 0.40 for cellulose + lignin."
- Evidence:
  - Statistical reporting: 165 paragraphs / 22 papers
  - `R²` 382 occurrences / 22 papers; `RMSE` 166 / 20; validation 173 / 21
- Exceptions: When the statistic is repeated from a table and the comparison is
  already established in the previous sentence.
- Confidence: High

## RULE-FIG-003 — Describe the pattern before the numbers

- Category: Figure & Results Description Rules
- Status: Candidate
- Scope: Results
- Rule: State the direction and spatial/temporal pattern first, then give the
  numbers that support it. Do not walk through the figure point by point.
- Application: "Accuracy decreased from north to south (Fig. 4), with RMSE rising
  from 0.31 to 0.58." — not "At site 1 RMSE was 0.31, at site 2 it was 0.34...".
- Evidence:
  - Overall-trend language: 88 paragraphs / 19 papers
  - Spatial-pattern language: 62 paragraphs / 19 papers
  - Figure-anchored openings: 93 paragraphs / 21 papers
- Exceptions: A paragraph whose purpose is to report a table of per-class
  accuracy.
- Confidence: Medium

## RULE-FIG-004 — Use the figure to answer the research question

- Category: Figure & Results Description Rules
- Status: Confirmed
- Scope: Results, Discussion
- Rule: After describing what the figure shows, state what it means for the
  question — usually one sentence at the end of the paragraph.
- Application: Add a closing sentence: "This indicates that ..." or "This
  suggests that ...". Keep the interpretation modest.
- Evidence:
  - Discussion comparison language: 29 paragraphs / 12 papers
  - Mechanism language: 23 paragraphs / 13 papers
- Exceptions: Results that are purely descriptive (e.g. study-area maps).
- Confidence: High

## RULE-FIG-005 — Captions are self-contained and start with the item type

- Category: Figure & Results Description Rules
- Status: Confirmed
- Scope: figure/table captions
- Rule: Begin with `Fig. N.` or `Table N`, then a noun phrase naming what is
  shown, then the conditions (site, date, sensor, statistic). Define abbreviations
  used in the panel.
- Application: "Fig. 3. Correlation between measured and predicted foliar
  nitrogen for fresh (a) and dry (b) leaves across the seven sites."
- Evidence:
  - 167 captions indexed across 24 papers
  - Captions in the corpus consistently open with the item type and a noun phrase
- Exceptions: Journals with a separate caption style guide.
- Confidence: High

## RULE-FIG-006 — Do not repeat the table in prose

- Category: Figure & Results Description Rules
- Status: Candidate
- Scope: Results
- Rule: A table reports the full matrix; the text reports the comparison the
  reader needs. Do not restate every cell.
- Application: If the paragraph lists more than about five numbers from one
  table, convert it to a statement about the pattern plus two or three key values.
- Evidence:
  - Table-anchored openings: 17 paragraphs; figure-anchored 57 — the corpus
    relies more on figures than on table recitation
  - Overall-trend and spatial-pattern language show the preference for synthesis
    (88 and 62 paragraphs)
- Exceptions: Small tables where every value is the result.
- Confidence: Medium

## RULE-FIG-007 — Keep figure references consistent in form

- Category: Figure & Results Description Rules
- Status: Confirmed
- Scope: all sections
- Rule: Use one form throughout: `Fig. 3` or `Figure 3`, not both. Same for
  `Table 2` and `Eq. (1)`.
- Application: Check the target journal's style, then apply it uniformly,
  including in captions and in parentheses.
- Evidence:
  - The corpus uses `Fig.` in running text and `Fig. N.` in captions for most
    journals; MDPI papers use `Figure`
- Exceptions: Journal-specific style.
- Confidence: High
