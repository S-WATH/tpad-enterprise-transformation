---
id: QG-001
title: Repository Ready
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
  - repository
  - quality-gate
---

# QG-001 — Repository Ready

## Objective

Confirm that the repository is in a healthy, synchronized state before it is used as a reliable working baseline or as evidence for a downstream quality gate.

## Entry Condition

A repository baseline, checkpoint, review, or release requires a health confirmation.

## Criteria and Required Evidence

| Criterion | Pass condition | Evidence |
|---|---|---|
| Working Tree Clean | No uncommitted, staged, or untracked changes are present unless an approved exception is recorded. | `git status --short` output or equivalent recorded check. |
| Branch synchronized | The working branch is synchronized with its designated upstream baseline. | Branch and synchronization check recorded by the Repository Maintainer. |
| Manifest valid | `bootstrap/PROJECT-MANIFEST.yaml` is syntactically valid and represents the intended current baseline. | Validation result and reviewed manifest. |
| Bootstrap synchronized | Bootstrap records consistently identify the current baseline, phase, and next work. | Review of bootstrap manifest, foundation, current state, roadmap, and changelog. |
| Changelog updated | The changelog records the material baseline or release change being assessed. | Relevant `bootstrap/CHANGELOG.md` entry. |

## Outcome

- **Pass:** all criteria pass and evidence is retained.
- **Conditional pass:** a time-bound, approved exception is recorded with owner and corrective action.
- **Fail:** one or more criteria fail or evidence is absent; resolve the issue before relying on the repository baseline.

## Record

Record the date, assessor, outcome, evidence location, exceptions, and corrective actions with the associated checkpoint, review, or release record.
