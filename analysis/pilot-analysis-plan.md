# Pilot Analysis Plan

**Status: Draft; no pilot data should be analyzed until preregistration and ethics approval are complete.**

## Outcomes

### Primary outcome

Participant-level mean Calibration Alignment Score:

\[
CAS_i = \frac{1}{n_i}\sum_{j=1}^{n_i}\left(1 - \frac{|E_{ij}-C_{ij}|}{5}\right)
\]

Only fully coded conclusions enter the mean. Report n and exclusion count.

### Secondary outcomes

- CCR: proportion of eligible confidence statements upgraded without sufficient new evidence;
- ADR: unsupported assumptions divided by total claims;
- BCE: total and direction-specific successful, unsuccessful, and unaddressed events;
- pre/post confidence;
- evidence-quality and reasoning-quality judge ratings;
- creativity and idea-generation ratings.

## Independent judging

Create a separate reliability sample before condition-blind outcome analysis. Use at least two independent judges. Blind condition when feasible.

Predefine:

- ordinal reliability with two-way random-effects ICC for E and C;
- CCR or categorical decision agreement with quadratic-weighted Kappa;
- ADR agreement with Krippendorff's alpha or an equivalent categorical reliability statistic;
- BCE boundary agreement;
- adjudication rules for disagreement.

Use adjudicated ratings for primary analyses. Publish separate reliability values for raw ratings and adjudicated outcomes.

## Condition model

For the primary comparison, fit a prespecified linear model with participant-level CAS as the outcome and condition as the predictor:

```text
CAS ~ condition + scenario_id
```

Scenario assignment should be randomized or otherwise balanced. Add a prespecified participant-level covariate only if identified in the preregistration.

The primary contrasts are:

1. C versus A;
2. C versus B.

Report estimates, uncertainty, and sensitivity to the scenario covariate. Do not add a C-versus-B claim as confirmatory if the pilot is too small to support it.

## Exploratory comparisons

ADR and CCR are proportions. Use an appropriate count or binomial model with a participant-level denominator. Report raw counts in every table.

BCE frequency should be compared only alongside exposure opportunity and participant correction success. A high correction count is not automatically beneficial.

Pre/post confidence changes can be examined descriptively and, where complete, with a prespecified paired model.

## Missing data

Report missingness by condition and reason. Do not silently impute primary outcomes. Where a sensitivity analysis is possible, compare complete-case analysis with a prespecified worst/best-case bound or available-case model.

## Reliability of the confidence and evidence scales

Check inter-rater reliability and scale behavior before the primary CAS comparison. If E or C ratings are not reliable, mark CAS as not valid for confirmatory pilot inference and use it descriptively only.

## Reporting requirements

Every result table must include:

- condition and scenario denominators;
- raw CCR, ADR, BCE, and CAS values;
- judge reliability;
- exclusions;
- estimated differences and uncertainty;
- missingness;
- exploratory labels.

## Negative findings and mechanism claims

Report null and negative effects. Do not infer mechanism from condition differences alone. In-context model behavior, human learning, prompt effects, and interaction topology are competing explanations.

The analysis plan does not establish emergent calibration or loop-level intelligence.
