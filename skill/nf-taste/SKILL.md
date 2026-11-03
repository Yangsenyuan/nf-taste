---
name: nf-taste
description: Evidence-based SCI academic writing guidance and editing for vegetation remote sensing research. Use when planning an English research manuscript, organizing paragraphs or sections, translating Chinese scientific writing into English, or polishing/revising English academic text.
---

# NF-Taste

Writing rules distilled from 24 English SCI papers in vegetation remote sensing.
Every corpus-derived rule in `references/` carries counted evidence: how many
paragraphs and papers use the pattern, and which paragraph IDs it came from.
Rules drawn from general SCI convention are labelled `general convention` and
are never presented as corpus findings.

This is **not** a general English grammar checker and **not** an imitation of one
author's voice. It encodes what this research group's published papers
consistently do at the paragraph, sentence, section, and argument level.

## Rule status vocabulary

| Status | Meaning | How to use it |
|---|---|---|
| `Confirmed` | Repeated across ≥8 papers, no large body of counter-examples | Apply by default |
| `Candidate` | Repeated but concentrated in fewer papers or one section | Apply when context matches; say so |
| `Contextual` | Valid only in a named section or paragraph type | Check the section first |
| `Retired` | Observed once or contradicted | Do not apply |

Never present a `Candidate` or `Contextual` rule as a universal requirement.
When you apply a rule, you may cite it by ID (e.g. `RULE-SECT-002`).

## Step 1 — Identify the task

| User asks for | Task | Read first |
|---|---|---|
| Polish / revise / edit this English | `POLISH` | section + paragraph + sentence + language |
| Translate this Chinese into academic English | `C2E` | sentence + logical + language + terminology |
| Help plan a manuscript / storyline | `PLAN` | research-argument + section |
| Structure this Introduction / Discussion | `SECTION` | section + research-argument + logical |
| Draft a paragraph about ... | `PARA` | paragraph + sentence + logical |
| Describe this figure / result | `FIGURE` | figure-results + sentence + terminology |
| Deep revision / restructure | `DEEP` | paragraph + logical + section + research-argument |

When the user names a section, use it. When they do not, infer from the text
(tense, citation density, figure references) and state the inference once.
Do not ask for information the user already supplied.

Ambiguous drafts:

- A paragraph with Introduction moves **and** a reported statistic is most
  likely an Abstract. Apply `RULE-SECT-011`, say so, and do not force
  Introduction position rules onto it.
- A single paragraph cannot satisfy section-position rules (e.g. "aim at
  three-quarters of the Introduction"). Apply only the structural part and say
  which part was skipped.
- When several sections are plausible, choose the one that makes fewer rules
  applicable, and state the assumption.

## Step 2 — Load only what the task needs

Progressive disclosure: read the reference files for the task, not all of them.

- `references/section-rules.md` — Introduction / Methods / Results / Discussion / Conclusion
- `references/paragraph-rules.md` — paragraph length, topic sentence, closure
- `references/sentence-rules.md` — length, voice, tense, anaphora, hedging
- `references/logical-rules.md` — result vs interpretation, comparison, causal language
- `references/language-rules.md` — word choice, connectives, claims strength
- `references/research-argument-rules.md` — gap → aim → contribution chain
- `references/figure-results-rules.md` — figure/table description and statistics
- `references/rs-terminology.md` — vegetation remote sensing terms and collocations
- `references/corpus-evidence.md` — paper list, evidence format, confidence definitions

## Step 3 — Choose the editing mode

### English polishing

Default: **Adaptive Editing**.

| Mode | Behaviour |
|---|---|
| `Conservative` | Fix language only; keep sentence and paragraph structure |
| `Adaptive` (default) | Fix language; adjust sentence order and paragraph structure when the logic requires it; explain substantive changes |
| `Deep` | Restructure sentences, paragraphs, and argument order; never add unsupported science |

Escalate only when the problem requires it:

- grammar, spelling, punctuation, word choice → fix directly, no explanation needed
- sentence-level clarity or information order → rewrite the sentence
- paragraph logic (topic sentence, evidence order, closure) → restructure and explain
- argument-level gap → point it out and propose a plan; do not invent facts

### Chinese → English

Default: **Academic Translation**.

| Mode | Behaviour |
|---|---|
| `Faithful` | Preserve information and order |
| `Academic` (default) | Reorganise information to English SCI conventions without changing meaning |
| `Rewriting` | Larger restructuring; still no new results, mechanisms, or citations |

Translate the science, not the syntax. A Chinese sentence that stacks three
clauses should usually become two or three English sentences, not one long one.

## Step 4 — Write

Follow the rules for the identified section. Keep the user's data, units,
statistics, citations, study area, and model settings exactly as given.

## Step 5 — Output

Default shapes (see `assets/output-templates.md`):

- Polish → `## Revised Version` + `## Key Changes`
- C2E → `## Academic English Version` + `## Notes`
- Guidance → `## Recommended Structure` + `## Paragraph Functions` + `## Logical Connections` + `## Evidence Needed`

If the user asks for text only, return text only.

## Scientific integrity (non-negotiable)

1. Never change numbers, units, significance levels, sample sizes, data sources,
   model parameters, study areas, or reported results.
2. Never turn correlation into causation, or a possible mechanism into a
   demonstrated one.
3. Never invent citations, DOIs, data sources, or findings.
4. Never add a contribution the user did not make.
5. Keep terminology consistent; do not swap terms with different meanings for
   the sake of variation.
6. If the source has a scientific-logic problem, say so instead of polishing it
   into fluent nonsense.
7. When unsure about a term, method, or fact, keep the original and flag it.
8. Never claim "the advisor would write it this way". Say "this follows the
   corpus rule RULE-XXX, evidenced in Pxx-XXX-Pxxx".

**Precedence.** These constraints override scope and style rules. If a rule is
scoped to Results but applying it would prevent an unsupported claim, the
integrity constraint wins and the scope check is waived. When a style target and
a no-padding rule conflict, no-padding wins.

## When the corpus does not cover the case

The rules describe tendencies, not laws. If a rule does not fit:

- say which rule you considered and why it does not apply;
- fall back to general SCI writing conventions, explicitly labelled as
  `general convention`, not as a corpus finding.

## Evidence format

`P07-DIS-P003` means paper 07, Discussion, paragraph 3.
Counts are written as `N paragraphs / M papers`. A percentage without a
denominator is not acceptable evidence.
