---
id: SEM-001
title: Enterprise Semantic Principles
type: standard
status: draft
version: 0.1.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - semantic
  - governance
  - knowledge-graph
related:
  - SEM-002
  - CON-001
---

# SEM-001 — Enterprise Semantic Principles

## Purpose

Define the minimum principles for representing TPAD enterprise knowledge as reusable, traceable, and machine-readable concepts.

## Scope

These principles apply to enterprise concepts, models, governance artefacts, standards, decisions, and deliverables recorded in the repository. They guide representation; they do not introduce a new enterprise architecture or replace existing governance standards.

## Principles

| Principle | Requirement |
|---|---|
| Repository-first | The repository is the authoritative location for a concept, its definition, and its governed references. |
| One concept, one meaning | Each concept has one clear, bounded definition; distinct meanings use distinct concepts. |
| Persistent identity | A concept or governed artefact uses a stable identifier that does not change when its title, file location, or implementation changes. |
| Explicit relationships | Material relationships are named and linked rather than inferred from prose alone. |
| Context and provenance | Definitions state their scope and retain references to the governing or source artefact where applicable. |
| Human and AI readability | Use concise headings, structured metadata, stable identifiers, and unambiguous language. |
| Controlled change | Semantic changes are traceable through versioning, review, and applicable governance controls. |

## Minimum Semantic Record

For a governed concept, record at least:

| Field | Description |
|---|---|
| Identifier | Persistent, unique identifier. |
| Name | Human-readable preferred name. |
| Definition | Concise statement of what the concept means. |
| Type | The class of thing represented, such as standard, model, capability, or deliverable. |
| Status | Lifecycle state of the record. |
| Relationships | Links to related, governing, dependent, or derived concepts where known. |

This minimum record is intentionally compatible with graph-based use: identifiers can act as nodes, named relationships as edges, and metadata as node or edge properties.

## Application

- Use [SEM-002 — Enterprise Identifier Standard](SEM-002-enterprise-identifier-standard.md) when assigning or recording identifiers.
- Register foundational concepts in [CON-001 — Enterprise Concept Catalog](../information/CON-001-enterprise-concept-catalog.md).
- Add relationships when they are known and valuable; do not create speculative relationships only to fill a model.

## References

- [Metadata Standard](metadata-standard.md)
- [Document Type Standard](document-type-standard.md)
- [Document Lifecycle Standard](document-lifecycle-standard.md)
