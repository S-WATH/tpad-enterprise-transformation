---
id: ADR-GOV-002
title: Introduce the MNT Identifier Family for Maintenance Transformation Artifacts
type: adr
status: approved
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-09-13
updated: 2026-09-13
tags:
  - adr
  - governance
  - identifier
  - maintenance
related:
  - SEM-002
  - DOM-001
  - AB-2.0
approved_by: Program Sponsor
approved_date: 2026-09-13
---

# ADR-GOV-002 — Introduce the MNT Identifier Family for Maintenance Transformation Artifacts

## Status

Approved — Program Sponsor approval recorded 2026-09-13.

## Context

`README.md` and both checkpoints (`TPAD-CHECKPOINT-2026-09-08`, `TPAD-CHECKPOINT-2026-09-12`) refer to `MNT-001 — Maintenance Operating Model — AS-IS Discovery` as a draft working artifact, with a defined scope and an evidence-classification scheme (E0–E4).

No `MNT`-prefixed file exists anywhere in the repository. The `MNT` prefix has not been introduced through governance: `bootstrap/ADR-INDEX.md` and `docs/adr/` contain only `ADR-GOV-001`.

The Enterprise Identifier Standard (`SEM-002`) states that new identifier families must be introduced through applicable governance rather than by silently changing or extending an existing family. Referring to `MNT-001` by name in narrative documents, without an approved family definition, does not satisfy this requirement, and does not itself make `MNT-001` a controlled artifact.

This gap must be closed before any `MNT`-prefixed document is created, so that the artifact is not backfilled to match narrative that already exists — which was the original problem being remediated.

## Decision

Introduce `MNT` as a governed identifier family for Maintenance Transformation artifacts, following the existing `<PREFIX>-<NNN>` pattern (consistent with `SEM-002`, e.g. `SEM-001`, `KB-001`, `DOM-001`, `REG-001`).

Scope of the family:

- `MNT-NNN` identifies controlled artifacts describing the Maintenance Transformation workstream: AS-IS discovery, regulatory-applicability cross-checks specific to maintenance, and — only after separate approval — target-state design.
- `MNT-001` is reserved for the AS-IS Maintenance Operating Model discovery artifact already described in narrative form in the current checkpoint.
- The family does not, by itself, authorize any organizational, Post Holder, MOE/CAME, or target-state design content. That restriction remains in force regardless of this ADR's disposition.

This ADR does not approve the content of `MNT-001`. A separate document would carry the actual AS-IS findings (F1–F7) currently recorded only in narrative form, with proper frontmatter and evidence tagging (E0–E4) as already specified in the checkpoint.

## Consequences

### Positive

- Closes the identifier-governance gap before any `MNT`-prefixed file is created, preventing a controlled artifact from being backfilled to match pre-existing narrative.
- Gives the Maintenance Transformation workstream the same governed identifier discipline already applied to `SEM`, `KB`, `DOM`, and `REG`.
- Makes explicit that AS-IS discovery content belongs in a controlled artifact, not permanently in README/checkpoint narrative.

### Constraints

- Approval of this ADR is not approval of `MNT-001`'s content; `MNT-001` still requires its own draft → review → approval cycle and must remain AS-IS discovery only — no target-state or organizational design.

## Approval Record

The Program Sponsor approved this ADR on 2026-09-13. This approval authorizes introduction of the `MNT` identifier family as defined above. It does not approve `MNT-001` itself, which remains subject to its own document lifecycle and evidence review.

## Alternatives Considered

### Treat MNT-001 as already existing because it is named in README/checkpoint

Rejected. Naming an artifact in narrative documents is not equivalent to it existing as a controlled artifact, and does not satisfy the identifier-governance requirement in `SEM-002`.

### Fold maintenance AS-IS discovery into an existing identifier family (e.g. `REG-KR`)

Rejected. Maintenance AS-IS discovery is operational/organizational current-state evidence, not a regulatory knowledge record; conflating the two would blur the distinction between `D02 Regulatory & Standards` and `D05 Airworthiness & Maintenance` that `DOM-001` already establishes.

## References

- [Enterprise Identifier Standard (SEM-002)](../governance/SEM-002-enterprise-identifier-standard.md)
- [Enterprise Knowledge Domain Architecture (DOM-001)](../information/DOM-001-enterprise-knowledge-domain-architecture.md)
- [TPAD-CHECKPOINT-2026-09-12](../governance/checkpoints/TPAD-CHECKPOINT-2026-09-12.md)
- [ADR-GOV-001](ADR-GOV-001-adopt-enterprise-quality-governance-framework.md)
