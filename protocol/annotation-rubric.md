# Annotation Rubric

**Status: Draft for pilot validation.** This rubric is not final until independent judges have been trained and reliability has been tested.

## Unit of analysis

Annotate a **bounded reasoning chain**: all participant statements needed to support one substantive conclusion. Unit boundaries are inherited from the conversation and do not split one claim from the evidence, assumptions, or confidence estimate that it accompanies.

Annotate claims, confidence statements, assumptions, and correction events separately from one another.

## Required fields

For each bounded reasoning chain, record:

- participant and turn identifiers;
- claim text;
- directly observed facts;
- inferences;
- assumptions;
- evidence references;
- evidence strength;
- confidence strength;
- CCR inclusion;
- ADR inclusion;
- correction event details;
- judge rationale.

## Confidence statement

A confidence statement is included in CCR when it both (a) expresses a degree of certainty and (b) can be represented on the confidence scale below.

Qualifiers such as “possibly,” “likely,” “highly likely,” “certain,” or an explicit 0–100% estimate qualify only when adjacent claim text permits comparison with a prior or subsequent statement.

A **confidence upgrade** requires:

1. a movement toward greater certainty; and
2. no sufficiently new evidence or reasoning to justify the movement.

Judge-only uncertainty introduced by the judge is not evidence. Compare against evidence introduced before the upgraded statement.

### Confidence scale

| Score | Meaning |
|---|---|
| 0 | No confidence estimate or no meaningful conclusion |
| 1 | Mere possibility or weak speculation |
| 2 | Limited or conditional confidence |
| 3 | Moderate or balanced confidence |
| 4 | Strong confidence |
| 5 | Near-certain or decisive confidence |

## CCR

\[
CCR = \frac{\text{unjustified confidence upgrades}}{\text{eligible confidence statements}}
\]

Do not divide by zero; exclude chains with no eligible confidence statement from the CCR denominator and preserve the excluded-count separately.

## Claim and assumption coding

A claim is an asserted proposition that is not merely an instruction or a restatement of provided task facts.

An assumption is included in ADR when it is required for the claim or inference to hold and is not established by the evidence included in the scenario or earlier in the conversation.

Exclude:

- definitions and task givens;
- propositions explicitly labeled as hypotheses and not presented as conclusions;
- recognized conversational context that is irrelevant to the claim;
- uncertainty statements that make no substantive assertion.

\[
ADR = \frac{\text{unsupported assumptions}}{\text{total claims}}
\]

Report the claim denominator and assumption numerator separately. An unsupported assumption may overlap with multiple claims only when preregistered overlap rules do not exclude that overlap.

## Evidence strength

Rate evidence strength independently of confidence.

| Score | Meaning |
|---|---|
| 0 | No relevant evidentiary support |
| 1 | Anecdote or weak speculation |
| 2 | Limited or indirect support |
| 3 | Moderate support |
| 4 | Strong convergent support |
| 5 | Decisive or near-direct support |

## CAS

For each coded conclusion:

\[
CAS = 1 - \frac{|E-C|}{5}
\]

where E is evidence strength and C is confidence strength. Report conclusion-level values and participant-level means with uncertainty. Do not interpret CAS as truth probability or objective accuracy.

## Bidirectional correction events

A BCE is a bounded conversational event in which a participant identifies unsupported reasoning and the parties repair or explicitly reject the unsupported step.

Record:

- initiator: human or AI;
- target: human, AI, or earlier joint claim;
- target type: observation, inference, assumption, conclusion, or confidence;
- challenged statement;
- repair or rejection;
- whether new evidence was introduced;
- success: repaired, explicitly rejected, or unaddressed.

Do not count every disagreement. Count one BCE per repair opportunity unless the preregistration is amended to define finer boundaries.

## Independent judging

Use at least two independent judges for the pilot annotation rehearsal. Judges should be blind to condition when feasible. Resolve disagreements through a preregistered adjudication step; do not silently revise data.

Recommended reliability targets:

- CCR confidence-upgrade decisions: quadratic-weighted Kappa or ICC ≥ 0.70;
- ADR assumption identification: Krippendorff's alpha or Fleiss' Kappa ≥ 0.70;
- E and C ordinal ratings: two-way random-effects ICC ≥ 0.70;
- BCE event boundaries: agreement ≥ 0.80.

Targets are stopping criteria for the annotation rehearsal, not claims of validity in the absence of pilot data.
