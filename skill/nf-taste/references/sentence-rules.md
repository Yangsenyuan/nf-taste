# Sentence Rules

Scope: sentence length, voice, tense, information order, and hedging.
Derived from 7,205 sentences across 24 papers.

---

## RULE-SENT-001 — Keep the median sentence near 19–20 words

- Category: Sentence Rules
- Status: Confirmed
- Scope: all sections
- Rule: Target a median of 19–20 words per sentence. About 54% of corpus
  sentences are ≤20 words; only 7% exceed 40 words.
- Application: When a sentence passes 40 words, split it at the main contrast or
  the second verb. Do not split at a prepositional phrase.
- Precedence: this is a descriptive target, not a quota. Never add words,
  clauses, or filler to reach 19–20 words. An honest 14-word sentence beats a
  padded 19-word one; RULE-LANG-007 (no padding) wins.
- Evidence:
  - Corpus: median 19, mean 20.4
  - ≤10 words 23.3%; 11–20 31.1%; 21–30 26.0%; 31–40 12.7%; 41+ 7.0%
  - Section medians: Introduction 23, Discussion 23, Methods 20, Results 19,
    Conclusion 21
- Exceptions: A single long sentence is acceptable for a list of parallel
  conditions or a multi-part definition, if it stays readable.
- Confidence: High

## RULE-SENT-002 — Use sentence-initial "However," for the main contrast

- Category: Sentence Rules
- Status: Confirmed
- Scope: all sections
- Rule: Mark the pivot with a sentence-initial `However,` rather than burying the
  contrast mid-sentence with "but" or "while".
- Application: "The model performed well for fresh leaves, but failed for dry
  leaves" → "The model performed well for fresh leaves. However, it failed for
  dry leaves."
- Evidence:
  - "However" sentence-initial: 140 paragraphs / 24 papers
  - Examples: P01-ABS-P002, P01-INT-P005
- Exceptions: `while`/`whereas` are appropriate for a contrast inside one
  sentence when the two halves are parallel and short.
- Confidence: High

## RULE-SENT-003 — Passive voice belongs to procedures, not to claims

- Category: Sentence Rules
- Status: Contextual
- Scope: Methods strongly; Results moderately; Introduction and Conclusion rarely
- Rule: Use passive when the actor is the instrument or the procedure ("Spectra
  were collected...", "The model was calibrated..."). Use active `we` when the
  actor is the research team's decision or finding ("We evaluated...", "We found
  that...").
- Application: In Methods, passive is normal. In Discussion and Conclusion,
  convert "It was found that" to "We found that" unless the finding is the topic
  and the authors are irrelevant.
- Evidence:
  - Passive constructions: 921 paragraphs / 24 papers (heuristic: be + past
    participle)
  - `we` + past-tense research verb: 117 paragraphs / 22 papers
  - Examples: P01-MET-P012 ("we calculated the absorption coefficient...") vs
    P01-ABS-P002 ("...have been quantified from hyperspectral data")
- Exceptions: Journals with a strong active-voice house style.
- Confidence: High

## RULE-SENT-004 — Past tense for what was done, present tense for what is true

- Category: Sentence Rules
- Status: Confirmed
- Scope: all sections
- Rule: Methods and specific results use past tense. General truths, established
  mechanisms, and interpretation use present tense.
- Application: "The model estimated LAI with R² = 0.72" (past, specific result)
  vs "LAI is a key control on canopy conductance" (present, general truth).
  Discussion interpretation may use either, but must be consistent within a
  paragraph.
- Evidence:
  - Methods and Results are dominated by past-tense reporting verbs
  - Introduction and Discussion contain present-tense general claims
  - 117 paragraphs / 22 papers use `we` + past research verb
- Exceptions: Results stated as standing facts in some journals.
- Confidence: High

## RULE-SENT-005 — Hedge mechanisms, not measurements

- Category: Sentence Rules
- Status: Confirmed
- Scope: Discussion, Conclusion, Introduction
- Rule: Measurements and validated statistics are reported directly. Mechanisms
  and extrapolations take a hedge (`may`, `could`, `might`, `likely`,
  `suggests`).
- Application: "The model estimated protein with R² = 0.45" (no hedge) vs "The
  lower accuracy may be due to the limited spectral contrast of protein"
  (hedged).
- Evidence:
  - `may`: 147 paragraphs / 24 papers
  - `could`: 102 / 21
  - `likely`: 34 / 16
  - `might`: 9 / 6
  - Mechanism frames: 23 paragraphs / 13 papers
- Exceptions: When a mechanism was directly tested and confirmed, state it
  without a hedge.
- Confidence: High

## RULE-SENT-006 — Boost only what the data supports

- Category: Sentence Rules
- Status: Confirmed
- Scope: Results, Discussion
- Rule: `demonstrate`, `show`, `reveal`, `confirm` are common in this corpus, but
  they report observed results or prior findings — they are not a licence to
  overclaim. Do not use `demonstrate` for a mechanism you did not test.
- Application: Keep `demonstrated` for what the analysis establishes; use
  `suggest`/`indicate` for interpretation.
- Evidence:
  - `showed`: 129 paragraphs / 22 papers
  - `demonstrated`: 72 / 21
  - `revealed`: 22 / 10
  - `confirmed`: 15 / 8
  - Most occurrences sit in Results reporting or in Introduction summaries of
    prior work, not in speculative claims
- Exceptions: None. This is a scientific-integrity rule as well as a style rule.
- Confidence: High

## RULE-SENT-007 — "Significantly" requires a statistical test

- Category: Sentence Rules
- Status: Confirmed
- Scope: Results, Discussion
- Rule: Use `significantly` only when a statistical test supports it and the test
  or threshold is reported. Otherwise use "substantially", "considerably", or a
  number.
- Application: "significantly higher yield (p < 0.05)" is fine; "significantly
  improved accuracy" with no test is not.
- Evidence:
  - `significantly`: 43 paragraphs / 13 papers — a minority of papers, used with
    statistical context
  - `substantially`: 20 / 9; `considerably`: 4 / 4 are used for magnitude without
    statistical claim
- Exceptions: Quoting another study's stated significance.
- Confidence: High

## RULE-SENT-008 — Put the known information first, the new information last

- Category: Sentence Rules
- Status: Candidate
- Scope: all sections
- Rule: Begin with what the reader already has (the dataset, the previous
  finding) and end with the new element (the result, the interpretation). This is
  why so many sentences open with The/This/These.
- Application: "A higher accuracy was achieved by the recalibrated model" →
  "The recalibrated model achieved a higher accuracy."
- Evidence:
  - Sentence openings: `This/These` 304 paragraphs / 24 papers; `The` dominates
    Methods (82) and Results (50) paragraph openings
- Exceptions: Deliberate fronting for emphasis ("Of particular interest was...").
- Confidence: Medium
