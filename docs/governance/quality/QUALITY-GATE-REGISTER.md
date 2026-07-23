---
id: GOV-QGR-001
title: Quality Gate Register
type: checklist
status: draft
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - governance
  - quality
  - quality-gate
---

# Quality Gate Register

## Purpose

Register the quality gates used by the TPAD Enterprise Transformation Program and provide the authoritative location for their criteria.

## Registered Gates

| Gate | Purpose | Inputs | Outputs | Related ADR | Related Baseline | Related Standards | Owner | Status | Definition |
|---|---|---|---|---|---|---|---|---|---|
| QG-001 | Confirm repository health before it is relied upon as a baseline. | Working-tree status; branch state; manifest; bootstrap records; changelog. | Repository health result and exceptions. | None currently. | BR-1.0 and subsequent baselines. | Document Lifecycle Standard; Metadata Standard. | Repository Maintainer | Draft | [QG-001-Repository-Ready.md](gates/QG-001-Repository-Ready.md) |
| QG-002 | Confirm architecture artefacts are ready for governed review and downstream use. | Architecture artefact; upstream relationships; applicable decisions. | Architecture readiness result and actions. | Applicable ADRs, where present. | Applicable architecture baseline. | Document Type Standard; Metadata Standard; Document Lifecycle Standard. | Reviewer | Draft | [QG-002-Architecture-Ready.md](gates/QG-002-Architecture-Ready.md) |
| QG-003 | Confirm standards are complete and ready for approval. | Draft standard; related governance artefacts; review evidence. | Standards readiness result and actions. | Applicable ADRs for governed changes. | Applicable governance baseline. | Document Type Standard; Metadata Standard; Document Lifecycle Standard. | Reviewer | Draft | [QG-003-Standards-Ready.md](gates/QG-003-Standards-Ready.md) |
| QG-004 | Confirm a release package is complete, traceable, and ready for release. | QG-001 result; approved artefacts; release scope; changelog. | Release readiness result and release evidence. | Applicable ADRs included in release scope. | Release baseline. | Document Lifecycle Standard; Metadata Standard; Quality Management Framework. | Repository Maintainer | Draft | [QG-004-Release-Ready.md](gates/QG-004-Release-Ready.md) |

## Register Rules

- A gate is registered when its definition is available in this register; its status follows the document lifecycle.
- Gate criteria and evidence are defined in the linked gate document.
- A gate result is recorded in the related Quality Review and linked to the relevant work, checkpoint, baseline, or release record; this register is not a log of individual results.
- Changes to a gate follow the document lifecycle and applicable governance standards.
