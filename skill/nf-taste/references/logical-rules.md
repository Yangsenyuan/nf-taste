# Logical Rules

Scope: how claims are connected to evidence, how results are separated from
interpretation, and how causal language is controlled.

---

## RULE-LOGIC-001 — Report the result before interpreting it

- Category: Logical Rules
- Status: Confirmed
- Scope: Results, Discussion
- Rule: In Results, state what was observed (direction, magnitude, metric,
  figure/table reference). In Discussion, interpret it. Do not put a mechanism
  inside a Results sentence.
- Application: Split "The model underestimated protein because protein absorption
  features are weak" into a Results sentence ("The model underestimated protein
  in fresh leaves") and, later in Discussion, the mechanism sentence.
- Evidence:
  - Results carries the statistical reporting load (165 paragraphs / 22 papers)
  - Mechanism language concentrates in Discussion (23 paragraphs / 13 papers)
  - Results paragraphs are anchored to figures/tables (93 paragraphs / 21 papers)
- Exceptions: Combined Results-and-Discussion sections interleave the two, but
  still at sentence boundaries.
- Confidence: High

## RULE-LOGIC-002 — Compare with the literature before explaining

- Category: Logical Rules
- Status: Confirmed
- Scope: Discussion
- Rule: For each main finding, first place it against published work
  (`consistent with`, `in contrast to`, `compared with`), then explain the
  agreement or difference.
- Application: A Discussion paragraph that only explains a mechanism, with no
  reference to what others found, reads as speculation. Add one comparison
  sentence.
- Evidence:
  - Comparison language: 29 paragraphs / 12 papers
  - Mechanism language: 23 paragraphs / 13 papers
  - `in contrast` 72 paragraphs / 20 papers; `whereas` 46 / 12
- Exceptions: A finding with no published counterpart may state that explicitly
  ("To our knowledge, no study has reported...").
- Confidence: High

## RULE-LOGIC-003 — Do not convert association into causation

- Category: Logical Rules
- Status: Confirmed
- Scope: all sections
- Rule: Correlational evidence supports "associated with", "related to",
  "covaries with", "explains part of the variance". Reserve "drives", "controls",
  "determines", "causes" for manipulative or mechanistic evidence.
- Application: Check every causal verb against the design. A regression between
  NDVI and GPP does not show that NDVI drives GPP.
- Evidence:
  - The corpus relies heavily on regression and retrieval (modelling markers in
    163 paragraphs / 22 papers) — most designs are observational
  - Hedged mechanism language (`may be attributed to`, `likely due to`) is the
    standard way of handling this (23 paragraphs / 13 papers)
- Exceptions: When citing an experimental study that established causation.
- Confidence: High

## RULE-LOGIC-004 — Move from the specific observation to the general implication

- Category: Logical Rules
- Status: Candidate
- Scope: Results paragraphs, Discussion paragraphs, Conclusion
- Rule: Within a paragraph, start with the specific result (dataset, site,
  metric), then generalise only as far as the evidence allows.
- Application: "At the seven sites, ..." → "Across the sampled gradient, ..." →
  "This suggests that ...". Do not jump from one site to a global claim.
- Evidence:
  - Results paragraphs open on figures/statistics (93 / 21), then use
    overall-trend language (88 / 19)
  - Conclusion adds implication language after restatement (11 paragraphs /
    9 papers)
- Exceptions: A paragraph whose entire purpose is the general claim.
- Confidence: Medium

## RULE-LOGIC-005 — Use concession to pre-empt the obvious objection

- Category: Logical Rules
- Status: Candidate
- Scope: Introduction, Discussion
- Rule: When a result is partly inconsistent with expectation, state the
  inconsistency in an `Although`/`While` clause and resolve it in the main clause,
  rather than hiding it.
- Application: "Although the accuracy was lower for dry leaves, the ranking of
  models was unchanged."
- Evidence:
  - `although`: 82 paragraphs / 23 papers
  - `while`: 167 paragraphs / 23 papers (includes temporal "while" uses)
  - Concessive openings appear in Discussion paragraph starts (Although 5 of the
    top Discussion openings)
- Exceptions: Overuse of concessive openings makes the Discussion defensive;
  use at most one per paragraph.
- Confidence: Medium

## RULE-LOGIC-006 — Keep the connective's meaning

- Category: Logical Rules
- Status: Confirmed
- Scope: all sections
- Rule: `therefore`/`thus` mark an inference; `moreover`/`furthermore`/`in
  addition` add a parallel point; `however`/`in contrast` mark a contrast;
  `whereas` compares two clauses inside one sentence. Do not use them as generic
  glue.
- Application: If two sentences are merely sequential, use no connective or
  "then". If the second does not follow logically from the first, `therefore` is
  wrong.
- Evidence:
  - `however`: 159 paragraphs / 24 papers
  - `therefore`: 92 / 24
  - `in contrast`: 72 / 20
  - `in addition`: 57 / 21
  - `moreover`: 26 / 14; `furthermore`: 22 / 13 (both far less frequent than
    however/therefore)
- Exceptions: None.
- Confidence: High

## RULE-LOGIC-007 — One argument chain per Discussion subsection

- Category: Logical Rules
- Status: Candidate
- Scope: Discussion
- Rule: A Discussion subsection should run: finding → comparison → mechanism →
  qualification. If a paragraph starts a new chain, it belongs in a new
  subsection.
- Application: Check that the last sentence of each paragraph either closes the
  chain or hands over to the next.
- Evidence:
  - Discussion paragraphs are the longest (median 113.5 words), consistent with
    multi-step chains
  - Comparison and mechanism language co-occur across 12–13 papers
- Exceptions: Short Discussions in letters.
- Confidence: Medium
