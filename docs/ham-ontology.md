# HAM Ontology

## Definition

HAM is a provisional taxonomy for describing active roles in a reasoning architecture:

- **H — Human:** an agent role carried out by a person.
- **A — Artificial Intelligence:** an agent role implemented through artificial intelligence.
- **M — Mechanism / Machine participant:** a participant that contributes to state transitions but is not adequately classified by H or A under the chosen frame.

The letters describe roles in a topology; they should not be interpreted as exhaustive ontological classifications.

## Role ≠ ontology

A role states what an entity does inside an architecture. Ontology states what the entity is.

Examples:

- A human may occupy a reviewer role.
- An AI may occupy an evaluator role.
- A deterministic workflow may occupy a gate role.
- A document or static checklist may extend a role without becoming a participant.

The same entity can occupy different roles across architectures, and one role can be assigned to different types of entities.

## Participant

A participant is a system element that can change subsequent system state in the reasoning loop.

Working indicators include:

- receiving system state
- processing or transforming information
- emitting a recommendation or action
- affecting subsequent decisions or observations

These indicators are not sufficient for a final definition and should not be conflated with consciousness or general agency.

## Tool

A tool extends capability but is treated as non-autonomously initiating decision flow within the current frame.

```text
Static checklist -> tool
Human-operated rule engine -> tool or instrumented participant, depending on role
Deterministic gate -> participant or component, depending on granularity
```

Classification may depend on context and the chosen unit of analysis.

## M alternatives

The name M remains unresolved. Candidate meanings:

- Machine Agent
- Mechanized Agent
- Mechanism Agent
- Mixed participant

Before M is operationalized, architecture diagrams should distinguish explanatory shorthand from a committed ontology.
