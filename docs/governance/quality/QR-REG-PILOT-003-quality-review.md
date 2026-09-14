---
id: QR-REG-PILOT-003
title: Quality Review — REG-PILOT-003 Regulatory Applicability Provision-Level Evidence Matrix
type: quality-review
status: draft
version: 0.1.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-09-14
updated: 2026-09-14
related:
  - REG-PILOT-003
  - REG-001
  - REG-KR-001
  - REG-PILOT-001
  - REG-PILOT-002
  - MNT-001
  - AB-2.0
---

# QR-REG-PILOT-003 — Quality Review

## 1. Review Purpose

Assess whether REG-PILOT-003 v0.1.0 is sufficiently controlled and evidence-bounded to proceed toward `Review`, and whether its provision-level applicability analysis maintains the discipline established by REG-001 and REG-PILOT-001/002.

## 2. Review Basis

The review is based on the repository version of REG-PILOT-003 v0.1.0 and the approved REG-001, REG-PILOT-002, and MNT-001 (draft). No Quality Gate (QG-001–004) is cited, consistent with established precedent (QR-REG-001, QR-REG-PILOT-001).

This review assesses internal consistency, structure, and boundary discipline. It does **not** independently re-verify the underlying Air Navigation Act or Chicago Convention citations against a controlled repository copy of those sources — no such controlled source file was found registered in the repository at the time of this review (the same gap already recorded against `HND-002`). This limitation is carried forward as an Observation below, not silently assumed away.

## 3. Review Criteria

| Criterion | Result | Observation |
|---|---|---|
| Purpose and scope explicit | PASS | States this is an applicability/evidence analysis, not a legal opinion, and does not authorize implementation. |
| Metadata Standard / Document Type Standard conformance | PASS | `type: information`, `domain: regulatory-and-standards` — matches the pattern used by REG-001, REG-KR-001, REG-PILOT-001/002. |
| Applicability taxonomy defined | PASS | Section 2 defines four canonical states (Directly relevant/retained; Not directly applicable through the civil regime; Applicability unresolved; Comparative baseline only) and three evidence-confidence levels. |
| Applicability taxonomy consistently applied | **Conditional pass** | See Observation O-001 — four matrix rows (RAE-001, RAE-013, RAE-014, RAE-015) use free-text applicability language that does not map cleanly onto the four defined categories. |
| Section 5 statutory boundary preserved | PASS | Air Navigation Act §5 is consistently treated as the civil/State-Police exclusion boundary, consistent with REG-PILOT-002's prior chain analysis. |
| Civil maintenance provisions not auto-imposed | PASS | Sections 4 and 6.2 explicitly state civil maintenance provisions (§§41/77–104) are not confirmed TPAD obligations and must not be treated as such without a separate applicability basis. |
| MNT-001 findings correctly reframed | PASS | Section 5 maps each MNT-001 finding (F1–F7) to a regulatory implication without converting an evidence/control gap into a finding of legal non-compliance — matches MNT-001's own findings register exactly, no drift. |
| Source/citation traceability | **Conditional pass** | See Observation O-002 — citations are specific (document, page, section) but the underlying source PDFs are not confirmed as controlled repository artifacts, so this review cannot independently re-verify exact provision text. |
| Legal-opinion boundary control | PASS | Explicit disclaimer in Section 1 and Section 7; matches the discipline already established in REG-001 and REG-PILOT-001/002. |
| Relationship/dependency integrity | PASS | `related` metadata correctly lists REG-001, REG-KR-001, REG-PILOT-001, REG-PILOT-002, MNT-001, AB-2.0; all are real, existing controlled artifacts. |
| Next controlled actions bounded | PASS | Section 8 identifies a specific next discovery task (State/Police maintenance and airworthiness regime) rather than an open-ended scope expansion. |
| Lifecycle status accuracy | PASS | `status: draft`; Section 9 states no approval record is present. |

## 4. Findings

### Finding F-001 — No blocking finding

No blocking quality finding was identified for progression toward `Review`.

### Observation O-001 — Applicability category labels not consistently applied

Section 2 defines four canonical applicability categories. In the Section 3 matrix, most rows cite one of these categories verbatim (e.g. RAE-002 "Directly relevant / retained"; RAE-006 "Applicability unresolved"; RAE-016 "Comparative baseline only"). Four rows use free-text phrasing instead:

- RAE-001 — "Direct statutory boundary" (a fifth, undefined term, rather than one of the four canonical categories);
- RAE-013 — "International normative boundary / comparative baseline" (mixes an undefined term with a partial match to "Comparative baseline only");
- RAE-014 — "Directly relevant as international State-aircraft classification baseline" (mixes "Directly relevant" with "baseline" language from a different category);
- RAE-015 — "Relevant for TPAD international operations" (does not clearly map to any of the four categories).

The underlying analysis in each of these rows is substantively sound and consistent with the rest of the matrix; this is a labeling-discipline gap, not a wrong conclusion. It is more than cosmetic, though — RAE-001 is the row that establishes the core Section 5 statutory boundary the rest of the matrix depends on, so leaving it outside the defined taxonomy creates real ambiguity for anyone filtering the matrix by category. Recommend tagging each row with one of the four canonical category labels verbatim, with any additional context appended as further explanation, before this document is submitted for `Approved` status.

### Observation O-002 — Source documents not confirmed as controlled repository artifacts

REG-PILOT-003 cites specific pages and sections of the consolidated Air Navigation Act and the Chicago Convention. Neither source file was found registered as a controlled artifact in the repository during this review — this mirrors the same gap already recorded in `HND-002` ("source file not available in the local repository at registration time"). This review is therefore unable to independently re-verify the cited provision text; it can only confirm that the matrix's *internal* reasoning (how it applies §5, how it treats the maintenance provisions) is consistent and disciplined. Recommend registering the source documents (or verified extracts/checksums) as controlled evidence before treating any RAE-row citation as `High`-confidence, authoritative source evidence for a future `Approved` baseline. This is the same class of gap as the pending Program Sponsor identity and QG-scope items already logged as governance debt.

### Observation O-003 — Carried governance debt (no new content)

The QG-scope gap and QR-numbering non-conformance already recorded in `bootstrap/CHANGELOG.md` apply equally to this QR. No new instance of either issue is introduced by REG-PILOT-003 itself; this entry cross-references rather than restates them.

## 5. Quality Decision

**Result: PASS — proceed toward `Review`, conditional on Observations O-001 and O-002 being resolved before `Approved` status is requested.**

REG-PILOT-003 v0.1.0 demonstrates disciplined provision-level analysis, correctly preserves the statutory State/Police boundary, and correctly avoids converting MNT-001's evidence gaps into compliance findings.

This decision does not:

- constitute a legal opinion or confirm any provision's applicability to TPAD;
- approve any maintenance organisation, post-holder authority, or civil-standard adoption;
- validate the underlying source citations independently (see Observation O-002); or
- constitute the Program Sponsor approval required by the Document Lifecycle Standard for progression beyond `Review`.

## 6. Next Controlled Action

Move REG-PILOT-003 to `status: review` administratively. Resolve Observations O-001 (category-label consistency) and O-002 (source-document registration) before requesting `Approved` status. Do not begin a third regulatory or maintenance deliverable until MNT-001 and REG-PILOT-003 have both cleared `Review`.
