# Research Argument Rules

Scope: the overall chain that makes the paper necessary — background → gap →
aim → method → finding → significance — and how a remote sensing method is tied
to a vegetation/ecological question.

---

## RULE-ARG-001 — The gap must be a consequence of the background, not an announcement

- Category: Research Argument Rules
- Status: Confirmed
- Scope: Introduction
- Rule: The gap should read as what the reviewed work cannot yet do, not as a
  free-standing statement that research is needed.
- Application: Before writing the gap sentence, state what prior work achieved
  and where it stopped. The gap sentence then names the specific missing
  capability.
- Evidence:
  - Prior-work markers appear before gap markers in the Introduction sequence
    (median position 0.32 vs 0.54; 18 and 13 papers respectively)
  - Gap precedes aim in 8/9 papers where both are detectable
  - Example chain: P01-INT-P005 (transfer difficulty) → P01-INT-P012 (retrieval
    remains challenging) → aim
- Exceptions: Papers that open with a methodological limitation.
- Confidence: High

## RULE-ARG-002 — State the aim as an action, not as a topic

- Category: Research Argument Rules
- Status: Confirmed
- Scope: Introduction
- Rule: Prefer "we evaluated / assessed / developed / quantified X" over "this
  paper is about X". The aim should name the object (trait, scale, sensor) and
  the operation (estimate, map, transfer, validate).
- Application: Replace "This study focuses on foliar nitrogen estimation" with
  "We evaluated whether canopy reflectance can retrieve foliar nitrogen across
  species".
- Evidence:
  - Aim frames: "in this study" 108 paragraphs / 21 papers; `we evaluated` 12 /
    8; `we investigated` 9 / 9; `we assessed` 7 / 4; `we developed` 6 / 4;
    `here we` 5 / 5
  - Explicit aim nouns ("aim/objective/goal/purpose"): 20 paragraphs / 15 papers
- Exceptions: Review articles, where the aim is to synthesise.
- Confidence: High

## RULE-ARG-003 — Name the contribution once, explicitly

- Category: Research Argument Rules
- Status: Candidate
- Scope: Introduction end, Conclusion
- Rule: State what the paper adds in one sentence, using a contribution frame,
  rather than letting the reader infer it from the aim.
- Application: "This study provides a template for characterising key foliar
  functional traits..." or "Our results demonstrate that...".
- Evidence:
  - Contribution frames: `our results` 32 paragraphs / 17 papers; `results
    showed` 13 / 11; `these findings` 9 / 7; `these results` 8 / 6;
    `results indicate` 6 / 6
  - Example: P07-CON-P002 ("This study provides a template for characterizing
    key foliar functional traits...")
- Exceptions: Very short papers where the aim already states the contribution.
- Confidence: Medium

## RULE-ARG-004 — Connect the sensor/method to the ecological quantity

- Category: Research Argument Rules
- Status: Confirmed
- Scope: Introduction, Discussion
- Rule: A remote sensing paper must say what vegetation quantity the signal
  stands for and why that quantity matters. Do not stop at "hyperspectral data
  can estimate X"; explain what X controls or indicates.
- Application: Every methods-driven paragraph should have one sentence linking
  the spectral variable to a physiological or ecological process.
- Evidence:
  - Field-importance openings in 16/23 Introductions
  - Mechanism language in Discussion: 23 paragraphs / 13 papers
  - Trait/process vocabulary: foliar 982 occurrences / 18 papers; canopy 640 / 23;
    chlorophyll 277 / 21; nitrogen 645 / 19
- Exceptions: Pure sensor-comparison papers.
- Confidence: High

## RULE-ARG-005 — Scale claims must match the sampling design

- Category: Research Argument Rules
- Status: Confirmed
- Scope: Discussion, Conclusion
- Rule: If the study sampled plots or sites, the conclusion is about those plots
  or that gradient. Global or operational claims require explicit extrapolation
  language and a stated limitation.
- Application: "Across the seven Arctic sites" not "across the Arctic"; "for the
  cultivars tested" not "for maize".
- Evidence:
  - Study-area/field-sampling subsections are the first Methods subsection in
    12 papers
  - Limitation language is brief and tied to a specific result (12 paragraphs /
    7 papers)
- Exceptions: Studies with a formal upscaling or global validation component.
- Confidence: High

## RULE-ARG-006 — Separate method novelty from scientific novelty

- Category: Research Argument Rules
- Status: Candidate
- Scope: Introduction, Discussion
- Rule: If the contribution is a method (e.g. transfer learning, a new inversion
  scheme), say what scientific question the method now makes answerable. If the
  contribution is scientific, say what method limitation it overcomes.
- Application: Add one sentence after the aim: "This makes it possible to ..." or
  "This overcomes the need for ...".
- Evidence:
  - Method-oriented papers in the corpus (P14 transfer learning, P19 hybrid
    inversion) frame the method as a route to transferability
  - Contribution frames appear in 17 papers
- Exceptions: Pure benchmark papers.
- Confidence: Medium
