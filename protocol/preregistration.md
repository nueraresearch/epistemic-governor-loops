# Pilot Preregistration

**Status: Draft preregistration; not a deployed or approved study protocol.**

## 1. Study purpose

This pilot asks whether a structured epistemic-governor interaction produces process and calibration differences relative to normal AI use and an unstructured reflection control.

This is a signal-detection and feasibility study. It is not powered to establish efficacy, mechanism, or architectural emergence.

## 2. Population and eligibility

Recruit adults with informed consent and no known conflict of interest. The default pilot target is 20–30 participants, with the final number determined before data collection.

Exclude participants who:

- cannot give informed consent;
- are under the applicable age of majority;
- submit no usable transcript;
- complete fewer than one full scenario;
- violate the randomized condition after assignment;
- disclose an exclusion-relevant high-impact real-world decision context.

No consequential medical, legal, employment, or financial decision may be made from participant outputs.

## 3. Study design

Participants complete one or more versioned low-stakes scenarios in three conditions:

- **A. Standard control:** normal AI interaction prompt.
- **B. Reflection control:** prompt the participant to pause and reconsider observations, alternatives, and confidence.
- **C. Epistemic governor:** structured separation of observations, inferences, assumptions, conclusions, confidence, missing evidence, alternatives, and review.

Randomize condition after eligibility and consent. Counterbalance scenario order if more than one scenario is used. Hold model, system prompt, available context, and time limits as comparable as possible.

Preserve a model-specification record including model name, provider, date, temperature if available, and system or interface instructions.

## 4. Primary hypothesis

**H1:** At post-interaction rating and process-measure level, epistemic-governor Condition C will show greater calibration alignment than Conditions A and B.

Primary outcome:

- **CAS**, the conclusion-level mean Calibration Alignment Score.

Interpret CAS only as a condition comparison on the pilot rubric. It is not a measure of truth or predictive accuracy.

## 5. Secondary process outcomes

- CCR;
- ADR;
- successful, unsuccessful, and unaddressed BCE;
- pre/post confidence difference;
- judge-rated evidence quality;
- judge-rated reasoning quality;
- idea-generation and creativity measures;

No secondary result will be described as a mechanism test.

## 6. Primary analysis

Use participant-level CAS after averaging conclusion scores within each participant. Apply a prespecified two-condition contrast or linear model as specified in `analysis/pilot-analysis-plan.md`.

Report:

- condition means and standard deviations;
- median and interquartile range;
- estimated difference and 95% confidence interval;
- ICC or Kappa for independent judges;
- exclusions and denominators;
- complete null and negative results.

The pilot is not a confirmatory efficacy trial. Do not use a “significant result” threshold to claim the epistemic-governor mechanism exists.

## 7. Exploratory questions

The following are explicitly exploratory:

- whether reflection alone accounts for effects;
- whether CCR, ADR, and BCE differ between conditions;
- whether effects vary by task domain;
- whether prior AI experience changes outcomes;
- whether the structured protocol changes idea generation or creativity;
- whether the bidirectional correction rate predicts CAS.

Report multiple-comparison limits and do not add outcomes after examining condition-level distributions.

## 8. Measurement and coding

Use `protocol/annotation-rubric.md` and the metric documents without post hoc modification.

The unit of analysis is the bounded reasoning chain. CCR and ADR denominators must be reported even where they are zero or incomplete.

Two independent judges will code a reliability rehearsal. Adjudication rules and final reliability thresholds are fixed before the pilot sample is annotated.

## 9. Exclusion and missing-data rules

Exclude an entire participant only for eligibility or process-completion failures specified above. Record, rather than delete, partial data where permitted.

For individual conclusions:

- include them when evidence and confidence ratings are complete;
- mark no-confidence and no-evidence cases according to the rubric;
- never replace a judge rating with a research-team guess;
- disclose missingness by condition.

## 10. Revisions

Any revision after this draft is preregistered must include:

- reason for revision;
- timestamp;
- changed text;
- impact on the primary outcome or analysis;
- ethics and approval implications.

## 11. Ethics and data handling

Obtain informed consent and institutional or independent ethics review where required.

Explain that AI-generated content may be inaccurate and cannot substitute for professional judgment.

Minimize identifiers and confidential material. Store consent records separately from data. Public artifacts may include only synthetic examples or approved, de-identified artifacts.

Participants may withdraw and request deletion where the approved protocol permits it.

## 12. Publication and reporting commitments

Report negative, null, and inconclusive findings. Distinguish behavioral differences from possible explanations. Do not claim causality solely from in-context model behavior. Preserve exact denominators, exclusions, and judge disagreement.
