# Register: correspondence

Load with `SKILL.md`. Covers email, cold outreach, follow-ups, replies, internal memos, announcements, status updates, meeting recaps, chat messages in Slack or Teams, and support replies written by a person.

**Provenance: convention, not corpus.** These rules come from business correspondence practice. No corpus study of machine-written email stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

Correspondence has a named sender and a named recipient who can answer back. That single fact changes the register: politeness formulas are function, not filler, and the reader is deciding within two seconds whether this needs them at all.

## Rules this register overrides

- **CW-41 chatbot closers is split, not suspended.** A sign-off is required in email. "Thanks" and "Let me know if that works" are correspondence, not artifacts. What stays a defect is the assistant voice pasted into a message: "I hope this helps", "Would you like me to expand on this?", "Feel free to reach out with any questions at all."
- **CW-44 summary padding is relaxed in a long thread.** One line at the top of a reply into a twenty-message thread ("Recapping where this landed:") is service to the reader.
- **CW-14 filler is narrowed.** "Thanks for the quick turnaround" is not filler. "I hope this email finds you well" is, and it marks the message as machine-written faster than any other sentence in this file.
- **CW-22 fragments are allowed in chat.** A Slack message can be three words. An email cannot be three words plus a subject line and nothing else.

## The first two lines

The reader sees a subject line and one preview line. Everything is decided there.

- **Subject.** Name the object and the ask. "Invoice 1042: needs your approval by Thursday" beats "Quick question". Never write "Touching base", "Following up", or "Checking in" as a subject: they name no object.
- **Lead with the ask, not the greeting run-up.** The pleasantry can stay, on its own line, but the first sentence of the body says what this is.

Before:

> I hope this email finds you well. I wanted to reach out to touch base regarding the project we discussed. As you may recall, we have been working diligently to move things forward, and I wanted to circle back to see if you had any thoughts.

Rules hit: CW-14, CW-40, CW-12, and four sentences containing no ask, no object, and no date.

After:

> Hi Ana. Can you approve the invoice by Thursday? [The source names no project, no invoice, and no deadline. Those come from the sender.]

## One message, one ask

A message with three asks gets one answered. Where three are genuinely needed, number them and put the deadline on each.

State the deadline as a date, never as "at your earliest convenience" or "ASAP". Both mean the sender did not want to say a date.

## Cold outreach

This is where CW-01 and CW-05 get broken most often, because personalisation is exactly the thing a model will invent.

- **Fabricated familiarity.** "I loved your recent post on scaling" when no post was read is a lie in the first sentence, and the recipient can check. If the research was not done, do not write the line.
- **Guessed pain.** "I know how hard it is to manage a team of your size" is CW-05: a guess in the grammar of fact.
- **The fake referral.** "A colleague suggested I reach out" without a nameable colleague is CW-04.
- **The invented compliment.** Generic praise reads worse than no praise.

Honest outreach says who you are, why this person specifically (with the real reason, or none), what you want, and how long it takes. Four sentences is a full cold email.

## Follow-ups

- Do not open with "Just circling back", "Bumping this to the top of your inbox", or "I wanted to follow up on my previous email". Repeat the ask and the deadline instead.
- Never claim a prior message was sent if it was not, and never invent what it said.
- Two follow-ups is the honest maximum before the answer is no.
- Do not manufacture urgency the sender does not have (CW-02).

## Replies

- Answer the question in the first line. Context after.
- Quote only the part being answered.
- Where the answer is no, write no. "Unfortunately at this time we are unable to accommodate" is three clauses of cushion around one word.

## Internal memos and status updates

- Name the actor in every sentence (CW-30). "The decision was made to postpone" hides who decided. Write "We postponed the launch. I made that call after the load test failed."
- Bad news goes first, in the subject line.
- A status update names what moved, what is stuck, and what you need from the reader. Anything else is a report nobody reads twice.
- Do not report progress that has not happened, and do not soften a slipped date into "on track with minor adjustments" (CW-01, CW-05).

## Support replies

Written by a person to a person, so the product UI rules do not apply directly. What carries over: state what happened, why, and what to do next.

What does not carry over: brevity outranking warmth. A support reply can apologise, once, for a real failure, and it should name the failure it is apologising for.

Never promise a fix date the team has not committed to.

## Chat versus email

Chat is a conversation. Do not write an email in it: no greeting paragraph, no sign-off, no "per my last message". Ask the thing.

Email is a record. It carries the subject, the object, the ask, and the date, because someone will search for it in six months.

## Format defaults for this register

- Bold: at most one span, on the deadline or the ask (CW-51).
- Lists: only where there are genuinely several items, and number them if each needs an answer.
- Emoji: match the thread's existing register, never in a first cold message (CW-53).
- Exclamation marks: at most one per message (CW-57).
- Em dashes: replace (CW-50).
- Length: an email past 200 words needs a reason. Chat past 60 words should be a call or a doc.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] The subject line names the object and the ask
- [ ] The first body sentence states why this message exists
- [ ] Exactly one ask, or numbered asks each carrying a date
- [ ] Every personal detail, referral, prior message, and compliment is real (CW-01, CW-04, CW-05)
- [ ] No "I hope this email finds you well", "circling back", "touching base", or "at your earliest convenience"
- [ ] No assistant voice: no "I hope this helps", no offer to expand (CW-41)
- [ ] Bad news is first and named, not softened into a schedule adjustment
- [ ] Every sentence about a decision names who made it (CW-30)
- [ ] No promised date the sender cannot keep
- [ ] Read it as the recipient at 8am with 40 unread. The ask is findable in two seconds
