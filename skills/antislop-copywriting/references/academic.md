# Register: academic and research writing

Load with `SKILL.md`. Covers journal articles, conference papers, theses and dissertations, abstracts, literature reviews, research proposals, peer review reports, and lab reports.

**Provenance: convention, not corpus.** These rules come from the conventions of academic publishing and peer review. No corpus study of machine-written academic prose stands behind the pattern lists here, so treat the shapes as real and their frequencies as unmeasured. The corpus-grounded material in this skill is the universal layer in `SKILL.md`.

This register inverts more of the universal layer than any other, because several of its conventions look exactly like machine tells. Uniform section structure, hedged claims, passive voice in a methods section, and one term repeated three hundred times are discipline requirements here. Stripping them damages the paper.

The compensation is that the Hard tier applies with no slack. A reader of a paper can check every claim, and some of them will.

## Rules this register overrides

- **CW-13 stacked hedging is relaxed into calibration.** "These results suggest that X may contribute to Y" reports a real confidence level. It is not slop. The defect is hedging that hides the absence of a result: "may potentially indicate a possible relationship" stacks qualifiers until the sentence claims nothing and admits nothing.
- **CW-26 uniform cadence is suspended in Methods and Results.** Procedural text is uniform because the procedure is. The rule still applies in the Introduction and the Discussion, which are arguments and should be lopsided.
- **CW-25 synonym cycling is inverted into a requirement.** One term per construct, for the length of the document. If the variable is "task completion time" in the Methods, it is not "task duration" in the Results. Rotating the term makes the finding unverifiable.
- **CW-30 actorless passive is relaxed in Methods only.** "Samples were incubated for 12 hours" is the convention and the actor is not in question. In the Discussion, the passive hides who is making a claim, and there it stays a defect: "it is argued that" is you arguing.
- **CW-20 rule of three is relaxed** for enumerations that reflect three real conditions, hypotheses, or experiments.
- **CW-56 Title Case follows the venue.** APA, Chicago, IEEE, or the target journal outranks the preference in `SKILL.md`.

## The dominant failure: citation drift

Fabricated references are the failure everyone knows. Invented DOIs, real authors bolted to papers they never wrote, plausible titles in real journals: all CW-01, each one career-level.

Citation drift is quieter and survives most checks. The reference exists. The authors are right. The year is right. The paper does not support the sentence it is attached to.

Three shapes:

- **Inflation.** The source reports a correlation in one small sample. The sentence cites it for a general causal claim.
- **Transitive citing.** The claim came from a paper that cited the source. The source was never read and does not say what the citing paper said it said.
- **Decoration.** A citation attached to a sentence that needs none, so an unsupported passage looks sourced. This is CW-03 wearing a reference list.

Rule for this skill: never attach a citation that was not in the source material, and never move an existing citation to another sentence. Moving one changes what it claims. Where a sentence needs support the material does not contain, write `[CITATION NEEDED]` (CW-06) and say so in the response.

## Abstract

An abstract states what was done, what was found, and what it means, with the numbers. It is the part most often written as an advertisement for the paper.

Before:

> This paper delves into the multifaceted challenges of distributed consensus, offering novel insights that shed light on an area that has garnered significant attention in recent years.

Rules hit: CW-10 (delve, multifaceted, novel, insights), CW-11, CW-40, and three sentences that report no result.

After:

> [State the method, the finding, and the effect size. The source contains none of them, so they must come from the paper.]

If the abstract cannot be written from the paper's own results, the paper is not finished.

## Introduction and the gap statement

The machine-written introduction summarises the field, announces a gap, and never says what the gap costs anyone.

- **The literature parade.** One sentence per citation, chronological, with no argument connecting them. A related-work section is an argument about why this work was needed, not a list.
- **The manufactured gap.** "However, little research has examined X." This is a checkable claim about the literature and it is CW-01 when nobody checked. Say which searches were run, or write the honest version: the gap is narrower than the sentence wants it to be.
- **CW-28 openers.** "In recent years, X has attracted increasing attention." Delete without replacement. The first real sentence is always better.

## Results versus Discussion

The line between them is where overclaiming happens.

Results report what was measured, in the past tense, without interpretation. Discussion interprets, and every interpretive sentence has to stay inside what the design supports.

- A correlational design does not produce "X improves Y". It produces "X was associated with higher Y".
- A significant result is not a large one. Report the effect size next to the p-value, or report neither.
- "Trending toward significance" describes a result that did not reach it. Write the number.
- Do not carry a Discussion verb back into the Results.

## Limitations

An AI-written limitations section is generic, self-flattering, and always the same three items: sample size, generalisability, future work.

Real limitations are specific and they cost something. Name the measurement that was noisy, the condition that was not counterbalanced, the population the sample excludes. If the honest list is uncomfortable, that is evidence it is the real one.

## Conclusion

- **CW-43 in academic dress.** "Future research is needed", "this remains an open question", "these findings hold promise". End on the last real finding.
- Do not restate the abstract. A conclusion says what changes now that this is known.
- No claim appears in the conclusion that did not appear, with support, earlier in the paper.

## Peer review reports

A review is correspondence with a person whose work is on the line. Two failures specific to it: the review that summarises the paper back to the author and adds nothing, and the review that hedges every objection until the editor cannot act on it.

State each point as a numbered request, tied to a line or section, marked major or minor. Say what would change your recommendation.

## Vocabulary

On top of CW-10, this register carries its own overused set: *novel, paradigm, shed light on, a growing body of literature, warrants further investigation, holds promise, plays a vital role, has garnered significant attention, multifaceted, underscores the importance of, sheds new light, paves the way*.

Formal vocabulary is not the tell. These specific words are.

## Format defaults for this register

- Bold: only where the venue's template uses it. Running prose gets none (CW-51).
- Lists: allowed in Methods and in reviews. In the Introduction and Discussion, an argument is prose.
- Em dashes: replace (CW-50), unless the venue's style guide uses them.
- Terminology: fixed, with a definition at first use. Keep a list if the document is long.
- Tense: past for what was done and found, present for what is established.

## Register-specific gate

Run after the universal gate in `SKILL.md`.

- [ ] Every citation exists, was read, and supports the exact sentence it sits on (CW-01, and see citation drift)
- [ ] No citation was added, moved, or reattached during editing
- [ ] Every number, effect size, sample size, and p-value traces to the results, not to the draft
- [ ] No claim about the literature ("little research has examined") that nobody verified
- [ ] Results contain no interpretation; the Discussion claims nothing the design cannot support
- [ ] One term per construct, identical across every section (CW-25 inverted)
- [ ] Limitations are specific to this study and cost something to admit
- [ ] The conclusion adds no claim that was not supported earlier (CW-43)
- [ ] Hedging reports a real confidence level and is not stacked (CW-13)
- [ ] The venue's style guide was followed where it disagrees with this skill
