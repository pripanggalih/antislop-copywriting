# Layer: search optimisation

Load in addition to `SKILL.md` **and** a register file, usually `marketing.md`, `editorial.md`, or `documentation.md`. This is a constraint layer, not a register. It adds requirements to whichever register the text already belongs to and replaces none of it.

**Provenance: convention, not corpus.** These rules come from search publishing conventions. No corpus study of machine-written search copy stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

Search work is where the two failures in `SKILL.md` meet. Copy written for a crawler reads as machine-written to a person, and copy scrubbed of its keyword becomes unfindable. Both are defects here.

## What this layer does not claim

This file describes conventions and display limits, not ranking mechanics. Any statement about what a search engine rewards is CW-02 unless it is cited to current documentation from that engine. Where a number matters to a decision, check the current guidance rather than trusting a figure written here.

## Rules this layer changes

- **CW-25 synonym cycling is inverted for the primary term.** The thing the page is about keeps one name throughout. Rotating it to avoid repetition makes the page about nothing.
- **CW-44 is relaxed for a summary that answers the question at the top.** A first paragraph that answers directly is service to a reader who arrived from a search, not padding.
- **CW-52 inline-header lists is relaxed inside an FAQ block**, where the question is the header and the answer follows.

## The dominant failure: writing to the keyword

Before:

> When it comes to project management software, choosing the right project management software for your team is essential. In this comprehensive guide to project management software, we'll explore everything you need to know about project management software.

Rules hit: CW-10 (comprehensive), CW-40, CW-14, and the term repeated four times in three sentences with no content between them.

After:

> [Answer the question the searcher typed. If the query is a comparison: "Four tools handle recurring tasks differently. Here is what each does when a task is missed."]

The term appears where it belongs in a sentence a person would write, and nowhere else.

## Structure for a reader who arrived from a query

- **Answer first.** The searcher's question is answered in the first paragraph. Background after.
- **One page, one question.** A page trying to rank for four unrelated queries answers none of them.
- **Headings name sections, not keywords.** A heading is a promise about what is under it.
- **No preamble before the answer.** The "In today's digital age" opener (CW-28) is the single most common thing between a searcher and what they came for.
- **Depth over length.** Padding a page to a word count adds the exact patterns this skill removes.

## Titles, descriptions, and links

- Title: name the specific thing, front-loaded. Truncation in results happens near 60 characters, so put the distinguishing word first rather than writing to a limit.
- Meta description: one or two sentences that say what the page delivers. It is a preview, not a slogan, and it is frequently rewritten by the engine anyway.
- Do not write a title the page does not fulfil. A title promising "10 examples" on a page with four is CW-01.
- Internal links: use the destination's real subject as the link text. "Click here" (CW-15) tells nobody, human or machine, what is at the other end.
- Alt text: describe the image for someone who cannot see it. Alt text stuffed with terms is a defect against a real user.

## Structured data and schema

Everything in the Hard tier applies to markup, and it is enforced by the platforms as policy.

- No review, rating, or aggregate markup for reviews that do not exist (CW-04).
- No FAQ markup for questions nobody asked, invented to occupy result space (CW-01).
- Markup must match what a visitor sees on the page. Text present only to a crawler is a fabrication with an audience of one.
- No invented author, no invented publication date, no backdated update.

## Refreshing an existing page

- Changing a date without changing the content is CW-01.
- Where a page is updated, say what changed.
- Do not add a keyword to an old sentence. Rewrite the sentence or leave it.

## Layer gate

Run after the universal gate and the register gate.

- [ ] The first paragraph answers the query the page targets
- [ ] The primary term has one name and appears where a person would write it (CW-25 inverted)
- [ ] No sentence exists to carry a keyword
- [ ] The title and headings promise only what the page delivers (CW-01)
- [ ] No padding added to reach a length
- [ ] Link text names its destination; alt text describes its image
- [ ] Every schema field matches something a visitor can see, and no review, rating, or FAQ markup is invented (CW-04)
- [ ] No date changed without a content change
- [ ] Read as someone who clicked from a results page. They have their answer before scrolling
