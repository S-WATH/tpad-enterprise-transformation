---
id: GOV-QRS-001
title: Quality Review Standard
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
  - quality-review
---

# Quality Review Standard

## Purpose

Define the Quality Review (QR) as the auditable review record used to assess evidence against applicable Quality Gates (QGs), record quality findings and decisions, and support approval, baselining, and release.

## Scope

This standard applies when a governed artefact, baseline, or release needs a recorded quality assessment. A QR supplements, but does not replace, the review and approval steps in the Document Lifecycle Standard.

## QR Numbering

QR records use the format `QR-<three-digit-sequence>`, beginning with `QR-001`. Allocate numbers sequentially and do not reuse a retired or superseded identifier. The QR identifier remains stable even if the related artefact changes title or location.

## Relationship Between QR and QG

- A **Quality Gate** defines the criteria and required evidence for one readiness decision.
- A **Quality Review** applies one or more gates to a defined scope and records the assessment.
- One QR may assess multiple QGs when they apply to the same scope; each assessed QG must have a distinct result and evidence reference.
- A QG does not approve an artefact. The QR informs the existing lifecycle approval decision by the appropriate role.

## Required Evidence

Each QR must identify:

| Evidence item | Requirement |
|---|---|
| Review scope | The artefact, baseline, or release being assessed, including version or commit reference where applicable. |
| Applicable QGs | Each gate assessed and the reason it applies. |
| Criteria results | Pass, conditional pass, or fail for every applicable criterion. |
| Evidence references | Repository links, commit references, validation outputs, or other traceable sources supporting each result. |
| Findings and actions | Non-conformances, exceptions, corrective actions, owner, and target date. |
| Decision | Overall QR recommendation and any conditions for approval, baselining, or release. |
| Participants | Author, reviewer, and approver where applicable. |

Evidence must be sufficient for an independent reviewer to understand what was checked and why the recorded conclusion was reached.

## Approval Workflow

1. The **Author** prepares the scope and evidence and requests a QR.
2. The **Reviewer** assesses the applicable QGs, records results and findings, and recommends pass, conditional pass, or fail.
3. The **Author** resolves findings or records a proposed exception and corrective action.
4. The **Program Sponsor** approves the artefact when required by the Document Lifecycle Standard; approval is not implied by a QR pass.
5. The **Repository Maintainer** confirms required repository evidence and preserves the QR record with the associated work, baseline, or release.

## QR Outcomes

| Outcome | Meaning |
|---|---|
| Pass | All applicable gate criteria pass; the work may proceed to its required lifecycle approval or next governed step. |
| Conditional pass | Non-blocking gaps have an explicit owner, action, and target date; approval authority decides whether the conditions are acceptable. |
| Fail | A blocking criterion fails, required evidence is absent, or a material non-conformance remains unresolved. |

## Records and Retention

QR records and their evidence are repository artefacts. They must remain traceable to the assessed scope and must be retained in accordance with the Document Lifecycle Standard; superseded records are archived rather than deleted.
