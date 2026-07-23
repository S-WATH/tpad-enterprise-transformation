---
id: GOV-GMP-001
title: Governance Map
type: guideline
status: draft
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - governance
  - quality
  - architecture
  - traceability
---

# Governance Map

## Purpose

Explain how project bootstrap, architectural decisions, governance controls, quality controls, standards, models, and deliverables relate within the TPAD Enterprise Transformation repository.

## Relationship Overview

Project Bootstrap packages (PBs) establish the project baseline, working principles, current phase, and immediate direction. Governance turns those principles into controlled rules, roles, and lifecycle practices. ADRs record material architectural or governance decisions that change or clarify those controls.

Quality applies governance through Quality Gates (QGs) and Quality Reviews (QRs). A QG defines readiness criteria; a QR records the evidence, result, findings, and actions. Standards define the reusable requirements that governed artefacts must follow. Models represent the enterprise objects and relationships governed by those standards. Deliverables are controlled outputs derived from models and standards, assessed through applicable quality controls, and approved and released through the established document lifecycle.

## Hierarchy

```text
PB — Project Bootstrap
└── Governance
    ├── ADR — material architecture and governance decisions
    ├── Standards — reusable rules, metadata, types, and lifecycle
    ├── Quality
    │   ├── QG — readiness criteria
    │   └── QR — assessment evidence and outcome
    └── Models — enterprise objects and relationships
        └── Deliverables — governed outputs, baselines, and releases
```

## Control Flow

1. A PB establishes the baseline and working principles for the programme.
2. Governance standards define how repository artefacts are structured, controlled, reviewed, approved, and released.
3. An ADR records a material decision that affects architecture or governance and provides traceable rationale.
4. Models apply standards to represent enterprise concepts, relationships, and design decisions.
5. Deliverables are produced from governed models and documentation.
6. QGs and QRs verify that deliverables, baselines, and releases meet applicable standards before they proceed through the document lifecycle.

## Key References

- [Project Bootstrap Package](../../bootstrap/PB-001-project-bootstrap-package-v1.0.md)
- [Quality Management Framework](quality/QUALITY-MANAGEMENT-FRAMEWORK.md)
- [Quality Gate Register](quality/QUALITY-GATE-REGISTER.md)
- [Quality Review Standard](quality/QUALITY-REVIEW-STANDARD.md)
- [Document Lifecycle Standard](document-lifecycle-standard.md)
- [Document Type Standard](document-type-standard.md)
- [Metadata Standard](metadata-standard.md)
