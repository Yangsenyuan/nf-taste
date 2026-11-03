# NF-Taste

A research-informed writing skill for vegetation remote sensing.

NF-Taste packages 54 writing rules, most distilled from 24 English SCI papers,
into a portable Agent Skill. It supports English polishing, Chinese → English
academic writing, and manuscript structure guidance.

## Download

- Website: https://nf-taste.vercel.app
- Skill package: [`nf-taste.zip`](nf-taste.zip)
- Source: [`skill/nf-taste/`](skill/nf-taste/)

## Install

```bash
# OpenAI Codex
cp -r nf-taste ~/.agents/skills/

# Claude Code
cp -r nf-taste ~/.claude/skills/
```

Unzip `nf-taste.zip` first, then run the command from the directory that contains
`nf-taste/`.

The package is plain Markdown. There is no runtime, no API key, and no build step.

## Contents

```
nf-taste/
├── SKILL.md
├── references/   9 rule files: paragraphs, sentences, logic, sections,
│                 language, research argument, figures, terminology, evidence
└── assets/       output templates
```

Every corpus-derived rule records its status, scope, exceptions, and the
paragraph IDs it came from. Rules drawn from general SCI convention are labelled
as such and are not presented as corpus findings.

## Website

`index.html` is a standalone page: fonts, the Skill ZIP, and font licences are
embedded. No CDN, no server, no analytics, no external asset requests.

The page has four full-screen sections, alternating warm white and black:
introduction and use cases; the corpus; the method; download.

## Corpus and privacy

The 24 source papers are **not** included in this repository or in the Skill
package. Only distilled rules, terminology notes, short illustrative examples,
and paper metadata are distributed.

## Prior art

NF-Taste studied, but did not copy, these projects:

- [writing-dna-skill](https://github.com/larashero3-dotcom/writing-dna-skill)
- [style-distiller](https://github.com/Guan-Yep/style-distiller)
- [academic-writing-dna-skill](https://github.com/yisyeasy-crypto/academic-writing-dna-skill)

## Typefaces

Instrument Serif (© The Instrument Serif Project Authors) and Inter
(© The Inter Project Authors), both under the SIL Open Font License 1.1. The
licence texts are embedded in `index.html`.
