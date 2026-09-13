# CHANGELOG

## Governance Approval & Metadata Remediation — 2026-09-13

### Completed

- Program Sponsor approval recorded for `ADR-GOV-001` — Adopt Enterprise Quality Governance Framework.
- Program Sponsor approval recorded for `ADR-GOV-002` — Introduce the MNT Identifier Family for Maintenance Transformation Artifacts.
- Corrected both ADR frontmatter records to use the Metadata Standard's `approver` field; non-standard `approved_by` and `approved_date` fields were removed.
- Recorded an explicit governance evidence gap: the repository currently establishes `Program Sponsor` as the approval role but does not establish the underlying person or formal appointment instrument for that role. No identity was inferred or substituted.
- `MNT-001` remains uncreated. Approval of `ADR-GOV-002` authorizes the `MNT` identifier family only; `MNT-001` requires its own Draft → Review → Approved lifecycle.

### Control Notes

- Approval decisions were retained; the remediation did not invent a historical `Review` status in the repository.
- This remediation did not redesign AB-2.0, did not alter the Architecture Freeze, and did not promote `MNT-001` or any other operational artifact.

## Governance Hygiene Remediation — 2026-09-13

### Completed

- Removed AI-tool citation markers (hidden private-use Unicode control characters wrapping `cite`/`filecite` tokens) that had been committed verbatim into `REG-KR-001` and `TPAD-CHECKPOINT-2026-09-12`. Each removed marker was replaced with an explicit flag for source re-verification; no citation content was invented to replace them.
- Added mandatory YAML frontmatter (`id`, `title`, `type`, `status`, `version`, `domain`, `owner`, `created`, `updated`) to both checkpoint files, consistent with the Metadata Standard and with the Checkpoint = Baseline document-type classification.
- Set `TPAD-CHECKPOINT-2026-09-08` status to `Archived` (superseded by `TPAD-CHECKPOINT-2026-09-12`), per the Document Lifecycle Standard rule that superseded documents are archived, not deleted.

### Control Notes

- This remediation did not redesign AB-2.0, did not alter the Architecture Freeze, and did not promote the lifecycle status of any other artifact.
- `MNT-001` was **not** created as part of this remediation. It remained a narrative reference pending resolution of the `MNT` identifier-family governance gap; that gap is now resolved by approved `ADR-GOV-002`.

## Phase 3 — Enterprise Knowledge Implementation

### Completed / Controlled

- `KB-001` — Enterprise Knowledge Foundation Baseline — Approved.
- `DOM-001` — Enterprise Knowledge Domain Architecture — Approved.
- `REG-001` — Regulatory & Standards Knowledge Domain Baseline — Approved v0.2.0.
- `REG-PILOT-001` — quality review PASS / pilot continuation authorized.
- Checkpoints `TPAD-CHECKPOINT-2026-09-08` and `TPAD-CHECKPOINT-2026-09-12` recorded as controlled state/handoff references.
- `ADR-GOV-001` — Approved.
- `ADR-GOV-002` — Approved; `MNT` identifier family is now governed.

### Active

- `REG-PILOT-002` — TPAD State/Police Aviation regulatory-chain analysis (Section 5 boundary, Section 16/1 Journey Log applicability).
- `REG-KR-001` — draft regulatory knowledge record set.
- Maintenance transformation workstream — AS-IS discovery in narrative form (findings F1–F7); `MNT-001` not yet captured as a controlled artifact.

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
