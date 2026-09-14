# CHANGELOG

## REG-PILOT-003 Provision-Level Regulatory Applicability Matrix — 2026-09-14

### Completed

- Created `REG-PILOT-003` — Regulatory Applicability — Provision-Level Evidence Matrix as a controlled `draft` regulatory-information artifact.
- Applied provision-level analysis rather than broad civil-aviation labels, with explicit distinction between direct applicability, civil-regime non-applicability, unresolved applicability, and comparative baseline use.
- Confirmed the statutory State/Police Aviation boundary in Air Navigation Act Section 5 and the retained Section 18/1–18/3 flight-plan/rules-of-air pathway.
- Assessed maintenance/airworthiness provisions (§§41/77–41/104) as civil-regime provisions that must not be treated as confirmed TPAD Police Aviation obligations without a separate State/Police applicability basis.
- Linked the regulatory analysis to `MNT-001` findings F1–F7 without converting evidence/control gaps into findings of legal non-compliance.
- Recorded the next discovery requirement: identify the separate State/Police Aviation maintenance, airworthiness, records, defect, parts and release-authority regime.

### Control Notes

- `REG-PILOT-003` is an applicability/evidence analysis, not a legal opinion and not an implementation authorization.
- No Part-145, CAMO, MOE, CAME, Part-M or other civil maintenance concept has been declared a statutory TPAD requirement.
- No maintenance authority, post-holder authority, delegation or identity has been inferred from job titles or organisational labels.

## MNT-001 AS-IS Discovery Draft — 2026-09-14

### Completed

- Created `MNT-001` — Maintenance Operating Model — AS-IS Discovery as a controlled `draft` artifact under the newly approved `MNT` identifier family.
- Preserved the AS-IS-only boundary: no target-state operating model, organizational structure, post-holder arrangement, maintenance-release authority, MOE/CAME arrangement, or implementation solution is approved by MNT-001.
- Established E0–E4 evidence classification and recorded current-state findings F1–F7 as E1 pending documentary/cross-validation.
- Recorded evidence gaps and separated current-state observations from regulatory applicability and target-state design.

### Governance Approval & Metadata Remediation — 2026-09-13

### Completed

- Program Sponsor approval recorded for `ADR-GOV-001` — Adopt Enterprise Quality Governance Framework.
- Program Sponsor approval recorded for `ADR-GOV-002` — Introduce the MNT Identifier Family for Maintenance Transformation Artifacts.
- Corrected both ADR frontmatter records to use the Metadata Standard's `approver` field; non-standard `approved_by` and `approved_date` fields were removed.
- Recorded an explicit governance evidence gap: the repository currently establishes `Program Sponsor` as the approval role but does not establish the underlying person or formal appointment instrument for that role. No identity was inferred or substituted.
- `MNT-001` was not created as part of the ADR approval/remediation activity; it was subsequently created on 2026-09-14 under its own Draft lifecycle.

## Governance Hygiene Remediation — 2026-09-13

### Completed

- Removed AI-tool citation markers (hidden private-use Unicode control characters wrapping `cite`/`filecite` tokens) that had been committed verbatim into `REG-KR-001` and `TPAD-CHECKPOINT-2026-09-12`. Each removed marker was replaced with an explicit flag for source re-verification; no citation content was invented to replace them.
- Added mandatory YAML frontmatter (`id`, `title`, `type`, `status`, `version`, `domain`, `owner`, `created`, `updated`) to both checkpoint files, consistent with the Metadata Standard and with the Checkpoint = Baseline document-type classification.
- Set `TPAD-CHECKPOINT-2026-09-08` status to `Archived` (superseded by `TPAD-CHECKPOINT-2026-09-12`), per the Document Lifecycle Standard rule that superseded documents are archived, not deleted.

### Control Notes

- This remediation did not redesign AB-2.0, did not alter the Architecture Freeze, and did not promote the lifecycle status of any other artifact.

## Phase 3 — Enterprise Knowledge Implementation

### Completed / Controlled

- `KB-001` — Enterprise Knowledge Foundation Baseline — Approved.
- `DOM-001` — Enterprise Knowledge Domain Architecture — Approved.
- `REG-001` — Regulatory & Standards Knowledge Domain Baseline — Approved v0.2.0.
- `REG-PILOT-001` — quality review PASS / pilot continuation authorized.
- Checkpoints `TPAD-CHECKPOINT-2026-09-08` and `TPAD-CHECKPOINT-2026-09-12` recorded as controlled state/handoff references.
- `ADR-GOV-001` — Enterprise Quality Governance Framework — Approved.
- `ADR-GOV-002` — MNT Identifier Family — Approved.

### Active

- `REG-PILOT-002` — TPAD State/Police Aviation regulatory-chain analysis (Section 5 boundary, Section 16/1 Journey Log applicability).
- `REG-PILOT-003` — draft provision-level regulatory applicability matrix.
- `REG-KR-001` — draft regulatory knowledge record set.
- `MNT-001` — draft AS-IS maintenance discovery artifact.

### Control Notes

- No Phase 2 semantic artifact (`SEM-001`, `SEM-002`, `CON-001`, `GLO-001`, `OBJ-001`, `REL-001`) has been promoted beyond `draft`.
- AB-2.0 and the Architecture Freeze remain unchanged.

## WS-310 - Controlled Baseline Synchronization

### Current

- WS-310 approved as the active workstream for controlled baseline synchronization.
- WS-300 Repository Bootstrap completed.
- AB-2.0 remains the current Architecture Baseline.
- Phase 2 is recorded as completed.
- Phase 3 is recorded as ready.
- Architecture Freeze 2.0 remains active.
- WS310-006 synchronized the six approved Phase 2 artifacts into Git control without promoting their lifecycle status.
- WS310-008 reconciled the AB-2.0 Baseline Evidence Register with the repository synchronization state.

### Control Notes

- BR-1.0 remains historical evidence.
- No Architecture redesign occurred.
- No lifecycle promotion of the six Phase 2 artifacts occurred.
- Bootstrap synchronization remains a controlled activity.

## WS-002 - Enterprise Quality Governance

### Completed

- Enterprise Quality Governance framework established.
- Quality Policy, Quality Review Standard, and Quality Gate Register added.
- Repository, architecture, standards, and release readiness gates defined.
- ADR-GOV-001 adopted the Enterprise Quality Governance Framework.

## BR-1.0 - Foundation Baseline Established

### Completed

-   Discovery Phase completed
-   Foundation Baseline 1.0 established
-   Repository-first strategy adopted
-   Enterprise Engineering selected as next phase

### Next

-   WS-001 Enterprise Semantic Foundation
-   GLO-001 Enterprise Glossary v0.1

### Notes

-   Continue ADR numbering from existing register.
-   Foundation evolves through governed changes.
