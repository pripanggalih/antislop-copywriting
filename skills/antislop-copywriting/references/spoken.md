# Register: spoken and scripted audio

Load with `SKILL.md`. Covers video scripts, YouTube, podcast episodes and intros, voiceover, webinars, conference talks, demo narration, audio ads, and the spoken track of course videos.

**Provenance: convention, not corpus.** These rules come from script-writing and broadcast practice. No corpus study of machine-written scripts stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

The listener cannot re-read a sentence, cannot skim ahead, and cannot see a comma. Text that works on a page can be impossible to follow at speaking speed, which makes this register the one where the read-aloud test in the universal gate stops being a check and becomes the whole method.

## Rules this register overrides

- **CW-25 synonym cycling is inverted.** Repeat the noun. A listener who meets "the platform", then "the tool", then "the system" has no way to scroll back and confirm they are the same thing.
- **CW-44 summary padding is relaxed.** After a long segment, a one-sentence recap is service. What stays a defect is a summary of something that ended thirty seconds ago.
- **CW-40 signposting is partly legitimate.** "First, the setup. Then the two failures." carries structure that a page would carry with headings. What stays a defect is signposting with no content: "In this video, we'll be diving into", "Let's get right into it", "Before we begin, let's understand".
- **CW-26 uniform cadence is measured in time, not paragraphs.** Sentence length still has to vary. A script where every sentence runs four seconds hypnotises.
- **CW-50 em dash** is invisible to the listener but stays out of the script, because the script's punctuation tells the reader where to breathe.

## Write for the ear

The test: read the script out loud once, at speaking speed, without stopping. Every place you stumble, run out of breath, or have to re-read is a defect. Fix the sentence, not the delivery.

- **One clause per sentence.** Nested clauses are invisible in audio. Split them.
- **Subject first.** "The build fails when the cache is cold" survives. "When the cache is cold, in cases where the runner has been recycled, the build fails" does not.
- **No parentheticals.** There is no sound for a bracket.
- **Contractions are required.** "Do not" reads as emphasis when spoken. Write "don't" unless the emphasis is intended.
- **Numbers in spoken form.** Write what the speaker says: "about two and a half million", not "2,483,912", unless the exact figure is the point. Where the exact figure matters, put it on screen and say the round one.
- **No homophone traps** in a sentence that has to land: their and there, hear and here.

## The cold open

Before:

> Hey guys, welcome back to the channel. Today we're going to be talking about database indexing. But before we get started, make sure to hit that like button. Let's dive in.

Rules hit: CW-40 twice, CW-42, and thirty seconds before the first fact.

After:

> [Start with the thing itself. If the topic is a slow query: "This query took eleven seconds. After one index, it takes forty milliseconds. Here is how the index works."]

The subscribe request, where it exists at all, goes after the first real segment, once and briefly.

## Structure

- Say the shape once, early, in one sentence. Then follow it.
- Give the listener a way back in. Someone drifts for ten seconds; the next sentence should still make sense.
- Transitions carry the structure: "That is the setup. Now the part that broke."
- End on the last real point. "Thanks for watching, see you in the next one" is fine as a sign-off, but it is not a conclusion (CW-43).

## Demo narration

- Say what you are doing before you do it, then say what happened. The viewer's eye follows your words.
- Name the thing you clicked by its on-screen label, exactly (CW-25 inverted, and it has to match the UI).
- Never narrate a result the recording does not show. A demo script that claims a passing test the video does not display is CW-01.
- Do not apologise for the interface on camera.

## Interviews and podcast prep

- Questions are short. A long question is a statement with a question mark.
- One question at a time. Two stapled together get one answer.
- Never script the guest's answer, and never write a quote for a person who has not said it (CW-04, CW-07).

## The script as a document

- Line breaks mark breaths.
- Mark direction in brackets on its own line: `[pause]`, `[on screen: the query plan]`. Keep them out of the spoken lines.
- No bold, no italics for emphasis. Emphasis is written into word order and sentence length, because the reader will not see the formatting.
- Include a word count and an estimated time. About 150 words per minute of conversational delivery is a working starting point; time the actual speaker rather than trusting it.

## Format defaults for this register

- Bold: none.
- Lists: for beats and shot notes, never for spoken lines.
- Emoji: none.
- Exclamation marks: none. Energy comes from the delivery, and a written exclamation makes a reader perform.
- Em dashes: replace (CW-50). Use a period, which is a breath.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] The whole script was read aloud once, at speed, and nothing forced a stumble or a second breath
- [ ] One clause per sentence, subject first, no parentheticals
- [ ] Contractions used; numbers written the way they are spoken
- [ ] The first fifteen seconds contain a real fact, not a welcome (CW-40)
- [ ] One term per thing, matching the on-screen label where there is one (CW-25 inverted)
- [ ] Nothing narrated that the recording does not show (CW-01)
- [ ] No quote put in another person's mouth (CW-04, CW-07)
- [ ] Sentence lengths vary when read on a clock, not just on the page (CW-26)
- [ ] The script ends on the last real point, with the sign-off separate from it
