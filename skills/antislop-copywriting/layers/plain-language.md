# Layer: plain language

Load in addition to `SKILL.md` **and** a register file. This is a constraint layer, not a register. It applies where the reader has no choice about reading, is under stress, is reading in a second language, or faces a consequence for misunderstanding: government forms and notices, health information, financial disclosures, safety instructions, consent screens, benefit and immigration guidance, and the explanatory text around a legal document.

**Provenance: convention, not corpus.** These rules come from plain-language practice. No corpus study of machine-written public-facing notices stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

Plain language is not simplification. It is the removal of everything between the reader and the action they must take, while every legal and factual obligation stays exactly as strong as it was.

## The boundary with legal text

CW-07 stands and this layer does not weaken it. Operative legal text (contract clauses, statutory wording, terms someone is agreeing to) is not rewritten here.

What this layer covers is the text around it: the summary, the notice, the consent screen, the instruction sheet, the explanation of what a clause means. Where a plain-language version sits next to operative text, it says which one governs.

Where a rewrite would change an obligation, a deadline, a right, or a liability, stop and mark it for the lawyer. That is a `[LEGAL REVIEW]` placeholder under CW-06, not a judgement call.

## Rules this layer changes

- **CW-25 synonym cycling is inverted.** One word per thing, every time. If it is a "claim" in paragraph one it is a "claim" in paragraph nine, never an "application" or a "request".
- **CW-30 actorless passive is tightened past the universal rule.** Every obligation names who must act. "The form must be submitted by 30 June" leaves the reader unsure whether that is their job.
- **CW-52 inline-header lists is suspended for definitions and for what-to-do lists**, where the header is the term or the situation.
- **CW-51 boldface is relaxed for the one fact that must not be missed**, usually a deadline or an amount. One per page. Bolding three things bolds nothing.
- **CW-22 fragments are allowed in numbered steps.** "Sign both copies." is a complete instruction.
- **CW-13 hedging is tightened.** A reader under stress reads "may be eligible" as "am I or not". Say what decides it.

## Sentence rules

- One idea per sentence. Target 15 to 20 words, and split anything past 25.
- Active voice with a named actor: "You must send the form" or "We will decide within 30 days".
- Present tense where it is true now.
- Second person for the reader, first person plural for the organisation. Not "the applicant" and "the Department".
- No double negatives. "Not ineligible" is a puzzle.
- Common words: *use* not *utilise*, *about* not *approximately*, *end* not *terminate*, *before* not *prior to*, *if* not *in the event that*, *must* not *shall*.
- Define a term at first use, in the sentence, not in a glossary the reader will not reach.
- Digits for numbers, including dates, amounts, and deadlines. Write the full year.

## Structure rules

- Put the action first. What the reader must do comes before the policy background that explains why.
- Group by the reader's situation, not by the organisation's departments.
- One page, one task, where the format allows it.
- Steps are numbered when order matters, and each step is one action.
- Say what happens if the reader does nothing, and say it plainly. This sentence is left out of almost every notice that needs it.
- Name where to get help, with a real channel and real hours.

## Example

Before:

> In the event that the requisite documentation is not received prior to the aforementioned deadline, the application may be subject to administrative closure without further notification.

After:

> Send your documents before 30 June 2026. If we do not have them by then, we will close your application. We will not contact you again first.

The rewrite names the actor, states the date, replaces three formal phrases with common ones, and answers the question the original avoided: what happens if the reader does nothing.

## Testing

- Read it aloud to someone in the situation it describes. Ask them what they have to do next and by when. If they cannot answer both, the text failed.
- A reading-level score is a rough check, not a pass. It counts syllables and cannot see that a sentence is ambiguous.
- Translation is a check as well as a deliverable: a sentence that cannot be translated cleanly was usually unclear in the source.

## Layer gate

Run after the universal gate and the register gate.

- [ ] No operative legal text was rewritten; anything that would change an obligation is marked `[LEGAL REVIEW]` (CW-07, CW-06)
- [ ] Every obligation names who must do it and by when (CW-30)
- [ ] One word per thing, throughout (CW-25 inverted)
- [ ] No sentence over 25 words; one idea each
- [ ] Every term defined at first use, in place
- [ ] Dates, amounts, and deadlines as digits, with the full year
- [ ] The consequence of doing nothing is stated
- [ ] A real help channel is named
- [ ] At most one bold fact per page (CW-51)
- [ ] A person in the reader's situation can say what to do and when, after one read
