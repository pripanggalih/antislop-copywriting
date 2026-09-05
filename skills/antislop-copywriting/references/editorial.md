# Register: long-form editorial

Load with `SKILL.md`. Covers blog posts, articles, essays, newsletters, opinion pieces, and case studies.

Length is what makes this register different. A landing page has too few words to establish a rhythm. Three thousand words establish one whether the writer intended it or not, and machine rhythm is the most reliable tell there is. In long text, structure gives you away before vocabulary does.

## The structural tells

These matter more here than any word list.

**CW-26 uniform cadence.** The strongest signal in this register and the least noticed. Machine-written long text settles into paragraphs of near-identical length, usually three to five sentences, section after section. Human writing lurches. A one-sentence paragraph after a long one is a human move, and its absence across two thousand words is a confession.

Measure it. Count the words in each paragraph. Five or more consecutive paragraphs within 15% of each other is a FAIL. The fix is not to randomise lengths, it is to let each paragraph end when its point ends.

**Section symmetry.** Every section the same depth, the same number of subsections, the same shape. Real arguments are lopsided, because some parts need more work than others. A piece where every section is the same size is a piece where the outline was filled rather than followed.

**The listicle skeleton under prose.** Text that is secretly a numbered list wearing paragraphs: each section makes exactly one point, introduces it, restates it, and moves on. Real argument builds, where later sections depend on earlier ones. If the sections can be shuffled without damage, there was no argument.

**Intro that summarises the article.** A first section that previews everything the piece will say, followed by the piece saying it. Cut the preview. Start with the thing itself.

## The sentence-level tells

- **CW-28 temporal opener.** "In today's fast-paced world", "In an era of". Delete without replacement.
- **CW-40 signposting.** "In this article, we'll explore", "Let's dive in", "Before we begin, let's understand". CW-44 is its closing twin: "In summary", "To recap", "In conclusion" ending a piece the reader just finished.
- **CW-42 fake-candid opener.** "Here's the thing", "Let's be honest", "Real talk". A theatrical pause before an ordinary claim.
- **CW-43 generic positive conclusion.** "The future looks bright", "one thing is certain: things will keep changing". End on the last real thing you have to say and stop.
- **CW-21 negative parallelism.** In long text these accumulate. Two in three thousand words is nothing, six is a signature.
- **CW-23 aphorism formulas.** "X is the currency of Y". The sentence that sounds like it belongs on a slide and survives no examination.
- **CW-12 authority tropes.** "At its core", "the real question is". Announces depth before delivering an ordinary point.
- **Transition stacking.** "Moreover", "Furthermore", "Additionally", "That said" opening consecutive paragraphs. One is a word. Four in a row is a machine gluing an outline together.

Before:

> In today's rapidly evolving digital landscape, the way we approach remote work has fundamentally shifted. In this article, we'll explore the key trends shaping the future of distributed teams. Let's dive in.

Rules hit: CW-28, CW-10 (landscape, fundamentally), CW-40 twice.

After:

> [Start with the first real claim. The source contains none, only an announcement that claims are coming.]

Three sentences and no content. This is the standard shape of a machine-written opening, and the honest rewrite of an empty opening is to delete it and begin at the first thing you actually have to say.

## Evidence in long form

Length invites fabrication, because a long piece feels underweight without numbers and quotes.

- CW-03 ghost attribution is the characteristic failure here. "Studies show", "research suggests", "experts agree". Name the study, link it, or drop the claim.
- Statistics need a source the reader can reach. A number with no link is a number you are asking to be trusted on.
- Do not invent an anecdote to open a section. The composite customer, the unnamed engineer at a large company, the conversation that illustrates the point too neatly. These are CW-01 and they are the most common fabrication in the register precisely because they feel like craft.
- Do not fabricate a counterargument to knock down. If nobody holds the position, do not attribute it to "some people".

## What good looks like here

The universal layer's CW-60 matters most in long form, because sterile prose survives a landing page and cannot survive three thousand words.

- Vary sentence length deliberately. Land a short one after a long one.
- Repeat a word when it is the right word. Elegant variation is a machine habit (CW-25).
- Keep the specific detail. The exact number, the odd name, the real date, the thing that could not have been guessed. LLMs round off, humans hoard.
- Leave tension unresolved where it is unresolved. "I think this is right and it still bothers me" is a sentence a model does not write.
- Let one paragraph be a single sentence when the point is a single sentence.

## Format defaults for this register

- Bold: rarely. Long text with bolded phrases scattered through it reads as a summary of itself (CW-51).
- Subheadings: only where the reader needs a landmark. A subheading every 200 words is a listicle in disguise.
- Lists: when the content is a set. A long piece that is more list than prose was an outline that never became an argument.
- Pull quotes: only for words someone actually said.
- Emoji: no (CW-53).
- Em dashes: replace (CW-50), unless the author's voice sample uses them, which in this register it often will.
- Exclamation marks: at most one per 150 words (CW-57), and usually zero.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Paragraph word counts measured; no run of 5 within 15% of each other (CW-26)
- [ ] Sections are not all the same size and cannot be shuffled without damage
- [ ] No preview section restating what the piece will say
- [ ] No signposting opener and no summary closer (CW-40, CW-44)
- [ ] Every statistic, study, and quote is named and reachable (CW-03)
- [ ] No composite anecdote, no invented conversation, no unnamed source (CW-01)
- [ ] No counterargument attributed to nobody in particular
- [ ] At least one specific, hard-to-invent detail survives in the final draft
- [ ] Read the opening and closing aloud. Neither announces itself
