---
id: GOV-QMF-001
title: Quality Management Framework
type: standard
status: draft
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - governance
  - quality
  - quality-management
---

# Quality Management Framework

## Purpose

Establish a consistent, evidence-based approach for assuring the quality of TPAD Enterprise Transformation repository artefacts. The framework applies the existing Repository-first and Standard-first principles: the repository is the authoritative record, and quality is demonstrated through governed, reviewable evidence.

## Scope

This framework applies to governance, architecture, standards, and release artefacts held in the repository. It governs readiness checks and their recorded evidence; it does not replace the document lifecycle, metadata, document-type, or architecture-governance standards.

## Principles

- **Repository-first:** quality evidence is recorded and traceable in the repository.
- **Standard-first:** existing approved standards define the criteria used by each gate.
- **Evidence-based:** a gate passes only when its stated evidence is available and verifiable.
- **Proportionate:** gates assess readiness for the decision at hand without introducing unnecessary process.
- **Traceable:** each decision, exception, and corrective action is linked to the affected artefact or gate.
- **Continuous:** lessons from gate outcomes improve criteria and guidance through normal governance.

## Roles

| Role | Quality responsibility |
|---|---|
| Author | Prepares artefacts, performs applicable checks, and provides evidence. |
| Reviewer | Verifies completeness, conformance, and the evidence supporting a gate result. |
| Repository Maintainer | Maintains gate records and repository-quality conformance. |
| Program Sponsor | Approves documents and releases where required by the document lifecycle. |

## Quality Lifecycle

1. **Plan** — identify the artefact, applicable standards, quality gates, and required review before work begins.
2. **Prepare** — create or update the artefact in accordance with the applicable standards and preserve its traceability.
3. **Check** — gather and verify the evidence defined by the relevant quality gate.
4. **Review** — conduct a Quality Review (QR), record the result, findings, exceptions, corrective actions, and decision.
5. **Approve and baseline** — progress the artefact through the established document lifecycle; where a checkpoint is established, record the approved scope as a baseline.
6. **Release** — apply QG-004 and release approved, traceable baseline content through the repository.
7. **Learn** — use review and gate outcomes to improve criteria, guidance, and quality practice through governed change.

## Quality Gates

The Quality Gate Register is the authoritative index of gates. A gate is a readiness decision, not a replacement for document approval. The initial gates are:

| Gate | Purpose | Applies before |
|---|---|---|
| QG-001 Repository Ready | Confirm repository health. | Work is relied upon as a synchronized repository baseline. |
| QG-002 Architecture Ready | Confirm architecture artefacts are ready for governed review. | An architecture decision or downstream elaboration. |
| QG-003 Standards Ready | Confirm a standard is ready for approval. | Standard approval or release. |
| QG-004 Release Ready | Confirm a release package is complete and traceable. | Release. |

The individual gate documents define scope, criteria, evidence, and outcomes. Gate results must be retained with the related Quality Review, checkpoint, or release evidence; a failed gate must identify corrective action before proceeding.

## Relationship Between Gates, Reviews, Baselines, and Releases

| Control | Role | Relationship |
|---|---|---|
| Quality Gate (QG) | Defines readiness criteria. | A QG specifies what evidence must be checked for a particular readiness decision. |
| Quality Review (QR) | Records assessment and decision. | A QR applies one or more QGs, evaluates the evidence, and records findings, outcome, exceptions, and actions. |
| Baseline | Establishes an approved reference point. | A baseline records the approved scope after the required QR and document-lifecycle approval; QG-001 confirms the repository state supporting it. |
| Release | Makes approved baseline content official. | A release is assessed with QG-004 and must reference the applicable baseline, QR evidence, and changelog entry. |

Quality gates do not replace reviews or approval. A gate supplies criteria; a QR supplies the auditable assessment; the document lifecycle supplies approval authority; and a baseline or release records the resulting controlled state.

## Continuous Improvement

Continuous improvement follows a closed, evidence-based cycle:

1. **Collect** — gather QG results, QR findings, exceptions, corrective actions, and recurring issues.
2. **Analyse** — identify trends, root causes, duplicated controls, and unclear criteria.
3. **Improve** — propose proportionate changes to guidance, gate criteria, templates, or working practices.
4. **Approve** — progress changes through the applicable governance and document lifecycle.
5. **Verify** — confirm through subsequent QRs that the change resolved the intended issue without reducing traceability or conformance.

The Repository Maintainer coordinates this cycle at appropriate checkpoints. Improvements must be recorded in the repository and follow existing governance. Changes to document types or metadata fields remain subject to ADR control under the applicable standards.
