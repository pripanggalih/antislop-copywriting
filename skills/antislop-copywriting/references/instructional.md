# Register: instructional and training material

Load with `SKILL.md`. Covers course modules, lesson plans, workshop material, training decks, tutorials written for learners, textbook sections, exercises, quizzes, and onboarding curricula.

**Provenance: convention, not corpus.** These rules come from instructional design practice. No corpus study of machine-written course material stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

The boundary with `references/documentation.md`: documentation serves a practitioner who wants to leave as fast as possible, so repetition and signposting waste their time. Instructional material serves a learner who is staying, has no prior structure to hang anything on, and will forget most of it. That reverses several rules. Where a text is a reference someone returns to, use `documentation.md`; where it is a path someone walks once, use this file.

## Rules this register overrides

- **CW-40 signposting is inverted into a requirement.** A lesson opens with what the learner will be able to do at the end. That is an objective, and it does work. The defect is signposting with no objective: "In this lesson, we'll explore the exciting world of X. Let's dive in."
- **CW-44 summary padding is relaxed.** A closing recap that restates the objective in the vocabulary the learner just acquired earns its place. A recap that repeats the opening sentence does not.
- **CW-25 synonym cycling is inverted.** One term per concept, with the definition at first use. A learner cannot tell whether two words are two things.
- **CW-26 uniform cadence is relaxed across lessons.** Parallel lesson structure helps a learner predict what comes next. Inside a lesson, the paragraphs still vary.
- **CW-20 rule of three is relaxed** for enumerations that reflect real steps, real cases, or real options.

## Objectives that can be checked

An objective names something the learner can do and someone can observe. "Understand", "appreciate", "be familiar with", and "gain insight into" name nothing and are the surest sign the objective was generated rather than designed.

Before:

> By the end of this module, learners will have a deeper understanding of database indexing and appreciate its importance in modern applications.

Rules hit: CW-10 (deeper understanding, modern), CW-11, and two verbs nobody can test.

After:

> By the end of this lesson you can read a query plan, name which index it used, and add an index that changes it.

Usable verbs: list, write, run, predict, compare, fix, choose, explain to someone else. Every objective in a module should map to an exercise that would fail if the learner had not met it.

## The explanation-first failure

Machine-written lessons define the concept, then list its properties, then give an example. Learners meet the abstraction with nothing to attach it to.

Invert it. Show the situation, let the problem bite, then name the thing that solves it. The definition lands after the learner has felt the need for it.

## Worked examples and fading

- The first example is fully worked, with every step shown, including the step that looks too obvious to write.
- The second is partly worked, with the learner finishing it.
- The third is theirs.
- Never skip a step because it is easy. The skipped step is where learners stop.

## Exercises

- An exercise must be able to fail. If any answer is accepted, it is a prompt, not an exercise.
- State how the learner knows they got it right.
- Do not write the answer into the question.
- Where the exercise depends on an environment, name the version and the setup, and never invent a command or a flag (CW-01, and the cost here is a learner who thinks they broke it).

## Quizzes and assessment

- Every distractor is a real misconception, not filler. "None of the above" as a habit means the item was generated.
- The correct answer is not the longest option.
- Test the objective, not the wording of the lesson.
- Feedback on a wrong answer says what the learner probably thought and why it fails. "Incorrect, try again" teaches nothing.

## Tone with a beginner

- Delete "simply", "just", "obviously", "of course", and "as you already know". They are CW-14 filler, and they also tell a stuck learner that their difficulty is a personal failing.
- Do not congratulate a trivial step. Praise that costs nothing is heard as condescension.
- Address the learner as "you". Third person ("learners will") belongs in the objective line, not in the lesson.
- Say when something is genuinely hard. It is the most useful sentence in most lessons.

## Prerequisites and sequencing

- Name what the learner must already know, and where to get it.
- Nothing appears in a lesson that a later lesson introduces.
- Where a topic is deferred, say so once and name the lesson that covers it, rather than half-explaining it now.

## Format defaults for this register

- Bold: on terms at first definition (CW-51 relaxed as in documentation).
- Lists: for steps and options. An explanation is still prose.
- Emoji: only where the programme's existing design uses them (CW-53).
- Exclamation marks: at most one per lesson.
- Em dashes: replace (CW-50).
- Code and commands: exact, versioned, and run at least once before shipping.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Every objective names an observable action, not "understand" or "appreciate"
- [ ] Every objective maps to an exercise that would fail without it
- [ ] The situation comes before the abstraction
- [ ] Worked examples show every step, including the obvious one
- [ ] Every exercise can fail, and states how the learner checks their answer
- [ ] Every distractor is a real misconception; wrong-answer feedback names the misconception
- [ ] One term per concept, defined at first use (CW-25 inverted)
- [ ] No "simply", "just", "obviously", or praise for a trivial step
- [ ] Every command, flag, version, and output is real and was run (CW-01)
- [ ] Nothing used before it is introduced
