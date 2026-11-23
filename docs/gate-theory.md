# Gate Theory and Governance

**Status:** Initial working outline (v0.1). Definitions in this document are hypotheses for operationalization and experimental testing, not settled findings.

## I. Foundations

### 1. Framework

A **framework** defines the reasoning loop: participant roles, loop topology, information flow, transition points, outputs, feedback relationships, and termination or escalation conditions.

A framework is descriptive. It does not by itself establish that a system is calibrated or controlled.

#### Loop topology

A loop topology describes how system elements exchange information and influence future state. The topology should distinguish sequential turns, cycles, parallel processes, review handoffs, and external feedback sources.

#### Participants

A participant is a role that influences future system state through observation, interpretation, action, recommendation, or state transition.

- **H — Human:** a participant role carried out by a person.
- **A — Artificial Intelligence:** a participant role implemented through artificial intelligence.
- **M — Mechanism/Machine participant:** a participant role not adequately represented by H or A in the chosen frame.

Participant role is distinct from ontology. A category may change with system context.

#### Information flow

Describe which elements receive observations, emit claims, consume evidence, issue corrections, and update or replace state. Information flow diagrams should identify both normal transitions and feedback.

### 2. Governance

**Governance** defines the constraint system placed within or around a framework. It controls whether, when, and how a state transition is admitted, modified, blocked, deferred, escalated, or audited.

Working notation:

```text
Framework = Loop
Governance = Loop + Gates
```

This notation is provisional. Governance may be implemented through social norms, interface structure, participant behavior, automated controls, or combinations of these mechanisms.

#### Constraint systems

Constraint types include:

- evidentiary constraints
- assumption constraints
- confidence constraints
- authority constraints
- timing constraints
- resource constraints
- safety constraints
- auditability constraints

#### Gate models

A gate model specifies each gate's trigger, input, threshold, state transition, authority, output, and failure behavior.

#### Override mechanisms

Overrides intentionally permit or alter a transition that would otherwise be blocked or deferred. Every override should preserve an observable record of authority, reason, state, risk, and outcome.

## II. Gate theory

### 1. Gate definition

A **gate** is a control point that admits, modifies, blocks, defers, escalates, or records a state transition in a reasoning system.

Each gate should define:

- **Input:** the claim, evidence, assumption, confidence estimate, or system state evaluated.
- **Threshold:** the rule or criterion determining the resulting state.
- **State:** the output state and resulting transition behavior.
- **Authority:** the participant or process that evaluates and may override the gate.
- **Audit:** the observable record necessary to reconstruct and review the decision.

### 2. Gate states

Candidate states:

- **PASS:** the gate permits the transition.
- **FAIL:** the gate blocks or degrades the transition.
- **OVERRIDE:** an authorized participant permits or modifies the transition despite the gate result.
- **DEFER:** the gate requires new information or review before deciding.
- **ESCALATE:** the gate routes the transition to a higher-authority process.
- **ERROR:** the gate cannot evaluate its input or execute correctly.

Gate states must be distinguishable from the quality of the underlying claim. A PASS state can still produce a bad outcome, and a FAIL state can prevent one.

### 3. Candidate gate types

- **Observation Gate:** identifies the admitted observation and separates observation from inference.
- **Evidence Gate:** evaluates evidence quality, sufficiency, provenance, and relevance.
- **Assumption Gate:** exposes required assumptions and whether they are supported.
- **Confidence Gate:** compares stated confidence with available evidence and flags mismatch or unjustified upgrade.
- **Correction Gate:** detects unsupported reasoning and routes a correction or repair.
- **Convergence Gate:** detects premature consensus or premature closure.
- **Contradiction Gate:** identifies unresolved contradictions and prevents silent reconciliation.

Additional gate types can be introduced only when they have distinct triggers and observable behavior.

## III. Gate failure

Gate failure is distinct from bad reasoning. A gate can fail by being absent, incorrectly triggered, incorrectly evaluated, silent, or overridden without sufficient authorization or evidence.

### 1. Missing evidence

The gate receives no adequate support for a claim that requires evidence.

### 2. Unsupported assumption

The reasoning chain depends on an assumption that is implicit, untested, or inadequately supported.

### 3. Confidence-evidence mismatch

Stated confidence materially exceeds or understates support quality under the preregistered scale.

### 4. Premature convergence

The system terminates exploration or agreement before alternatives, contrary evidence, or unresolved uncertainty has been considered.

### 5. Unresolved contradiction

The system preserves incompatible claims or silently chooses among them without identifying the conflict or revision rule.

### 6. Silent gate failure

A gate appears active but emits no result, or an error is indistinguishable from a PASS or FAIL state.

## IV. Gate override

An override is an intentional departure from gate-enforced control. It should be rare enough to be observable and consequential enough to require audit.

Every override record should include:

- overrider and authority level;
- original gate and state;
- reason;
- new evidence or policy, if any;
- affected claim or transition;
- acknowledged risks;
- resulting state;
- outcome and later review status.

### 1. Human override

A human intentionally permits or revises a transition blocked or deferred by the system.

### 2. AI override

An AI participant explicitly changes or bypasses a gate state through its own output or action. In a governed system, this should be distinguished from ordinary recommendation.

### 3. System override

An automated process applies policy, prioritization, fallback, or escalation logic to alter gate behavior.

### 4. Emergency override

A predefined procedure permits immediate action under time pressure or safety conditions while preserving mandatory audit and review.

Emergency override should not become a general substitute for missing design or weak gate thresholds.

## V. HAM governance

HAM governance studies how governance changes as roles and participants are arranged. Notation describes the working topology, not settled ontology.

### 1. H-A loops

A direct human-AI loop with optional direct review, reflection, or correction.

### 2. H-A-M loops

A human-AI loop with an additional mechanism or machine participant that participates in state transition, measurement, enforcement, or escalation.

### 3. Multi-human systems

Two or more human roles interact with AI or machine participants. Examples include reviewer, proposer, decision-maker, recorder, and escalation authority roles.

### 4. Multi-agent systems

One or more human roles interact with multiple artificial-agent roles or role-specialized AI components.

### 5. Mixed architectures

Architectures combine humans, artificial participants, deterministic mechanisms, tools, gates, and external information sources. A complete topology must define whether every element is a participant or an instrument.

### Candidate topologies

- `H+A`
- `H+A+G`
- `H+AA`
- `H+AA+G`
- `HH+A`
- `HH+AA`
- `HH+AA+G`

Where:

- `A` represents an artificial-intelligence role;
- `H` represents a human role;
- `AA` represents multiple artificial-agent roles, not necessarily multiple model instances;
- `G` represents governance through gates;
- `M` represents an additional mechanism or machine participant.

## VI. Evaluation

Gate effectiveness should be evaluated without assuming that every intervention improves epistemic calibration.

### CCR — Confidence Creep Rate

Measure unjustified confidence upgrades relative to confidence statements. Gate hypotheses include whether confidence gates reduce upgrades that lack new evidence.

### ADR — Assumption Drift Rate

Measure unsupported assumptions relative to total claims. Gate hypotheses include whether assumption and evidence gates reduce the entry or strengthening of unsupported assumptions.

### CAS — Calibration Alignment Score

Measure mismatch between evidence strength and confidence strength. Gate hypotheses include whether governed loops improve evidence-confidence alignment.

### BCE — Bidirectional Correction Events

Measure instances in which either side detects and repairs unsupported reasoning. BCE should be reported by direction and outcome, not as an unconditional good.

Additional process measures include:

- gate activation rate;
- false PASS rate;
- false FAIL rate;
- override frequency;
- override success rate;
- unresolved contradiction count;
- premature convergence count;
- time to repair;
- creativity and idea-generation preservation;
- participant burden.

## VII. Experimental validation

### 1. Ungoverned systems

Establish baseline behavior in normal AI use and reflection-only conditions. These baselines help distinguish protocol effects from participant and model effects.

### 2. Governed systems

Compare one or more gate implementations with ungoverned baselines. Gates should be evaluated by their structure, trigger, threshold, and behavior rather than as a unitary “governance” intervention.

### 3. Gate effectiveness

Estimate whether each gate changes relevant behavior. Report:

- sensitivity to gate-relevant failures;
- specificity to those failures;
- intervention effect;
- false intervention rate;
- burden and latency;
- participant and model variability.

### 4. Failure analysis

Analyze negative findings and failure modes:

- missing activation;
- misclassification;
- threshold failure;
- gate gaming;
- needless interruption;
- unjustified override;
- premature convergence;
- unresolved contradiction;
- cascading gate failure.

A gate can appear effective in aggregate while failing specific participants or contexts. Reports should preserve disaggregated results where privacy and sample-size constraints permit.

## VIII. Operational requirements

Before experimental use, preregister:

1. gate trigger and input definition;
2. threshold and state-transition rule;
3. override authority and record;
4. failure criterion;
5. unit of analysis;
6. primary and secondary outcomes;
7. inter-rater reliability procedure;
8. exclusion and missing-data rules;
9. ethics and privacy controls;
10. null and negative finding reporting.

## IX. Current position

Gate theory is a proposed architecture vocabulary and hypothesis-generation framework. It does not yet establish that gates improve calibration, that governance is separable from framework, or that calibration is a property of an architecture rather than participants.
