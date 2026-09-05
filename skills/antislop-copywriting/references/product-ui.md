# Register: product UI microcopy

Load with `SKILL.md`. Covers button labels, form labels and helper text, error messages, empty states, loading states, confirmations, tooltips, toasts, notifications, onboarding, and permission prompts.

**Provenance: convention, not corpus.** These rules come from content design practice. The vocabulary rules this file cites are inherited from the corpus-grounded universal layer in `SKILL.md`; the register-specific pattern lists below are not, so treat their shapes as real and their frequencies as unmeasured. The same applies to every file in `references/` and `layers/`. No corpus study of machine-written microcopy stands behind them.

Microcopy is read by someone in the middle of doing something, often something that has just gone wrong. Every word costs the reader attention they were spending elsewhere. This register is where the universal rules bend the most, because brevity outranks nearly everything.

## What changes in this register

- **Sentence fragments are correct.** "Saved", "No results", "2 files selected". Fragments that would be CW-22 staccato in editorial are the right form here.
- **Repetition is correct.** A button labeled "Delete" in twelve places should say "Delete" in all twelve. CW-25 synonym cycling is a much more serious defect here than in prose, because inconsistent labels teach the user that two identical things are different.
- **Exclamation marks are mostly still wrong.** The CW-57 threshold is relaxed but the reasoning holds: a UI that celebrates every save is exhausting. Reserve them for genuine milestones, at most once per flow.
- **Voice runs quieter.** Personality in microcopy is a garnish and it goes stale on the hundredth reading. The user will see this string far more often than any landing page.

## Errors

The dominant AI failure here is apologising instead of informing.

An error message answers three things, in this order: **what happened, why, and what to do next.** Cut anything that is not one of those three.

Before:

> Oops! Something went wrong. Don't worry, our team is on it. Please try again later. Thanks for your patience!

Rules hit: CW-41 (chatbot reassurance), CW-57, and a total absence of information.

After:

> [State the actual failure and the actual next step. If the upload failed because the file is over the size limit: "This file is over the 10 MB limit. Try a smaller file." The source names no cause, so the cause must come from the code.]

The bracket is the point. "Something went wrong" is not a message, it is the absence of one, and no rewrite can invent the cause (CW-01). Read the error path in the code and say what it found.

Specific defects:

- **Blame reversal.** "You entered an invalid email." Prefer "This email address is missing an @." State the problem, not the user's failing.
- **Apology padding.** "We're sorry for the inconvenience." Fix the problem or explain it. The apology occupies the line the explanation needed.
- **Error codes alone.** "Error 0x8007" with no sentence. A code is for support, a sentence is for the user, ship both.
- **Reassurance without action.** "Don't worry" is CW-41. It asks the user to feel something instead of telling them what to do.

## Empty states

An empty state is the most-read screen a new user sees, and the one most often filled with encouragement instead of instruction.

It needs two things: **why it is empty, and the one action that fills it.**

Before:

> Nothing to see here! Get started by creating your first item. Let's go!

Rules hit: CW-57, CW-40, CW-41.

After:

> No projects yet. Create one to get started.

That rewrite adds no fact: "projects" replaces "item" only if the screen is the projects screen. If the object is unknown, keep the source's noun.

Distinguish the three empty states, because they need different words:

- **First run.** Nothing exists yet. Explain the object and offer the action.
- **Filtered to nothing.** Data exists but the filter excludes it. Say so, and offer to clear the filter. Telling a user with 400 records that they have none is a bug in the copy.
- **Cleared.** The user emptied it themselves. Confirm quietly, do not congratulate.

## Buttons and labels

- Label the verb, not the concept. "Save changes" beats "Submit". "Delete project" beats "Confirm".
- The button and the dialog must agree. A dialog asking "Delete this project?" with buttons "OK" and "Cancel" forces the user to re-read the question. Use "Delete" and "Keep".
- Never label a destructive action with a neutral word, and never make the destructive option the visually default one.
- Sentence case, not Title Case (CW-56).
- Do not put an ellipsis on a button unless it opens something that asks for more input. That convention is real and users rely on it.

## Confirmations and destructive actions

- Name the object and the consequence: "Delete 12 files permanently?" not "Are you sure?".
- Say whether it can be undone. If it cannot, say that plainly.
- Do not soften a destructive action with warmth. This is the one place where friendliness is a hazard.

## Loading and progress

- Prefer stating what is happening: "Uploading 3 of 12". A bare spinner with "Loading..." is acceptable but weaker.
- Do not write rotating jokes into a loader. They are funny once and irritating on the fourth wait, and they land badly when the operation is failing.
- Never claim progress you are not measuring. A progress bar that does not reflect real progress is CW-01 in visual form.

## Notifications and toasts

- One fact per toast.
- Include the object: "Invoice #1042 sent", not "Sent successfully".
- "Successfully" is almost always deletable. "Saved" already means it worked.

## Format defaults for this register

- Bold: essentially never. There is not enough text for emphasis to mean anything.
- Lists: only in longer helper text.
- Emoji: only where the product's design system already uses them deliberately, never as decoration in an error (CW-53).
- Em dashes: replace (CW-50). Microcopy has room for a period.
- Terminology: fixed. One word per concept across the whole product. Keep a list.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Every error names what happened and what to do next, with the cause read from the code, not guessed (CW-01)
- [ ] No apology, reassurance, or "don't worry" standing where information belongs (CW-41)
- [ ] Empty states distinguish first run from filtered-to-nothing
- [ ] Buttons name their verb and agree with the dialog that asks the question
- [ ] Destructive actions name the object, the consequence, and whether it is reversible
- [ ] One term per concept, used identically everywhere (CW-25 inverted: repetition required)
- [ ] No progress or status claim the code does not actually measure
- [ ] Read every string as if seeing it for the hundredth time. Nothing that would grate
