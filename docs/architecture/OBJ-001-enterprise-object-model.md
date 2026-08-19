---
id: OBJ-001
title: Enterprise Object Model
type: information
status: draft
version: 0.1.0
domain: information
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - enterprise-architecture
  - object-model
  - semantic
  - knowledge-graph
related:
  - SEM-001
  - SEM-002
  - CON-001
  - GLO-001
  - REL-001
---

# OBJ-001 — Enterprise Object Model

## Purpose

Define the canonical classification and minimum record for Enterprise Objects in the TPAD Enterprise Transformation Program. Enterprise Objects represent durable business-level things of value, control, knowledge, or capacity; they are not implementation artefacts.

## Scope and Boundary

This model classifies Enterprise Objects used to describe the enterprise. It does not define database entities, APIs, application classes, file schemas, or other implementation constructs.

Enterprise Objects are distinct from Processes:

| Enterprise Object | Process |
|---|---|
| A durable thing with identity and business meaning. | A temporal sequence of activities that acts on objects. |
| May be governed, required, enabled, produced, consumed, or transformed. | May create, consume, transform, or use objects. |
| Is classified by this model. | Is modelled separately in the process domain. |

## Canonical Object Classification

| Identifier | Object class | Definition | Examples of object types | Semantic Foundation trace |
|---|---|---|---|---|
| OBJ-CLS-001 | Business | An object that expresses enterprise purpose, value, obligation, or service intent. | Mission, Capability, Requirement, Deliverable | SEM-001; SEM-002; CON-001; GLO-001 |
| OBJ-CLS-002 | Governance | An object that establishes authority, direction, decision, policy, rule, or assurance. | Standard, Policy, ADR, Quality Gate, Quality Review | SEM-001; SEM-002; CON-001; GLO-001 |
| OBJ-CLS-003 | Information | An object that records, describes, classifies, or communicates enterprise knowledge. | Concept, Identifier, Catalog, Glossary, Model | SEM-001; SEM-002; CON-001; GLO-001 |
| OBJ-CLS-004 | Resource | An object that provides enterprise capacity for work or service delivery. | Organization, Role, Competency, Asset, Facility | SEM-001; SEM-002; CON-001; GLO-001 |

The class identifies the primary enterprise meaning of an object. An object has one primary class; additional characteristics are represented through explicit relationships, not by assigning multiple primary classes.

## Minimum Object Record

Every Enterprise Object recorded in the repository shall include:

| Field | Requirement |
|---|---|
| Identifier | A persistent identifier assigned in accordance with SEM-002. |
| Preferred name | A canonical, human-readable name; glossary terms are used where available. |
| Object class | One of Business, Governance, Information, or Resource. |
| Definition | A concise business-level statement of what the object is. |
| Status | The applicable lifecycle state. |
| Authority | The accountable owner or governing source. |
| Semantic trace | References to SEM-001, SEM-002, CON-001, and GLO-001. |
| Relationships | Explicit relationship types from REL-001, with identified targets. |

## Object Modelling Rules

1. Model an object only when it has distinct enterprise meaning and business value.
2. Keep objects independent of a specific system, data structure, or implementation technology.
3. Use a persistent identifier as the stable key; names and locations may change without changing identity.
4. Use canonical glossary terms where available; request a new term or concept before introducing ambiguous vocabulary.
5. Express dependencies and structure through explicit REL-001 relationship types. Do not use unspecified relationship labels.
6. Model a process separately when the subject is an activity sequence rather than a durable thing.

## Knowledge-Graph Compatibility

An Enterprise Object maps to a graph node with `identifier`, `name`, `object_class`, `definition`, `status`, and `authority` properties. REL-001 relationship instances map to typed, directed edges. The repository Markdown record remains authoritative for the object and its evidence.

## Semantic Foundation References

- [SEM-001 — Enterprise Semantic Principles](../governance/SEM-001-enterprise-semantic-principles.md)
- [SEM-002 — Enterprise Identifier Standard](../governance/SEM-002-enterprise-identifier-standard.md)
- [CON-001 — Enterprise Concept Catalog](../information/CON-001-enterprise-concept-catalog.md)
- [GLO-001 — Enterprise Glossary](../information/GLO-001-enterprise-glossary.md)
- [REL-001 — Enterprise Relationship Model](REL-001-enterprise-relationship-model.md)
