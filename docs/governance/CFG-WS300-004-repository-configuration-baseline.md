---
id: CFG-WS300-004
title: Repository Configuration Baseline
type: reference
status: approved
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-08-19
updated: 2026-08-19
tags:
  - repository
  - configuration
  - baseline
  - ws-300
related:
  - STR-WS300-003
  - QG-001
---

# CFG-WS300-004 — Repository Configuration Baseline

## Record

| Field | Value |
|---|---|
| Document ID | CFG-WS300-004 |
| Status | Approved |
| Sprint | WS-300 |
| Architecture Baseline | AB-2.0 |
| Architecture Freeze | Active |
| Scope | Repository Configuration Baseline |

## Purpose

Record the approved WS300-004 repository configuration baseline. This document records the existing repository configuration and deferred configuration matters only. It does not establish or modify an architecture baseline.

## Existing Configuration Baseline

| Configuration area | Baseline record |
|---|---|
| Primary branch | `main` |
| Remote | `origin` |
| Version-control system | Git |
| Ignore configuration | The existing `.gitignore` excludes `.DS_Store`. |
| Metadata configuration | [Metadata Standard](metadata-standard.md) defines the repository metadata fields, allowed statuses, domains, and field-naming rules. |
| Naming configuration | [Document Type Standard](document-type-standard.md) requires one document type per file and supports the repository's governed document naming and identification practice. |
| Quality configuration | [Quality Management Framework](quality/QUALITY-MANAGEMENT-FRAMEWORK.md), [Quality Gate Register](quality/QUALITY-GATE-REGISTER.md), and [Repository Ready](quality/gates/QG-001-Repository-Ready.md) provide the existing quality configuration. |

## Deferred Configuration Items

The following items are deferred and are not configuration requirements introduced by WS300-004:

| Deferred item | Recorded disposition |
|---|---|
| Legacy bootstrap configuration conflict | Deferred. Committed bootstrap records identify `BR-1.0`, `CP-004`, and `WS-001`, which conflicts with the supplied AB-2.0 / Phase 3 execution state. This document does not resolve the conflict. |
| Phase 2 artifact synchronization | Deferred. The six Phase 2 artifacts remain local and untracked; repository evidence is insufficient to verify them as an approved Phase 2 baseline. |
| Baseline synchronization | Deferred to a subsequent controlled activity with the required repository evidence. |
| CI/CD and GitHub Actions | Deferred; no CI/CD or GitHub Actions configuration is introduced. |
| Branching strategy | Deferred; no branching strategy is introduced. |
| CODEOWNERS | Deferred; no CODEOWNERS configuration is introduced. |
| Automation | Deferred; no automation is introduced. |

## Scope Boundary

WS300-004 does **not** authorize:

- baseline synchronization;
- architectural change;
- repository-structure change;
- bootstrap metadata changes;
- Phase 2 artifact synchronization;
- CI/CD, GitHub Actions, branching-strategy, CODEOWNERS, or automation configuration.

## References

- [Repository Structure Baseline Assessment](STR-WS300-003-repository-structure-baseline-assessment.md)
- [Metadata Standard](metadata-standard.md)
- [Document Type Standard](document-type-standard.md)
- [Document Lifecycle Standard](document-lifecycle-standard.md)
- [Quality Management Framework](quality/QUALITY-MANAGEMENT-FRAMEWORK.md)
- [Quality Gate Register](quality/QUALITY-GATE-REGISTER.md)
- [Repository Ready](quality/gates/QG-001-Repository-Ready.md)
