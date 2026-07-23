---
id: QG-004
title: Release Ready
type: checklist
status: draft
version: 1.0.0
domain: governance
owner: Repository Maintainer
created: 2026-07-23
updated: 2026-07-23
tags:
  - governance
  - quality
  - release
  - quality-gate
---

# QG-004 — Release Ready

## Objective

Confirm that a release package is complete, approved as required, traceable, and ready to be released through the repository.

## Entry Condition

A set of governed artefacts is proposed for release.

## Criteria and Required Evidence

| Criterion | Pass condition | Evidence |
|---|---|---|
| Repository health | QG-001 has passed for the release baseline. | QG-001 result. |
| Scope complete | The release contents and exclusions are identified. | Release note, checkpoint, or release record. |
| Lifecycle complete | Each included artefact has completed the approval steps required by the Document Lifecycle Standard. | Artefact status and approval evidence. |
| Traceability complete | Included artefacts, decisions, and applicable requirements or standards can be traced. | Release inventory and links. |
| Changelog complete | Material release changes are recorded in the changelog. | Relevant `bootstrap/CHANGELOG.md` entry. |

## Outcome

- **Pass:** the release may be committed and pushed as the official repository release.
- **Conditional pass:** only an approved, time-bound post-release action remains; it is visible in the release record.
- **Fail:** release scope, lifecycle evidence, traceability, repository health, or changelog evidence is incomplete.

## Record

Record the result with the release note or checkpoint, including release baseline, assessor, evidence locations, exceptions, and follow-up actions.
