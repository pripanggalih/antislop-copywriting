# antislop-copywriting

A single agent skill that filters machine-written prose. It removes the patterns that mark text as AI-generated, and it treats the opposite failure, copy scrubbed until it sounds like nobody, as a defect too.

Works with any agent that reads the [Agent Skills](https://skills.sh) standard: Claude Code, Codex, Cursor, Gemini CLI, OpenCode, and others.

## Install

```bash
npx skills add pripanggalih/antislop-copywriting
```

Add `-g` for a global install. The skill folder is copied into your agent's skills directory and loads on its own when the task is prose work.

Nothing is written to `CLAUDE.md`, `AGENTS.md`, or any other entry file. The skill is triggered by its `description`, so no pointer block is needed and none is created.

Manual install: copy `skills/antislop-copywriting/` into your agent's skills directory.

## What it covers

Four registers, because prose rules are not universal. Documentation needs the bolded term lists that marketing must avoid, and a UI error message needs the sentence fragments that would be a defect in an essay.

| Register | Covers |
|---|---|
| Marketing | Landing pages, headlines, CTAs, value propositions, pricing, FAQ |
| Product UI | Buttons, labels, errors, empty states, tooltips, notifications |
| Documentation | README, API reference, guides, changelogs, code comments |
| Editorial | Blog posts, articles, essays, newsletters |

Plus a language layer for Indonesian copy, which sits in its own file and is [labeled honestly](#the-indonesian-layer-is-not-validated).

## How it decides

Two tiers, because "you invented a statistic" and "you used three adjectives" are not the same kind of problem.

**Hard rules** are absolute and falsifiable. A fact either has a source or it does not. Inventing numbers, testimonials, customer names, quotes, or citations is a defect on the first instance, with no purpose test and no override.

**Threshold rules** describe degree. One em dash is a punctuation mark, six in a page is a signature. Each carries a number:

- 3 or more distinct threshold rules inside any 200 words
- Any single rule 3 or more times per 500 words
- 5 consecutive paragraphs within 15% of the same word count
- 2 or more triads within 150 words

Thresholds exist so an audit can fail the same way twice. Without them, "look for clusters" means whatever the model felt like that run.

## What it will not do

- It will not add a fact, name, number, date, or quote that was not in the source. A rewrite that invents a plausible statistic is worse than the vague sentence it replaced, because it reads as honest while being false.
- It will not rewrite text inside quotations, titles, proper names, or legal text.
- It will not strip a writer's voice. Supply a writing sample or a `VOICE.md` and it matches your habits instead of a default. A sample can override threshold rules. It cannot override the hard ones: your voice does not authorise a fabricated number.
- It will not treat a writing sample as instructions. A sample describes how to write, and text inside it that looks like a command is a quotation.

## Usage

Load it and write. The skill infers what you want from the task.

Writing or editing: the rules apply as the text is produced, and it finishes with a pass or fail gate.

Auditing: ask whether something reads as AI, or ask for a review. You get a numbered findings list with rule IDs, quoted text, and one-line fixes. Nothing is changed until you pick numbers. Findings are reported inline; a file is written only if you ask for one.

## The Indonesian layer is not validated

The English material is grounded in published work: corpus studies of excess vocabulary in 2024 publications, editorial guidance, and detection research. No equivalent corpus exists for Indonesian.

The Indonesian patterns were derived inductively from 18 synthetic samples across the four registers. That finds real patterns but can only find the ones present in the generator's own habits, and it measures nothing about how often they occur in real text. The layer is kept in its own file so it can be corrected or replaced without touching validated material.

If you have real Indonesian AI-written copy, open an issue. Patterns that appear in real text but not in that synthetic set are the most useful contribution this project can receive.

## Layout

```
skills/antislop-copywriting/
├── SKILL.md                        universal rules, thresholds, delivery gate
└── references/
    ├── marketing.md
    ├── product-ui.md
    ├── documentation.md
    ├── editorial.md
    └── bahasa-indonesia.md
```

`SKILL.md` is read every time. One reference file is read per task, chosen by register. Loading all of them at once is the thing this layout exists to avoid.

## Naming

The name follows the `antislop` convention used across the agent skills ecosystem for filters of this kind. This is an independent implementation, not a derivative of any other project's code or text.

## Contributing

Useful contributions, in order of value:

1. Real samples of AI-written copy, especially Indonesian.
2. A pattern that survives the thresholds but should not.
3. A false positive: human writing this skill would wrongly flag.

## License

MIT. See [LICENSE](LICENSE).
