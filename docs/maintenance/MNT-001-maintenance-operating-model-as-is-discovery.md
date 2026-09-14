---
id: MNT-001
title: Maintenance Operating Model — AS-IS Discovery
type: operational
domain: capability
status: draft
version: 0.1.0
owner: TPAD Enterprise Transformation Team
created: 2026-09-14
updated: 2026-09-14
tags:
  - maintenance
  - as-is
  - discovery
  - evidence
related:
  - ADR-GOV-002
  - DOM-001
  - AB-2.0
  - TPAD-CHECKPOINT-2026-09-12
---

# MNT-001 — Maintenance Operating Model — AS-IS Discovery

## Status

**Draft — not approved.**

This document is the controlled AS-IS discovery artifact authorized by ADR-GOV-002. Approval of ADR-GOV-002 established the `MNT` identifier family; it did **not** approve the content of this artifact.

## Purpose

Capture the current maintenance operating state as an evidence-based discovery baseline for subsequent regulatory-applicability analysis and controlled maintenance target-state design.

This document does not define or approve a target-state operating model, organizational structure, post-holder arrangement, maintenance-release authority, MOE/CAME arrangement, or implementation solution.

## Scope

1. Current maintenance activities
2. Internal versus outsourced maintenance
3. Responsibility and authority as currently evidenced
4. Technical data and records
5. Interfaces
6. Evidence gaps

## Evidence Classification

| Code | Classification | Interpretation |
|---|---|---|
| E0 | No evidence identified | No supporting evidence has been identified in the current discovery set. This does not mean the activity does not exist. |
| E1 | Reported / interview | Information reported through interviews or working discussions; not independently validated. |
| E2 | Documentary | Supported by documentary evidence identified during discovery. |
| E3 | Cross-validated | Supported by more than one compatible evidence source or independently cross-checked. |
| E4 | Controlled authoritative | Supported by an authoritative controlled source or formally approved record. |

## Interpretation Rules

- No evidence identified ≠ activity does not exist.
- Evidence gap ≠ proven non-compliance.
- Job title ≠ proof of formal authority.
- Current-state observation ≠ target-state decision.
- Reference to a regulatory framework ≠ proof of applicability.

## Current-State Discovery

### 1. Maintenance Execution Model

The current-state material identifies two major maintenance execution modes:

1. **In-house maintenance** through the TPAD / Police Aviation aircraft maintenance group.
2. **Outsourced maintenance** through Thai Airways under an annual contract, with aircraft groups managed through defined TPAD/Thai Airways coordination arrangements.

**Evidence status:** E1 — reported current-state description pending documentary/cross-validation.

### 2. Scheduled Maintenance Interface

The current-state description indicates the following working sequence:

```text
TPAD aircraft list / flight hours / schedule
        ↓
Thai Airways plan
        ↓
TPAD review
        ↓
Agreed maintenance timing
```

**Evidence status:** E1 — reported current-state description pending documentary/cross-validation.

### 3. Unscheduled Defects / Return to Operational Use

The current-state description indicates that unscheduled defects are corrected immediately where possible, followed by inspection and, where required, test flight and command authorization for return to operational use.

This statement is recorded as current-state discovery only. The formal authority basis and applicable regulatory requirements remain subject to separate applicability analysis.

**Evidence status:** E1 — reported current-state description pending documentary/cross-validation.

## Information and Records State

### F3 — In-house Maintenance Records are Document-Centric

The current-state material indicates that in-house maintenance remains predominantly document-centric, including the absence of a systematic Work Order / Work Sheet model in normal practice.

**Evidence status:** E1.

### F4 — Historical Records Retrieval Gap

Fragmented maintenance history and difficult retrieval were identified. Records may become scattered when aircraft are stationed at flight units; older paper records are difficult to retrieve and may be lost over time.

**Evidence status:** E1.

### Technical Data

Technical manuals are mainly maintained through manufacturer subscriptions.

**Evidence status:** E1.

### F6 — Parts History Information Gap

Parts requisition and parts history exist but are not yet systematic/easy to search.

**Evidence status:** E1.

### F5 — Defect Recording Exists; Defect Tracking Lacks Central System

Defect reporting exists through official correspondence and aircraft logbook / aircraft record book entries. The current-state material indicates no dedicated central defect-tracking system and no systematic tracking for minor flyable defects.

**Evidence status:** E1.

### F7 — Fleet Status Visibility Gap

The current-state material indicates no single real-time source of truth for fleet status.

**Evidence status:** E1.

## Current-State Findings Register

| ID | Finding | Current interpretation | Evidence status |
|---|---|---|---|
| F1 | Dual Maintenance Execution Model | In-house and outsourced maintenance modes are both described. | E1 |
| F2 | Outsourced Maintenance Contract-Based Interface | Thai Airways is described as the outsourced maintenance interface under an annual contract. | E1 |
| F3 | In-house Maintenance Records are Document-Centric | Records are predominantly document-centric; systematic WO/WS model not identified in normal practice. | E1 |
| F4 | Historical Records Retrieval Gap | Historical records are difficult to retrieve; paper records present a retention/retrieval concern. | E1 |
| F5 | Defect Recording Exists; Defect Tracking Lacks Central System | Defect recording exists, but a central tracking system was not identified. | E1 |
| F6 | Parts History Information Gap | Parts history exists but is not systematic/easy to search. | E1 |
| F7 | Fleet Status Visibility Gap | No single real-time fleet-status source of truth was identified. | E1 |

## Responsibility and Authority Boundary

This AS-IS artifact records reported activities and interfaces but does not infer formal organizational authority from job titles or current working arrangements.

The following remain unresolved for subsequent controlled analysis:

- formal maintenance responsibility;
- formal maintenance-release authority;
- regulatory applicability affecting maintenance authority;
- relationship between maintenance execution and continuing-airworthiness functions;
- any formal post-holder structure;
- applicability of MOE/CAME/Part-145/CAMO concepts.

These matters require evidence and/or provision-level regulatory applicability analysis before target-state design.

## Evidence Gap Register

| ID | Gap | Current status |
|---|---|---|
| EG-001 | Documentary evidence for the two maintenance execution modes | Open |
| EG-002 | Controlled evidence for outsourced maintenance contractual interface | Open |
| EG-003 | Documentary evidence for current maintenance record practices | Open |
| EG-004 | Historical-record retention and retrieval evidence | Open |
| EG-005 | Central defect-tracking capability evidence | Open |
| EG-006 | Parts-history information-system evidence | Open |
| EG-007 | Fleet-status visibility / source-of-truth evidence | Open |
| EG-008 | Formal authority basis for maintenance release / return-to-service decisions | Open |

## Relationship to Regulatory Applicability Analysis

MNT-001 is not a legal opinion and does not determine whether any external civil, state, police, or international aviation requirement applies to TPAD.

The next controlled analysis must test relevant provisions individually using the program's regulatory chain:

```text
Authority
→ Source Document
→ Provision / Citation
→ Requirement / Obligation
→ Applicability Assessment
→ TPAD Control / Standard
→ Procedure
→ Evidence
```

In particular, current-state observations must not be converted directly into assumptions about Part-145, CAMO, MOE, CAME, Part-M, or other external frameworks.

## Target-State Boundary

Target-state design is explicitly out of scope for this document.

No target-state organizational chart, post-holder structure, maintenance-release scheme, MOE/CAME model, software solution, SOP, form, or implementation decision is approved by MNT-001.

## Lifecycle

```text
Draft → Review → Approved → Released → Archived
```

MNT-001 is currently **Draft**. It must complete evidence review and the applicable approval process before it can be treated as an approved controlled baseline.

## Next Controlled Actions

1. Review and validate the E1 current-state statements against available documentary evidence.
2. Perform the Regulatory Applicability — Provision-Level Evidence Matrix for the maintenance-related provisions.
3. Update MNT-001 evidence classifications as evidence is validated.
4. Submit MNT-001 for Review when the AS-IS evidence set is sufficiently complete.
5. Do not begin maintenance target-state design until the relevant AS-IS and applicability work has completed its controlled review/approval gates.

## Approval Record

No approval has been granted for MNT-001.

ADR-GOV-002 approval authorizes use of the `MNT` identifier family only and does not constitute approval of this document.
