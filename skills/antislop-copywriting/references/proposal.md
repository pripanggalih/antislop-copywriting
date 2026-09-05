# Register: proposals and decision documents

Load with `SKILL.md`. Covers client proposals, RFP and tender responses, pitch decks, executive summaries, business cases, investor updates, grant applications, and internal one-pagers that ask for a decision.

**Provenance: convention, not corpus.** These rules come from bid and proposal practice. No corpus study of machine-written proposals stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

Every other register is written to be browsed. This one is written to be judged, often by one reader against a rubric, sometimes by a committee scoring sections independently. The reader is looking for a reason to say no and stop reading. Ceremony gives them one.

## Rules this register overrides

- **CW-11 significance inflation is enforced harder than anywhere else.** This is the register's native disease. "A transformative partnership that will redefine how your organisation operates" is the default output and it scores nothing on any rubric.
- **CW-02 is tightened.** Every capability claim needs a named prior engagement, a named team member, or a labeled placeholder. "Extensive experience in the sector" without a nameable project is CW-02.
- **CW-52 inline-header lists is suspended for requirement matrices.** `- **R-4.2 Data residency:** All records stay in ap-southeast-1.` is the correct form when the header is the requirement identifier from the buyer's document.
- **CW-25 synonym cycling is inverted, against your own preference.** Use the buyer's vocabulary exactly as their document writes it, even where your term is better. A scorer searching for their word must find it.
- **CW-26 uniform cadence is relaxed** where a template fixes the section lengths.

## Answer the question that was asked

The dominant failure is a proposal that describes the vendor instead of answering the requirement.

Before:

> Our team brings a wealth of experience and a proven track record of delivering transformative solutions. We pride ourselves on our client-centric approach and our commitment to excellence at every stage of the engagement.

Rules hit: CW-11, CW-10 (proven, transformative), CW-02 (no evidence behind any claim), and no requirement answered.

After:

> [Answer the requirement. If the requirement is a migration window: "We will migrate 40 TB over three weekends, with the cutover on the third. Rollback stays available for 14 days."]

Practical method: build the response against the buyer's own numbering. Where a requirement cannot be met, say so and say what you offer instead. A scored "partially meets, here is the gap" beats an unscored paragraph of enthusiasm, and it survives the reference call that a bluff does not.

## The executive summary

It exists so that one person who reads nothing else can decide. It contains the decision being asked for, the number, and the date.

- Open with the ask, not with a thank-you for the opportunity.
- One paragraph on what is being proposed, in the buyer's terms.
- The price and the timeline appear here, not only in an appendix.
- No claim appears here that is not supported later in the document.

## Scope and pricing

- Name what is out of scope. A proposal with no exclusions is either dishonest or unpriced.
- Do not invent a price to fill a slot. Write `[PRICE]` and say what it depends on (CW-06).
- Assumptions get their own list, because each one is a change order later.
- Never present an estimate in the grammar of a commitment.

## Risk

A proposal that names no risk is not believable, and experienced buyers read the risk section first to find out whether the vendor has done this before.

Name the two or three real risks, the trigger for each, and what you do when it fires. Generic risk registers ("scope creep", "resource availability") say the template was filled.

## Investor updates

- Bad news first, with the number, in the first paragraph.
- Report the metric the same way every period. Changing the definition to make a quarter look better is CW-01 with a spreadsheet.
- "Ahead of plan on several fronts" without the numbers is CW-05.
- Name the ask. An update with no ask wastes the only reader who could act.

## Pitch decks

- One claim per slide, and the claim is the headline. A slide titled "Market" says nothing; "The 400 agencies in this segment each pay for three tools" says something.
- Market sizes are sourced or absent. A fabricated market number is the fastest way to end a meeting (CW-01, CW-02).
- No aphorism slides (CW-23). "Data is the new oil" survives no examination and buys no belief.
- Team slides name real people and their real prior work.
- The traction slide shows the axis labels. A chart without them is CW-01 in visual form.

## Format defaults for this register

- Bold: on the numbers, the dates, and the requirement identifiers. Not on adjectives (CW-51).
- Lists: correct for requirements, assumptions, exclusions, and risks. Prose for the argument.
- Emoji: none.
- Exclamation marks: none.
- Em dashes: replace (CW-50).
- Headings: follow the buyer's template, in the buyer's order, even where a better order exists.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Every requirement in the buyer's document has a response, in their numbering and their vocabulary
- [ ] Every requirement that cannot be met is marked as such, with the alternative stated
- [ ] The executive summary contains the ask, the price, and the date
- [ ] Every capability claim names a real project, a real person, or a labeled placeholder (CW-02, CW-06)
- [ ] No metric, market size, logo, or reference that is not real and permitted (CW-01, CW-04)
- [ ] Scope names its exclusions and its assumptions
- [ ] The risk section names real risks with real triggers
- [ ] No estimate written in the grammar of a commitment
- [ ] Nothing in the summary that the body does not support
- [ ] Read it as a scorer with eleven other submissions. Every answer is findable against their numbering
