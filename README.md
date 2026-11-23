# Epistemic Governor Loops

> **Status:** Version 0.1 research notebook. This repository documents a developing research program, not a validated theory.

> **Before participating or citing a claim:** read [How to use this repository](docs/how-to-use-this-repository.md). Claims marked **Hypothesis**, **Provisional**, or **Stretch** have not been validated. We do not collect human-subject data until the protocol is preregistered and applicable ethics requirements are met.

This project asks whether human-AI reasoning systems can become more epistemically calibrated through interaction structure and governance. Its early focus is observable behavior; a broader architecture hypothesis is now under investigation.

## Core research question

Can a human and an AI, with distinct reasoning deficiencies, form a coupled feedback system that is more epistemically calibrated than either participant operating independently?

## Evolving direction

The original participant-centered question has expanded toward a system-architecture question:

```text
Human + AI
  -> Human + AI + Governance
  -> Human + Artificial + Machine
  -> Framework
  -> Governance
  -> Gates
  -> Calibration
```

This does not mean calibration is yet established as an architectural property. It defines a current working hypothesis and a future empirical program.

## Governance-pacing principle

Agentic systems need governance strong enough to prevent drift and unchecked technical debt, but light enough to preserve useful throughput and adaptation. This is a context-dependent tradeoff, not a fixed default.

```text
Too little governance -> drift, inconsistency, unchecked accumulation
Too much governance -> latency, premature convergence, process debt
Calibration -> sufficient control plus sufficient throughput
```

Use lighter gates for reversible, low-risk work and stronger gates for irreversible or high-impact work. Compress repeated gates after evidence of reliability; preserve deliberation for novel or uncertain work.

**Working hypothesis:** agentic systems fail when governance pressure and execution pace are improperly calibrated. This complements, rather than replaces, the epistemic-calibration research program.

See [Governance-Pacing in Agentic Workflows](docs/governance-pacing.md).

## Start here

1. **Nothing here is assumed to be validated.** H1–H4, HAM classifications, gate states, topologies, and emergent-intelligence claims remain testable proposals.
2. **Preregistration is mandatory before pilot data collection.** Hypotheses, conditions, primary outcomes, exclusions, coding rules, and analysis must be committed first.
3. **No sensitive or identifiable human-subject data belongs here.** Store protected transcripts privately and commit only synthetic or approved, safely de-identified artifacts.

## Research record

- [How to use this repository](docs/how-to-use-this-repository.md)
- [Preregistration template](protocol/preregistration-template.md)
- [Preregistration checklist](protocol/preregistration-checklist.md)
- [Research Note 001: From Epistemic Governor Loops to HAM Architectures](docs/research-note-001.md)
- [HAM ontology](docs/ham-ontology.md)
- [Framework versus governance](docs/framework-governance.md)
- [Gate theory](docs/gate-theory.md)
- [Governance-pacing in agentic workflows](docs/governance-pacing.md)
- [Topologies](docs/ham-topologies.md)
- [Open questions](docs/open-questions.md)
- [Research agenda](docs/research-agenda.md)
- [Terminology](docs/terminology.md)
- [Ethics](docs/ethics.md)

## Calibration metrics

| Metric | Working definition | Desired direction | Status |
|---|---|---|---|
| Confidence Creep Rate (CCR) | Unjustified confidence upgrades divided by total confidence statements | Lower | Operationalization incomplete |
| Assumption Drift Rate (ADR) | Unsupported assumptions divided by total claims | Lower | Operationalization incomplete |
| Calibration Alignment Score (CAS) | One minus normalized mismatch between evidence and confidence strength | Higher | Validation required |
| Bidirectional Correction Events (BCE) | Instances where either side detects and repairs unsupported reasoning | Measured as a process outcome; not automatically good in isolation | Coding required |

## Pilot hypothesis

**Hypothesis, not result:** structured governance may produce lower CCR and ADR, higher CAS, and measurable BCE while preserving creativity and idea generation.

| Condition | Structure |
|---|---|
| A. Control | Normal AI usage |
| B. Reflection control | Pause-and-reconsider protocol |
| C. Epistemic governor | Observation, inference, assumption, conclusion, confidence, and review |

A 20–30 participant pilot can estimate feasibility but is insufficient for strong publication claims.

## Repository status

- [x] Initial research question
- [x] Metric concepts
- [x] Pilot conditions
- [ ] Metric coding rules
- [ ] Inter-rater protocol
- [ ] Scenario validation
- [ ] Preregistration
- [ ] Pilot data
- [ ] Analysis

## Governing principle

Be publicly confident in observations and publicly cautious about conclusions. Capture ambiguity, negative findings, and unresolved definitions instead of converting them into premature theory.

## Contributing

Issues and pull requests are welcome for counterexamples, operational definitions, protocol critique, coding ambiguities, replication designs, and alternative architectures.

Label theory work as **provisional** and pilot questions as **hypotheses**. Do not describe a result as validated until the evidence and analysis support that description.

## License

No license has been selected yet.
