---
id: REL-001
title: Enterprise Relationship Model
type: information
status: draft
version: 0.1.0
domain: information
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - enterprise-architecture
  - relationship-model
  - semantic
  - knowledge-graph
related:
  - SEM-001
  - SEM-002
  - CON-001
  - GLO-001
  - OBJ-001
---

# REL-001 — Enterprise Relationship Model

## Purpose

Define the canonical, explicit relationship types used to connect Enterprise Objects. The registry provides a controlled vocabulary for relationships so that enterprise meaning is traceable and machine-readable.

## Relationship Rules

1. Every relationship is directed: its source and target are recorded in the stated order.
2. Every relationship instance uses one relationship type from this registry.
3. Every relationship instance identifies both participating objects and its source evidence.
4. Generic labels such as `related_to`, `linked_to`, `associated_with`, and `has` are not permitted because they do not state enterprise meaning.
5. Process-to-object relationships are allowed only to describe how a separately modelled Process acts on an Enterprise Object; a Process is not an Enterprise Object.
6. Relationship identifiers are persistent identifiers managed in accordance with SEM-002.

## Canonical Relationship Registry

| Identifier | Relationship | Source class | Target class | Explicit definition | Semantic Foundation trace |
|---|---|---|---|---|---|
| REL-TYP-001 | governs | Governance | Any Enterprise Object | The source establishes binding authority, direction, or control over the target. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-002 | defines | Governance or Information | Any Enterprise Object or Relationship | The source states the required meaning, rule, structure, or boundary of the target. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-003 | constrains | Governance or Business | Business, Information, or Resource | The source limits permitted scope, behaviour, use, or outcome of the target. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-004 | requires | Business or Governance | Business, Information, or Resource | The source cannot achieve its intended outcome without the target. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-005 | enables | Information or Resource | Business or Governance | The source provides knowledge or capacity that makes the target achievable. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-006 | is_composed_of | Any Enterprise Object | Same or subordinate Enterprise Object | The source is a whole whose identity includes the target as a constituent part. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-007 | is_responsible_for | Resource | Business, Governance, Information, or Resource | The source has assigned accountability for the target. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-008 | realizes | Business (Deliverable) or Resource | Business | The source provides an implemented or operational expression of the target business intent or capability. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-009 | produces | Process | Enterprise Object | The source Process creates the target object as an outcome. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-010 | consumes | Process | Enterprise Object | The source Process uses the target object as an input without changing its identity. | SEM-001; SEM-002; CON-001; GLO-001 |
| REL-TYP-011 | transforms | Process | Enterprise Object | The source Process changes the target object; the record identifies the input and resulting object as evidence. | SEM-001; SEM-002; CON-001; GLO-001 |

## Relationship Record

Each relationship instance shall record:

| Field | Requirement |
|---|---|
| Relationship identifier | Persistent identifier for the recorded relationship instance, where the relationship itself is governed. |
| Relationship type | One `REL-TYP-###` identifier from the Canonical Relationship Registry. |
| Source object | Persistent identifier and name of the source. |
| Target object | Persistent identifier and name of the target. |
| Evidence | Source artefact, decision, standard, model, or approved review that supports the relationship. |
| Status | Applicable lifecycle state. |
| Semantic trace | References to SEM-001, SEM-002, CON-001, and GLO-001. |

## Knowledge-Graph Compatibility

Each registered relationship type maps to a typed, directed edge predicate. A relationship instance uses `source_identifier`, `relationship_type`, `target_identifier`, `evidence`, and `status` properties. This supports graph use while retaining repository artefacts as the authoritative evidence.

## Semantic Foundation References

- [SEM-001 — Enterprise Semantic Principles](../governance/SEM-001-enterprise-semantic-principles.md)
- [SEM-002 — Enterprise Identifier Standard](../governance/SEM-002-enterprise-identifier-standard.md)
- [CON-001 — Enterprise Concept Catalog](../information/CON-001-enterprise-concept-catalog.md)
- [GLO-001 — Enterprise Glossary](../information/GLO-001-enterprise-glossary.md)
- [OBJ-001 — Enterprise Object Model](OBJ-001-enterprise-object-model.md)
