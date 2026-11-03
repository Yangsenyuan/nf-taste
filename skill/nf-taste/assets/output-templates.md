# Output Templates

Use these shapes by default. If the user asks for text only, return only the
text — no headings, no commentary.

---

## English polishing

```markdown
## Revised Version
[revised English]

## Key Changes
- [what changed and why it matters]
- [substantive changes only; omit pure grammar fixes]

## Unresolved
- [only if present: a rule the draft cannot satisfy without information the
  author has not supplied — say which rule and what is missing]
```

Omit `## Unresolved` when everything was resolvable. Never invent content to
empty this section.

Rules for `Key Changes`:

- List only changes a reader could disagree with: sentence order, paragraph
  split/merge, claim strength, terminology choice.
- Do not list spelling or punctuation fixes.
- If a claim was weakened or strengthened, say so explicitly and why.

---

## Chinese → English

```markdown
## Academic English Version
[English text]

## Notes
- [term choice and why]
- [logic that was reordered]
- [places where the Chinese source was ambiguous and the original phrasing was
  kept]
```

Do not pad `Notes` with grammar commentary. Three bullets is usually enough.

---

## Writing guidance / manuscript planning

```markdown
## Recommended Structure
[section or paragraph plan, in order]

## Paragraph Functions
1. [paragraph task — one line each]
2. ...

## Logical Connections
- [how paragraph N hands over to paragraph N+1]

## Evidence Needed
- [data, literature, or analysis the author still needs to supply]
```

`Evidence Needed` must be honest: if the storyline requires a comparison the
author has not run, say so rather than writing the sentence.

---

## Section outline (Introduction example)

```markdown
## Introduction Outline

| # | Function | Content to include | Rule |
|---|---|---|---|
| 1 | Field importance | why this trait / process matters | RULE-SECT-004 |
| 2 | Prior work | what has been done, by approach | RULE-SECT-001 |
| 3 | Gap | the specific limitation | RULE-SECT-003 |
| 4 | Aim + approach | what this study does, how | RULE-SECT-002 |
| 5 | Contribution | what it adds | RULE-ARG-003 |
```

Adapt to the target journal. Do not force five paragraphs if the paper needs
seven.

---

## Figure / result description

```markdown
## Description
[pattern first, then the key statistic, then the figure reference]

## Interpretation
[one or two sentences, hedged to match the evidence]
```

---

## Revision report (for a full section)

```markdown
## Revised Version
[full revised text]

## Structural Changes
- [paragraph moved / split / merged]

## Claim-Level Changes
- [any change in modal strength or causal language]

## Unresolved
- [scientific issues that need the author's data or decision]
```

---

## What never goes in the output

- Invented citations, DOIs, or data sources.
- New numbers or units.
- "The advisor would write..." — cite `RULE-XXX` and the paragraph ID instead.
- Praise for the draft. The user wants the text, not a review.
