# Register: technical documentation

Load with `SKILL.md`. Covers README files, API reference, guides and tutorials, changelogs, migration notes, architecture documents, and prose inside code comments.

**Provenance: convention, not corpus.** These rules come from technical writing practice. The vocabulary rules this file cites are inherited from the corpus-grounded universal layer in `SKILL.md`; the register-specific pattern lists below are not, so treat their shapes as real and their frequencies as unmeasured. The same applies to every file in `references/` and `layers/`. No corpus study of machine-written documentation stands behind them.

Documentation is written to be searched, scanned, and abandoned the moment the reader has what they came for. Nobody reads it for pleasure and nobody reads it in order. That changes which universal rules apply.

## Rules this register overrides

These are deliberate reversals of the universal layer. Applying the universal rule here would make the document worse.

- **CW-52 inline-header lists is suspended.** `- **`timeout`:** milliseconds to wait before failing` is the correct form for a parameter list. The header is the lookup key, not a restatement. The pattern is a defect when the header restates the sentence after it, which in documentation means an entry like `- **Performance:** performance is better`.
- **CW-51 boldface overuse is relaxed.** Bold is how a scanning reader finds a term. Bold the term on first definition and in reference entries. It is still a defect when applied to ordinary words in running prose for emphasis.
- **CW-25 synonym cycling is inverted into a requirement.** One term per concept, forever. If it is a "workspace" in the installation guide it is not a "project" in the API reference. Documentation that rotates vocabulary is documentation that cannot be searched.
- **CW-20 rule of three is relaxed.** Three-item lists that reflect three real options are correct. The tell here is triads in the *prose*, not in genuine enumerations.
- **CW-56 Title Case** follows the project's existing heading convention. Consistency beats the preference.

Everything in the Hard tier still applies without exception, and applies harder. A fabricated flag, a plausible-looking parameter that does not exist, or an invented default value costs the reader a debugging session. This is the register where CW-01 does the most damage when broken.

## The dominant failure: describing instead of instructing

AI documentation narrates the existence of a feature rather than telling the reader how to use it.

Before:

> This powerful feature allows users to seamlessly configure their environment variables, providing a robust and flexible way to manage configuration across different deployment scenarios.

Rules hit: CW-10 (powerful, seamlessly, robust, flexible), CW-31 (the feature "allows" and "provides"), and a sentence that never says what to type.

After:

> Set environment variables in `.env`. [Show the actual syntax and the actual precedence rules from the source.]

The rewrite keeps only what the source supports. The original states no file name, no syntax, and no precedence, so an honest rewrite states none either and marks where the facts must come from. Read the implementation and fill the bracket from it.

## Documentation-specific defects

- **Restating the signature in prose.** "The `getUser` function gets a user." If the sentence adds nothing to the name, delete it and document the arguments, the return, and the failure modes instead.
- **Undocumented failure.** Happy path only. Every function that can fail needs its failure documented: what error, when, and what the caller should do. This is the single most common gap in machine-written documentation.
- **Invented defaults.** A default value that was never checked against the code is CW-01. Read the source, do not infer it from the parameter name.
- **Version-free instructions.** Steps that worked in one version and are silently wrong in the next. State the version the instructions apply to.
- **The tour.** "In this guide, we'll explore the fascinating world of authentication." CW-40. Start with the first step.
- **Prerequisite amnesia.** Step 1 assumes a running database that was never mentioned. List prerequisites before step 1, or the guide fails for everyone who is not the author.
- **Comment noise.** `// increment i` above `i++`. In code comments, document *why*, not *what*. The what is already in the line below.

## Changelogs

- One entry per user-visible change, written from the reader's position: what they can now do, or what will now break.
- "Various bug fixes and improvements" is an entry that says nothing. Name the fixes, or say the release contains internal changes only.
- Breaking changes go first and say exactly what breaks and what to do.
- Do not date-stamp a release with a date you are guessing at (CW-01).

## READMEs

The order that serves readers: **what it is, what it is for, how to install, the smallest working example, then everything else.**

- The first sentence states what the thing is in plain words. Not what it "empowers you to" do.
- The first code block must run as written, on a clean machine, with nothing implied.
- Do not include badges for services the project does not use.
- Do not write a "Features" section that is a triad of adjectives (CW-20, CW-10). List what it does.

## Format defaults for this register

- Bold: on defined terms and reference keys. Not in running prose.
- Lists: heavily, and correctly. Numbered for sequences, bulleted for sets.
- Code: every identifier, path, flag, and value in backticks. Every runnable example in a fenced block with the language tagged.
- Emoji: not in headings (CW-53). Emoji in a heading breaks anchor links and search in several documentation tools, so this one is a functional rule here, not a taste one.
- Em dashes: replace (CW-50).
- Tables: for reference data with consistent columns. Not for prose.
- Second person for instructions ("run", "set"), not first person plural ("we will now run").

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Every parameter, default value, flag, and return type was read from the source, not inferred (CW-01)
- [ ] Every failure mode a caller can hit is documented
- [ ] The first code example runs as written on a clean machine
- [ ] Prerequisites are listed before the first step
- [ ] One term per concept across the whole document set
- [ ] No sentence that only restates an identifier's name
- [ ] Changelog entries name what changed, from the reader's position
- [ ] The document answers the question a reader arrives with, in the first screen
