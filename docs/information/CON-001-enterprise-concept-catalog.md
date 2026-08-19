---
id: CON-001
title: Enterprise Concept Catalog
type: reference
status: draft
version: 0.1.0
domain: information
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - semantic
  - concept-catalog
  - information
  - knowledge-graph
related:
  - SEM-001
  - SEM-002
---

# CON-001 — Enterprise Concept Catalog

## Purpose

Provide the initial controlled vocabulary for enterprise semantic work. The catalog is a lean, cross-reference-ready source for concept names, definitions, and relationships.

## Catalog Rules

- One row represents one concept and one intended meaning.
- Definitions are concise and avoid circular wording.
- Relationships reference stable identifiers where they exist.
- This catalog records concepts; it does not replace the governing standard or source artefact.

## Concepts

| Concept | Concept class | Type | Definition | Governing / source | Related concepts |
|---|---|---|---|---|---|
| Enterprise Concept | Semantic foundation | Semantic object | A defined unit of business, governance, architecture, or information meaning used consistently across the enterprise. | [SEM-001](../governance/SEM-001-enterprise-semantic-principles.md) | Identifier; Relationship; Model |
| Identifier | Semantic attribute | Semantic attribute | A persistent, unique key used to refer to a governed object or concept. | [SEM-002](../governance/SEM-002-enterprise-identifier-standard.md) | Enterprise Concept; Cross-reference |
| Concept Catalog | Information asset | Information reference | A controlled collection of enterprise concepts, definitions, and relationships. | CON-001 | Enterprise Concept; Model |
| Relationship | Semantic connector | Semantic link | A named connection between two concepts or governed artefacts that expresses context, dependency, governance, or derivation. | [SEM-001](../governance/SEM-001-enterprise-semantic-principles.md) | Enterprise Concept; Model; Deliverable |
| Standard | Governance control | Governance artefact | A governed document that defines reusable rules or requirements for the repository or enterprise. | [GOV-DTS-001](../governance/document-type-standard.md) | Governance; Deliverable |
| Quality Gate | Quality control | Quality control | A defined set of readiness criteria and required evidence for a specific decision. | [QUALITY-GATE-REGISTER](../governance/quality/QUALITY-GATE-REGISTER.md) | Quality Review; Baseline; Release |
| Quality Review | Quality assessment | Quality record | An auditable assessment that applies one or more Quality Gates and records evidence, findings, and outcome. | [QUALITY-REVIEW-STANDARD](../governance/quality/QUALITY-REVIEW-STANDARD.md) | Quality Gate; Baseline; Release |
| Deliverable | Enterprise output | Controlled output | A governed output produced from enterprise work and progressed through applicable review, approval, baseline, or release controls. | [GOVERNANCE-MAP](../governance/GOVERNANCE-MAP.md) | Model; Standard; Quality Gate |

## Knowledge-Graph Compatibility

Each catalog row can be represented as a node with the following properties: `name`, `concept_class`, `type`, `definition`, `source`, and `status`. The “Related concepts” column supplies candidate edges that may be formalized when a relationship registry is established. The Markdown catalog remains authoritative until a governed graph implementation is adopted.

## References

- [SEM-001 — Enterprise Semantic Principles](../governance/SEM-001-enterprise-semantic-principles.md)
- [SEM-002 — Enterprise Identifier Standard](../governance/SEM-002-enterprise-identifier-standard.md)
- [Metadata Standard](../governance/metadata-standard.md)
