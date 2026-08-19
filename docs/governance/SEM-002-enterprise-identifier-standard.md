---
id: SEM-002
title: Enterprise Identifier Standard
type: standard
status: draft
version: 0.1.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - semantic
  - identifier
  - governance
  - knowledge-graph
related:
  - SEM-001
  - CON-001
---

# SEM-002 — Enterprise Identifier Standard

## Purpose

Define lean rules for persistent identifiers used by TPAD enterprise knowledge artefacts and concepts.

## Scope

This standard applies to identifiers recorded in governed repository artefacts. All governed TPAD identifiers are persistent identifiers: they preserve the identity of the governed object across title, location, lifecycle, and implementation changes. The standard preserves existing identifiers and provides a consistent basis for future cross-references and knowledge-graph use.

## Rules

1. An identifier is persistent, unique within its governed scope, and never reassigned to a different object.
2. Identifiers use uppercase letters, digits, and hyphens only.
3. Numeric sequences use three digits, beginning at `001` within the applicable identifier family.
4. Existing identifiers remain valid; do not rename an identifier solely to change its format.
5. A reference uses the identifier as the stable key and may use the title as a human-readable label.
6. The identifier is recorded in the document metadata and, where relevant, in a catalog or register.

## Existing Identifier Patterns

The repository already uses the following compatible patterns:

| Pattern | Use | Examples |
|---|---|---|
| `<PREFIX>-<NNN>` | A concise identifier family. | `SEM-001`, `CON-001`, `QG-001` |
| `<PREFIX>-<CLASS>-<NNN>` | An identifier family with an additional classification or domain token. | `GOV-MDS-001`, `ADR-GOV-001`, `GLO-TERM-001` |

Select the pattern already used by the relevant identifier family. New identifier families must be introduced through applicable governance rather than by silently changing an existing family.

## Identifier Assignment

| Step | Requirement |
|---|---|
| Define | Confirm the object has business value and a distinct semantic purpose. |
| Check | Search the repository and applicable register or catalog for an existing identifier. |
| Assign | Allocate the next available sequence in the selected family. |
| Record | Add the identifier to metadata and the relevant catalog, register, or record. |
| Retain | Keep the identifier visible when the object is superseded or archived. |

## Identifier Lifecycle

An identifier has a lifecycle independent of the lifecycle of the document or artefact that records it.

```text
Reserved → Assigned → Active → Superseded or Retired
```

| State | Meaning |
|---|---|
| Reserved | An identifier is held for an approved, distinct object but is not yet recorded as its active identifier. |
| Assigned | The identifier is recorded against one object and must not be assigned to another object. |
| Active | The identified object is in active use or under active governance. |
| Superseded | A successor object exists; retain the identifier and record the successor relationship. |
| Retired | The object is no longer active; retain the identifier for traceability and never reuse it. |

An identifier remains persistent in every state. Superseding, archiving, moving, or renaming an artefact does not make its identifier available for reuse.

## Cross-Reference and Knowledge-Graph Use

Identifiers are the stable join keys between documents, concepts, decisions, models, quality records, and deliverables. A reference should preserve both the identifier and the relationship context—for example, “governed by `SEM-002`” or “assessed by `QG-004`.” This supports machine extraction without requiring a specific graph technology.

## References

- [SEM-001 — Enterprise Semantic Principles](SEM-001-enterprise-semantic-principles.md)
- [CON-001 — Enterprise Concept Catalog](../information/CON-001-enterprise-concept-catalog.md)
- [Metadata Standard](metadata-standard.md)
