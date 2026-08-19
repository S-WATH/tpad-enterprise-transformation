---
id: GLO-001
title: Enterprise Glossary
type: reference
status: draft
version: 0.1.0
domain: information
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - glossary
  - semantic
  - information
  - knowledge-graph
related:
  - SEM-001
  - SEM-002
  - CON-001
---

# GLO-001 — Enterprise Glossary

## Purpose

Provide the controlled, canonical vocabulary used in TPAD enterprise artefacts. This glossary maps terms to concepts in CON-001; CON-001 remains the authoritative source of concept definitions.

## Scope

GLO-001 records preferred terms, permitted synonyms, acronyms, and deprecated terms. Each glossary term has a persistent `GLO-TERM-###` identifier. The glossary does not create concepts or repeat their definitions.

## Term Status

| Status | Meaning | Usage |
|---|---|---|
| Preferred | Canonical term for new and revised artefacts. | Use by default. |
| Synonym | Permitted alternative to a preferred term. | Map to the canonical concept; prefer the preferred term in titles and metadata. |
| Acronym | Abbreviation for a preferred term. | Expand on first use in a document. |
| Deprecated | Term retained for interpretation of legacy material. | Do not use in new or revised artefacts; use its replacement. |

## Canonical Vocabulary

| Identifier | Term | Domain | Language | Status | Canonical term | Concept reference | Authority | Usage note |
|---|---|---|---|---|---|---|---|---|
| GLO-TERM-001 | Enterprise Concept | information | English | Preferred | Enterprise Concept | [CON-001: Enterprise Concept](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use for a controlled unit of enterprise meaning. |
| GLO-TERM-002 | Identifier | information | English | Preferred | Identifier | [CON-001: Identifier](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use when referring to a stable key. |
| GLO-TERM-003 | Persistent Identifier | information | English | Synonym | Identifier | [CON-001: Identifier](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Permitted where persistence needs emphasis. |
| GLO-TERM-004 | PID | information | English | Acronym | Identifier | [CON-001: Identifier](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Expand as “Persistent Identifier” on first use. |
| GLO-TERM-005 | Concept Catalog | information | English | Preferred | Concept Catalog | [CON-001: Concept Catalog](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use for the controlled collection of concepts. |
| GLO-TERM-006 | Relationship | information | English | Preferred | Relationship | [CON-001: Relationship](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use only for an explicit named connection. |
| GLO-TERM-007 | Standard | governance | English | Preferred | Standard | [CON-001: Standard](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use for a governed reusable rule set. |
| GLO-TERM-008 | Quality Gate | governance | English | Preferred | Quality Gate | [CON-001: Quality Gate](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use for readiness criteria and evidence. |
| GLO-TERM-009 | QG | governance | English | Acronym | Quality Gate | [CON-001: Quality Gate](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Expand on first use. |
| GLO-TERM-010 | Quality Review | governance | English | Preferred | Quality Review | [CON-001: Quality Review](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use for the auditable assessment record. |
| GLO-TERM-011 | QR | governance | English | Acronym | Quality Review | [CON-001: Quality Review](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Expand on first use. |
| GLO-TERM-012 | Deliverable | information | English | Preferred | Deliverable | [CON-001: Deliverable](CON-001-enterprise-concept-catalog.md) | TPAD Enterprise Transformation Team | Use for a controlled output of enterprise work. |

## Deprecated Terms

No deprecated terms are registered in version 0.1.0. When a term is deprecated, retain its row with `Deprecated` status, identify the preferred replacement, and preserve the concept reference for traceability.

## Knowledge-Graph Compatibility

Each glossary row can be represented as a term node with `identifier`, `term`, `domain`, `language`, `status`, `canonical_term`, and `authority` properties. The Concept reference provides a `denotes` relationship from the term to the corresponding CON-001 concept. This preserves a machine-readable distinction between vocabulary and concept definition without requiring a graph platform.

## References

- [SEM-001 — Enterprise Semantic Principles](../governance/SEM-001-enterprise-semantic-principles.md)
- [SEM-002 — Enterprise Identifier Standard](../governance/SEM-002-enterprise-identifier-standard.md)
- [CON-001 — Enterprise Concept Catalog](CON-001-enterprise-concept-catalog.md)
