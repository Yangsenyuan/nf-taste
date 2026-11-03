# Language Rules

Scope: word choice, claim strength, connectives, and terminology consistency.
Rules marked `general convention` are standard SCI practice, not corpus findings,
and must be labelled as such when cited.

---

## RULE-LANG-001 — Keep one term for one concept

- Category: Language Rules
- Status: Confirmed
- Scope: all sections
- Rule: Do not rotate synonyms for technical terms. `foliar nitrogen` stays
  `foliar nitrogen`; do not alternate with `leaf N`, `canopy nitrogen`, and
  `nitrogen content` unless they mean different quantities.
- Application: Before polishing, list the key terms and their definitions. If two
  terms refer to the same measured variable, pick one and use it throughout.
- Evidence:
  - The corpus maintains stable term sets across sections (e.g. `foliar` in 982
    occurrences across 18 papers; `canopy` 640 / 23; `spectral` 653 / 24)
  - Near-synonyms with distinct meanings are kept distinct in the terminology
    file (see `rs-terminology.md`)
- Exceptions: A synonym may be used to avoid repetition when the meaning is
  identical and the term is non-technical.
- Confidence: High

## RULE-LANG-002 — Hedge strength should match evidence strength

- Category: Language Rules
- Status: Confirmed
- Scope: Discussion, Conclusion
- Rule: Use a three-level scale: observed (`showed`, `was`) > supported
  inference (`indicates`, `suggests`) > speculation (`may`, `could`, `might`).
  Move down a level when the evidence is indirect.
- Application: A single-site regression supports "indicates"; a cross-site
  validation supports "shows"; an untested mechanism supports "may".
- Evidence:
  - `may` 147 paragraphs / 24 papers; `could` 102 / 21; `likely` 34 / 16;
    `might` 9 / 6
  - `suggested` 35 paragraphs / 14 papers; `suggest` 13 / 7; `suggests` 9 / 8
  - Boosters `showed` 129 / 22 and `demonstrated` 72 / 21 concentrate in Results
    and in summaries of prior work
- Exceptions: None. This is also a scientific-integrity rule.
- Confidence: High

## RULE-LANG-003 — Prefer the verb to the nominalisation

- Category: Language Rules
- Status: general convention
- Scope: all sections
- Rule: "We estimated biomass" beats "An estimation of biomass was performed".
  Nominalisations lengthen sentences and hide the actor.
- Application: Convert "the evaluation of the model performance was conducted" to
  "we evaluated model performance".
- Evidence: General SCI convention. Corpus sentences are short (median 19 words),
  which is consistent with verb-centred writing, but this rule was not separately
  counted.
- Exceptions: When the process itself is the topic ("Model inversion remains
  ill-posed").
- Confidence: n/a (general convention)

## RULE-LANG-004 — Use "significantly" only with a test

- Category: Language Rules
- Status: Confirmed
- Scope: Results, Discussion
- Rule: See RULE-SENT-007. `significantly` is a statistical claim, not a synonym
  for "substantially".
- Evidence: 43 paragraphs / 13 papers use it, generally with test context;
  `substantially` (20 / 9) and `considerably` (4 / 4) carry magnitude only.
- Confidence: High

## RULE-LANG-005 — Choose the connective by relation, not by habit

- Category: Language Rules
- Status: Confirmed
- Scope: all sections
- Rule: This corpus contrasts with `however` far more than it adds with
  `moreover`/`furthermore`. If a paragraph's logic is additive, prefer `in
  addition`; if inferential, `therefore`/`thus`.
- Evidence:
  - `however` 159 paragraphs / 24 papers
  - `therefore` 92 / 24
  - `in contrast` 72 / 20
  - `in addition` 57 / 21
  - `moreover` 26 / 14; `furthermore` 22 / 13
- Exceptions: None.
- Confidence: High

## RULE-LANG-006 — Name instruments, datasets, and products exactly

- Category: Language Rules
- Status: Confirmed
- Scope: Methods, Results
- Rule: Use the instrument/product name as the manufacturer and community use it
  (`HySpex VNIR-1600`, `Sentinel-2 MSI`, `NEON AOP`), with the spectral range or
  resolution where it matters for interpretation.
- Application: Do not write "a hyperspectral sensor" when the specific sensor
  determines the spectral resolution and therefore the result.
- Evidence:
  - Methods data-source markers: 79 paragraphs / 17 papers
  - Hyperspectral 189 occurrences / 19 papers; satellite 144 / 17
- Exceptions: When the sensor is genuinely generic in the argument.
- Confidence: High

## RULE-LANG-007 — Avoid empty academic padding

- Category: Language Rules
- Status: general convention
- Scope: all sections
- Rule: Delete "It is worth noting that", "It should be emphasized that",
  "In recent years, with the rapid development of...", and "plays an important
  role in" when they carry no information.
- Application: If removing the phrase does not change the meaning, remove it.
- Evidence: General convention; the corpus opens Introduction paragraphs on
  concrete field statements rather than on "in recent years" formulas
  (16/23 papers open on field importance).
- Exceptions: None.
- Confidence: n/a (general convention)

## RULE-LANG-008 — Do not upgrade the claim during polishing

- Category: Language Rules
- Status: Confirmed
- Scope: polishing tasks
- Rule: Polishing must not change epistemic strength. "May improve" must not
  become "improves"; "suggests" must not become "demonstrates".
- Application: Diff the draft against the revision for modal verbs and reporting
  verbs. Any change in strength must be flagged in `## Key Changes`.
- Evidence: Scientific-integrity constraint, consistent with the corpus's
  hedge/booster distribution (hedges 237 paragraphs; boosters concentrated in
  observation reporting).
- Exceptions: The user explicitly asks to strengthen a claim and supplies
  evidence.
- Confidence: High
