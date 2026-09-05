# Register: social and community posts

Load with `SKILL.md`. Covers posts and threads on X, LinkedIn, Instagram captions, TikTok and Reels on-screen text, YouTube titles and descriptions, Reddit and forum posts, Discord announcements, and replies in a community.

**Provenance: convention, not corpus.** These rules come from platform conventions and the post formulas that circulate on them. No corpus study of machine-written social posts stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

Social is the register where the machine tells are loudest, for a reason worth naming: the engagement formulas were already formulaic before models learned them. "Unpopular opinion:" was a template written by humans. A model reproducing it is copying a pattern the audience is tired of, and the audience punishes it faster here than anywhere else, because the post sits next to forty others.

## Rules this register overrides

- **CW-22 staccato drama is relaxed to a budget.** A hook may be a fragment. One run of short lines per post is a rhythm; a whole post built from one-line paragraphs is the LinkedIn wall, which is this register's most recognisable failure.
- **CW-53 emoji is relaxed where the platform's norm carries them.** An emoji inside a sentence is fine on Instagram. An emoji leading every bullet in a list is still a defect, on every platform.
- **CW-57 exclamation is relaxed to one per post.**
- **CW-27 rhetorical opener stays a defect** unless the question is real and the reply is the point. "What if you could 10x your output?" is a defect. "What broke for you in this release?" is a question.
- **CW-26 uniform cadence applies inside a thread.** Ten posts of near-identical length is the thread equivalent of uniform paragraphs, and it reads as generated.

## The engagement-bait grammar

These are the phrases that mark a post as machine-written before the reader reaches the content. Treat any of them as a defect on first instance, in the same way CW-15 treats "Learn More".

*Unpopular opinion:, Hot take:, Let that sink in, Read that again, Here's what nobody tells you, Nobody talks about this, I'll say it louder for the people in the back, This changed everything for me, Let me explain., And the results speak for themselves, Save this for later, Thank me later, The best part?, Here's the kicker, Most people get this wrong.*

Related shapes:

- **The colon-and-drop.** A two-word line, a colon, then the claim, repeated eight times down a post.
- **The false confession.** "I failed for 3 years before I learned this." Fabricated biography is CW-01 and CW-04 together, and it is the most common invented content in this register.
- **The numbered-lesson skeleton.** "7 lessons from building X" where the seven are interchangeable and none depends on another. This is the listicle skeleton from `editorial.md`, compressed.
- **The CTA tail.** "Follow for more", "Repost if you agree", "Drop a fire emoji if this resonates", "Comment WORD and I'll DM you the guide."
- **The hashtag pile.** More than two or three, or hashtags on a platform that does not use them.

## The hook

The first line decides whether the rest is read, which is why it attracts the most formula.

A hook that works names a specific thing. A hook that fails names a category and a feeling.

Before:

> Unpopular opinion: most teams are doing onboarding completely wrong. Here's what nobody tells you. 🧵

Rules hit: engagement-bait twice, CW-40, CW-53, and a claim with no content.

After:

> [State the specific thing that was observed. If the source is a support log: "Half our support tickets in March were people who could not find the export button."]

The bracket rule from `marketing.md` holds here. A hook cannot be written from a post that contains no observation.

## Platform notes

These are conventions, not ranking claims. Where a platform's limits matter, check the current ones rather than trusting a number in this file.

- **X.** A thread should have a reason to be a thread. If post 4 does not depend on post 3, it is a list and it wants to be one post or an article.
- **LinkedIn.** The one-line-paragraph wall, the humblebrag origin story, and the "Agree?" closer are the three tells. Ordinary paragraphs read as unusual there, which works in their favour.
- **Instagram and TikTok.** On-screen text is read at speed with sound off. Short lines, one idea each. The caption carries the detail the video could not.
- **YouTube.** The title states what the viewer will be able to do or see. The description is not a place for keyword lists.
- **Reddit and forums.** Marketing register is detected and punished. Answer the question, disclose the affiliation, and stop.

## Replies and community management

- A reply that restates the question before answering it wastes the reader's time.
- Do not answer criticism with gratitude formulas. "Thanks for the valuable feedback!" reads as a deflection.
- Never invent a fix, a date, or a policy in a reply. If it is not decided, say it is not decided.

## Format defaults for this register

- Bold: unavailable on most platforms and unnecessary on the rest.
- Lists: allowed and often correct. Do not lead each item with an emoji (CW-53).
- Emoji: at most two per post, inside sentences, never as bullets.
- Exclamation marks: one per post (CW-57).
- Em dashes: replace (CW-50). They render badly and read as pasted.
- Line breaks: use them to separate ideas, not to manufacture drama.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] No phrase from the engagement-bait list, in any form
- [ ] The first line names something specific, not a category and a feeling
- [ ] Every personal story, number, screenshot claim, and result is real (CW-01, CW-04)
- [ ] A thread is a thread because the posts depend on each other
- [ ] Post lengths inside a thread vary (CW-26)
- [ ] No CTA tail, no engagement instruction, no hashtag pile
- [ ] At most one exclamation mark and two emoji, none as bullets
- [ ] Affiliation is disclosed where the post promotes something
- [ ] Read it as the fourth post in a feed. It survives being scrolled past
