# Register: personal and professional writing about a person

Load with `SKILL.md`. Covers cover letters, resume and CV summaries and bullets, LinkedIn About sections, speaker and author bios, About pages for an individual, personal statements, scholarship and admission essays, and artist statements.

**Provenance: convention, not corpus.** These rules come from hiring and admissions practice. No corpus study of machine-written application material stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

Two things make this register different from marketing, which it otherwise resembles. The subject is a real person who will be asked about every sentence in an interview, so a fabricated line is a lie they have to defend. And the sterile failure (CW-60) dominates here: the professional voice removes every detail that would distinguish one applicant from four hundred others.

## Rules this register overrides

- **CW-60 sterile default is the primary rule, not the backstop.** Copy that passes every other check and describes no identifiable person has failed. In this register the question "would this sentence be false about anyone else in the pile?" outranks every threshold.
- **CW-30 actorless passive is tightened.** The document exists to say who did what. "The migration was completed ahead of schedule" hides whether the writer led it, worked on it, or watched it.
- **CW-01 is tightened to metrics.** An invented percentage on a resume bullet is checkable, and it is checked. Where a number is not known, write the action without a number rather than a plausible figure.

## The trait-claim substitution

The dominant failure: a list of traits standing where evidence should be.

Before:

> I am a detail-oriented team player with a proven track record of delivering results in fast-paced environments. I am passionate about leveraging technology to drive meaningful impact.

Rules hit: CW-10 (proven, leveraging, meaningful, impact), CW-11, CW-20, CW-60, and no verifiable statement.

After:

> [Replace each trait with the thing that demonstrates it. If the source is a shipping record: "I rewrote our deploy script after the third failed release. Deploys went from a two-person job to one command."]

Test for every sentence: could a person who is the opposite of this claim write the same sentence? If yes, cut it. Nobody applies as a careless non-team-player, so "detail-oriented team player" carries no information.

Words to cut on sight in this register, on top of CW-10: *passionate about, results-driven, proven track record, dynamic professional, thrives in fast-paced environments, wearing many hats, go-getter, self-starter, think outside the box, synergy, hard-working and dedicated*.

## Resume bullets

The shape: verb, object, outcome. All three, with the outcome measured where a real measurement exists.

- Lead with the verb the person actually performed. "Led", "wrote", "shipped", "negotiated" are different claims. Choose the true one.
- One measured outcome beats three unmeasured ones.
- Where no number exists, name the concrete change instead: "took over an unowned service", "cut the release checklist from 40 steps to 12". Both are specific and both are checkable, which is the point.
- Do not inflate the role. "Led a team of 5" when the person was one of five is CW-01 and it ends at the reference check.
- Do not claim a team result as an individual one. Say what part was yours.

## Cover letters

- Delete "I am writing to express my interest in the position of X". The reader knows.
- The first paragraph names the specific reason this person and this role. If the writer cannot name one, the letter is not ready.
- The why-this-company paragraph must contain a fact about the company that could not be copied into another letter. If no real research was done, do not invent it (CW-05).
- Address a real problem the role exists to solve, and say what you would do in the first month.
- Three paragraphs is enough.

## Bios

- Third person, and the name goes first.
- One line on what they do now, one specific thing they have done, one way to reach them or find their work.
- No adjective stacks. A bio that calls someone "an accomplished and visionary leader" reads as written by them.
- Speaker bios: match the length the organiser asked for, exactly.
- Never award a title, a degree, a certification, or an affiliation the person does not hold (CW-01).

## Personal statements and application essays

- The tidy epiphany is the machine shape: an early hardship, a turning point, a lesson learned, a resolved present tense. Real experience is less symmetrical.
- Do not manufacture hardship, and do not sharpen a real one into a better story. Both are CW-01, and the second is worse because it uses something real.
- Unresolved tension is a signal of a human writer and it survives editing here. "I still do not know whether that was the right call" is a sentence a model rarely writes.
- The essay answers the prompt that was asked. A moving essay that answers a different prompt scores nothing.

## What not to scrub

This register loses the most from over-editing. Preserve, and argue for keeping:

- The odd specific detail: the exact machine, the strange first job, the number that is not round.
- Plain vocabulary where the writer's own vocabulary is plain.
- A sentence that admits a limit. It makes the rest believable.
- The writer's actual sentence rhythm, from a sample where one exists (see Voice in `SKILL.md`).

## Format defaults for this register

- Bold: on job titles and company names in a resume only (CW-51).
- Lists: resume bullets. Letters, bios, and essays are prose.
- Emoji: none, including in LinkedIn About sections.
- Exclamation marks: none.
- Em dashes: replace (CW-50), unless the person's own writing uses them.
- Length: bio under 100 words unless a length was set; cover letter under 400.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Every sentence would be false about most other applicants (the opposite test)
- [ ] No trait claim standing without the evidence that demonstrates it
- [ ] Every number, title, degree, date range, team size, and affiliation is real (CW-01)
- [ ] No team result presented as an individual one
- [ ] Every verb names what this person actually did (CW-30)
- [ ] The why-this-company paragraph contains a fact that could not be pasted into another letter
- [ ] No manufactured or sharpened hardship
- [ ] The specific, odd, hard-to-invent details survived editing (CW-60)
- [ ] No "passionate about", "results-driven", or "proven track record"
- [ ] The person could defend every sentence in an interview
