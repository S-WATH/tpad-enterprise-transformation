---
id: ADR-GOV-001
title: Adopt Enterprise Quality Governance Framework
type: adr
status: approved
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-09-13
tags:
  - adr
  - governance
  - quality
approver: Program Sponsor
---

# ADR-GOV-001 — Adopt Enterprise Quality Governance Framework

## Status

Approved — Program Sponsor approval recorded 2026-09-13.

## Context

TPAD applies Repository-first and Standard-first principles: the repository is the authoritative record for governed artefacts, their relationships, and their evidence. Existing governance standards define document metadata, document types, and the document lifecycle, but they do not provide a unified framework for assessing repository, architecture, standards, and release readiness.

The Enterprise Quality Governance framework introduces an evidence-based quality-management framework, policy, quality-gate register, Quality Review (QR) standard, and four initial quality gates. It must complement the existing document lifecycle and architecture governance without creating a separate architecture or bypassing established approval authority.

## Decision

Adopt the Enterprise Quality Governance framework under `docs/governance/quality/` as the governed location for quality-management artefacts.

The framework shall:

- use Quality Gates (QGs) to define readiness criteria and evidence;
- use Quality Reviews (QRs) to record assessment results, findings, actions, and recommendations;
- preserve the existing Document Lifecycle Standard as the authority for document approval and release;
- apply QG-001 for repository readiness and QG-004 for release readiness;
- maintain traceability from quality gates to applicable standards, ADRs, baselines, and release evidence.

## Consequences

### Positive

- Repository health and release readiness have explicit, reusable criteria.
- Quality evidence becomes reviewable and traceable in the repository.
- Architecture and standards reviews use a consistent assessment structure without replacing their existing governance.
- Baselines and releases can reference an auditable QR and QG result.

### Constraints

- Authors, reviewers, and the Repository Maintainer must retain quality evidence with the associated work.
- QG criteria and QR records add a proportionate review step before baselining or release.
- Future changes to document types or metadata fields remain subject to existing ADR controls.

## Approval Record

The Program Sponsor approved this ADR on 2026-09-13. The controlled metadata records the approver using the `approver` field defined by the Metadata Standard.

**Authority identity evidence gap:** the repository currently establishes the approval role as `Program Sponsor`, but no controlled repository document reviewed for this remediation establishes the underlying person or formal appointment instrument for that role. This gap is recorded explicitly and must not be resolved by inference or by substituting a job title or personal identity without authoritative evidence.

This approval authorizes adoption of the Enterprise Quality Governance framework as described in this ADR. It does not by itself approve the individual quality-governance artefacts referenced by the framework unless those artefacts complete their own applicable lifecycle approval.

## Alternatives Considered

### Rely only on the Document Lifecycle Standard

Rejected. The lifecycle defines status transitions and approval responsibilities, but it does not define specific readiness criteria, evidence, or review records for repository and release quality.

### Use an external quality-management system

Rejected. It would divide quality evidence from the Repository-first source of truth and reduce traceability between artefacts, decisions, and releases.

### Create separate quality processes for each domain

Rejected. Independent processes would duplicate controls and make cross-domain readiness inconsistent. A common framework with gate-specific criteria is sufficient.

## References

- [Quality Management Framework](../governance/quality/QUALITY-MANAGEMENT-FRAMEWORK.md)
- [Quality Policy](../governance/quality/QUALITY-POLICY.md)
- [Quality Gate Register](../governance/quality/QUALITY-GATE-REGISTER.md)
- [Quality Review Standard](../governance/quality/QUALITY-REVIEW-STANDARD.md)
- [Document Lifecycle Standard](../governance/document-lifecycle-standard.md)
- [Document Type Standard](../governance/document-type-standard.md)
- [Metadata Standard](../governance/metadata-standard.md)
