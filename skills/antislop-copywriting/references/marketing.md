# Register: marketing and landing copy

Load with `SKILL.md`. Covers landing pages, product marketing, ads, headlines, CTAs, value propositions, pricing, FAQ, and About pages.

Marketing is the register where fabrication is most tempting and most damaging, because vague copy and invented copy look identical at a glance. The Hard rules do most of the work here.

## Reading the examples

Every rewrite below obeys CW-01: it introduces no fact that is not in the text being rewritten. Most slop headlines contain no facts at all, so an honest rewrite of one cannot contain facts either. Where that is the case, the rewrite states the gap in brackets and, where useful, shows what the line would look like under a stated assumption. That bracket is the lesson, not a placeholder for laziness. Copy that needs a real detail gets the real detail from the user, or gets written without it.

## Headlines

The default AI headline announces a category and a feeling. It survives being pasted onto a competitor's site, which is the test it fails.

**Swap test.** Put a competitor's name in the headline. If it still reads as true and sensible, the headline says nothing. This is the fastest check in this file.

- **Abstraction stack.** Three abstract nouns bolted together: "Streamlined Workflow Intelligence". Nobody can picture it.
- **Benefit without mechanism.** "Ship faster." Faster than what, by doing what. The mechanism is the interesting half and it is always the half that gets cut.
- **Colon formula.** "Acme: The Future of Team Collaboration". The colon promises a definition and delivers a category.
- **Question headline.** "Tired of messy spreadsheets?" A question hands the reader work before giving them anything.

Before:

> Unlock the power of seamless collaboration to elevate your team's journey to the next level.

Rules hit: CW-10 (unlock, seamless, elevate), CW-11 (next level), CW-24 (journey framing), CW-60 after any naive cleanup.

After, and note that the source names no product behaviour, so neither can the rewrite:

> [State what the product does. If it is a shared editor: "Your team writes in the same document."]

The bracket is not a cop-out. It is the correct output when the input contains no product. Ask the user what the thing does and the headline writes itself.

## CTAs

A CTA names the action the button performs. Generic CTAs (CW-15) are the tell, but the fix is not a longer generic CTA.

Weak defaults: *Get Started, Learn More, Try Now, Explore, Discover, Sign Up, Submit, Click Here*.

The test: read the CTA with the question "and then what happens?" If the answer is not in the label, the label is not finished.

| Instead of | Write what happens |
|---|---|
| Get Started | Create your first project |
| Learn More | See how billing works |
| Try Now | Open the demo, no account needed |
| Contact Us | Email the support team |
| Submit | Send the request |

Two rules that follow:

- The CTA and the destination must agree. A button that says "Start free trial" leading to a pricing table is a broken promise, and it is a CW-01 problem, not a style problem: it states something untrue about what the click does.
- Do not add urgency the product does not have. "Only 3 spots left" without a real limit is CW-02.

## Value propositions

The shape that works: **who it is for, what it does, what changes.** All three, in plain words, without adjectives doing the work.

Failure modes specific to this register:

- **Adjective substitution.** "Powerful, intuitive, and beautiful" replaces the description rather than adding to it. CW-10 plus CW-20.
- **Everyone-and-no-one.** "For teams of every size, in every industry." Audience-blanket phrasing that describes no reader. Related: "Whether you're a solo founder or an enterprise, ...".
- **Pivot sentence.** The problem paragraph, then "That's where Acme comes in." CW-29. Cut the hinge and let the product statement stand alone.
- **Temporal opener.** "In today's fast-paced world." CW-28. Delete without replacement, the paragraph is always fine without it.

Before:

> In today's fast-paced digital landscape, teams are drowning in tools. That's where Acme comes in. Acme is a powerful, intuitive platform that empowers teams to do their best work.

Rules hit: CW-28, CW-29, CW-10 (powerful, intuitive, empowers), CW-11.

After:

> Teams are drowning in tools. [State what Acme does and for whom. The source does not say.]

Everything except the first sentence was ceremony and the source never supplied a product fact to keep.

## Social proof

This is where CW-04 bites hardest, and where the temptation is strongest, because a testimonials section looks unfinished when empty.

It is better empty. A fabricated testimonial is not a placeholder that gets replaced later, it is a false statement shipped to customers.

- No real customers to name: delete the section. Do not soften it into "Trusted by teams everywhere", which is CW-02 with the evidence removed rather than supplied.
- Real customers, no permission to name them: describe the shape without the identity. "Used by two logistics companies in Southeast Asia" is honest if true, and it is a fact the user must supply.
- Numbers: every number needs a source you could show someone. "10,000+ users", "99.9% uptime", "500M requests" are CW-01 and CW-02 together unless real.
- Logo bars: every logo must be a real customer with permission. A logo bar of companies that merely use the underlying open-source library is a lie by arrangement.

Before:

> Trusted by thousands of teams worldwide. "Acme cut our review time in half." - Sarah Chen, VP Engineering

After:

> [Delete both lines unless a real customer and a real quote exist. If they do, use their words and their name, with permission.]

## Pricing

- Name what the buyer gets, in their words, not in feature names only they will not recognise.
- Do not invent tier contents. If the tiers are undecided, write `[TIER CONTENTS]` and say so (CW-06).
- "Most popular" must reflect real purchase data. Otherwise it is CW-04 dressed as a badge.
- "No hidden fees, no contracts, no surprises" is CW-20 plus CW-21. State the actual billing terms instead.

## FAQ

An FAQ is answers to questions people actually asked. Anything else is filler that costs trust.

- Template questions ("Is my data secure?", "Can I cancel anytime?") belong in an FAQ only when they are the questions your users send you, and the answer is specific.
- "Absolutely!" and "Of course!" as answer openers are CW-57 and add nothing.
- If you do not know what people ask, the section does not exist yet.

## Format defaults for this register

Marketing prose is read fast and skimmed first, which makes formatting tells louder here than anywhere else.

- Bold: sparingly, and never on every key term (CW-51). Threshold is 2 spans per 100 words.
- Lists: only where the content is genuinely a list. Do not use `- **Header:** restatement` (CW-52).
- Emoji: not in headings (CW-53).
- Exclamation marks: at most one per 150 words (CW-57).
- Em dashes: replace (CW-50), unless the user's voice sample uses them.
- Title Case: use sentence case in headings unless a brand guide says otherwise (CW-56).

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] The headline fails the swap test: putting a competitor's name in it makes it false or odd
- [ ] Every CTA names what happens on click, and the destination matches the promise
- [ ] The value proposition states who it is for, what it does, and what changes
- [ ] Every number, logo, quote, and named customer is real and permitted (CW-01 to CW-04)
- [ ] No pivot sentence, no temporal opener (CW-28, CW-29)
- [ ] Pricing describes real tiers, or labeled placeholders
- [ ] Every FAQ question is one a real user asked
- [ ] The page would still make sense to a reader who skipped every adjective
