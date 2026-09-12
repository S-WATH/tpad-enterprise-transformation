# TPAD Transformation Checkpoint — 2026-09-12

**Checkpoint ID:** TPAD-CHECKPOINT-2026-09-12  
**Project:** TPAD Enterprise Transformation Program  
**Repository:** `S-WATH/tpad-enterprise-transformation`  
**Source of Truth:** `main`  
**Purpose:** Controlled project-state checkpoint and cross-session handoff reference

---

## 1. Checkpoint Status

This checkpoint records the project state established from the controlled repository, the prior checkpoint `TPAD-CHECKPOINT-2026-09-08`, and the current controlled working session as of 2026-09-12.

This document is a **state/handoff checkpoint**, not a new architecture baseline and not an approval of draft artifacts.

No historical numeric checkpoint sequence is asserted. The project continues to use date-based checkpoint identifiers.

---

## 2. Authority and Architecture State

- Architecture Baseline: **AB-2.0**
- Architecture Freeze: **Active**
- Current Phase: **Phase 3 — Enterprise Knowledge Implementation**
- Repository Source of Truth: **`main`**
- Approved architecture is not to be redesigned through this checkpoint.

### Controlled Semantic Foundation

The following Phase 2 semantic artifacts remain draft unless their individual lifecycle status says otherwise:

- SEM-001
- SEM-002
- CON-001
- GLO-001
- OBJ-001
- REL-001

### Knowledge Foundation

- KB-001: Approved
- KD-001: controlled foundation component
- KD-002: controlled foundation component
- DOM-001: Approved
- OBJ-001 meta-model: controlled foundation

---

## 3. Repository / Workstream State

### Completed / Controlled

- WS-300 — Repository Bootstrap: **CLOSED**
- WS-310 — Controlled Baseline Synchronization: **CLOSED**
- Phase 2 approved-artifact synchronization: completed
- REG-001 lifecycle approval: completed
- REG-PILOT-001 quality review: **PASS — pilot continuation authorized**

### Regulatory Knowledge Work

- REG-PILOT-002: active working stream for TPAD State/Police Aviation regulatory-chain analysis.
- REG-KR-001: draft regulatory knowledge record set.
- Flight Plan requirement extraction and current-state/control analysis have been established as prior controlled working context.
- The regulatory chain remains:

`Parent Legal Instrument → Authority/Delegation → Subordinate Regulatory Instrument → Detailed Provision → Requirement/Obligation → Applicability → TPAD Control → Evidence`

For civil provisions, applicability must be tested rather than assumed:

`Civil Aviation Provision → Scope / Applicability Test → Applicable / Not directly applicable / Unresolved`

A parent Thai legal instrument must not be treated as if it contains every detailed operational requirement where subordinate instruments provide the detail.

---

## 4. Maintenance Transformation State

Maintenance is now the current major controlled transformation workstream.

The required sequence remains:

`AS-IS Maintenance → Regulatory Applicability → Maintenance Operating Model → Maintenance / Continuing Airworthiness Boundary → Roles & Authority → Target-State Architecture → International Benchmark Mapping → Internal Standards → Procedures → Controlled Documents → Records / Evidence / Assurance`

### AS-IS Maintenance Evidence Established

Current maintenance execution has two major modes:

1. **In-house maintenance** through the TPAD / Police Aviation aircraft maintenance group.
2. **Outsourced maintenance** through Thai Airways under an annual contract, with one aircraft group managed by Thai Airways and another jointly planned with TPAD.

Scheduled maintenance generally follows:

`TPAD aircraft list / flight hours / schedule → Thai Airways plan → TPAD review → agreed maintenance timing`

Unscheduled defects may be corrected immediately by an accompanying mechanic, followed by inspection and, where required, test flight and command authorization for operational use.

For outsourced maintenance, TPAD maintenance coordinates directly with Thai Airways after aircraft handover. Out-of-contract / “over and above” matters are currently handled through joint coordination/meetings; a formal contractual approval path has not been evidenced in the current-state material.

### Current Records / Information State

In-house maintenance is predominantly document-centric. The current-state description indicates:

- no systematic Work Order / Work Sheet model in normal practice;
- maintenance history exists but is fragmented and difficult to retrieve;
- records may become scattered when aircraft are stationed at flight units;
- older paper records are difficult to retrieve and may be lost over time;
- technical manuals are mainly manufacturer subscriptions and are regularly updated;
- parts are requisitioned from central stores and parts history is retained by maintenance, but the information is not systematic/easy to search;
- defect reporting exists through official correspondence and aircraft logbook / aircraft record book entries;
- there is no dedicated central defect-tracking system;
- minor defects that remain flyable do not have systematic tracking;
- there is no single real-time source of truth for fleet status.

These observations are **current-state evidence**, not conclusions of regulatory non-compliance.

### Key Maintenance Findings

- F1 — Dual Maintenance Execution Model
- F2 — Outsourced Maintenance Contract-Based Interface
- F3 — In-house Maintenance Records are Document-Centric
- F4 — Historical Records Retrieval Gap
- F5 — Defect Recording Exists; Defect Tracking Lacks Central System
- F6 — Parts History Information Gap
- F7 — Fleet Status Visibility Gap

---

## 5. MNT-001 Draft State

A draft working artifact has been defined as:

### `MNT-001 — Maintenance Operating Model — AS-IS Discovery`

Status: **Draft / not approved**

Purpose: evidence-based current-state discovery, not target-state design.

Scope:

1. Current maintenance activities
2. Internal vs outsourced maintenance
3. Responsibility / authority as currently evidenced
4. Technical data / records
5. Interfaces
6. Evidence gaps

Evidence classification proposed for the draft:

- E0 = no evidence identified
- E1 = reported / interview
- E2 = documentary
- E3 = cross-validated
- E4 = controlled authoritative

Interpretation rules:

- No evidence identified ≠ activity does not exist.
- Evidence gap ≠ proven non-compliance.
- Job title ≠ proof of formal authority.

MNT-001 must not be treated as an approved operating model or target-state organizational design.

---

## 6. Regulatory Applicability — Current Working State

The current regulatory work has moved from general framing to **provision-level applicability analysis**.

The primary legal source currently being examined is the uploaded consolidated:

`พระราชบัญญัติการเดินอากาศ พ.ศ. 2497 และที่แก้ไขเพิ่มเติมจนถึงฉบับที่ 14`

### Evidence-backed legal boundary identified

Section 5 is a critical applicability boundary. It establishes that the Act generally does not apply to air navigation in military, police, customs, and certain other government service, subject to specified exceptions including flight-plan and rules-of-air provisions under sections 18/1–18/3.

Source evidence:

fileciteturn49file0L198-L210

Therefore the current working position is **not** that Police Aviation is completely outside the Air Navigation Act. The correct approach is provision-by-provision applicability analysis.

### Maintenance definition evidence

The Act defines maintenance broadly in relation to continuing airworthiness, including repair, inspection, removal/replacement, modification, and defect correction.

Source evidence:

fileciteturn49file0L11-L20

This is currently treated as scope/concept evidence only. It does not by itself establish that all maintenance provisions apply to Police Aviation.

### Journey Log evidence

The Act contains provisions concerning journey logs and recording responsibilities of the registered owner/operator and pilot.

Source evidence:

fileciteturn48file3L116-L143

Applicability to TPAD State/Police Aviation remains **unresolved pending cross-check against the Section 5 boundary and the applicable subordinate provisions/instruments**.

### Current applicability positions

| Topic | Current position |
|---|---|
| Police/government aviation scope | Applicability boundary evidenced; detailed exceptions require provision-level analysis |
| Maintenance definition | Definition evidenced; does not establish applicability of all maintenance provisions |
| Journey Log | Provision evidenced; TPAD applicability unresolved pending cross-check |
| Maintenance organisation / maintenance unit requirements | Unresolved |
| Technical records requirements | Unresolved |
| Defect / inspection requirements | Unresolved |
| Sections 18/1–18/3 | Requires detailed provision-level analysis |
| Part-145 / CAMO / EASA | Strategic/reference benchmark unless applicability is established |
| ICAO Annexes | Must distinguish international obligation from benchmark/reference |
| TCAR civil requirements | Applicability must be tested provision-by-provision |

---

## 7. Regulatory Interpretation Rules

The following rules are mandatory for continuation of this workstream:

1. Do not assume civil aviation requirements automatically apply to TPAD State/Police Aviation.
2. Do not assume that use of a civil maintenance provider changes the legal status of the aircraft or automatically imports a civil regulatory regime.
3. Do not treat Part-145, CAMO, MOE, CAME, EASA, Part-M or similar concepts as statutory TPAD requirements without authoritative applicability evidence.
4. Distinguish legal obligation, regulatory requirement, international standard, benchmark/reference, and internal requirement.
5. Use provision-level evidence rather than broad regulatory labels.
6. Evidence gap ≠ proven non-compliance.
7. Exclusion from a civil regime ≠ unregulated activity.
8. Parent law ≠ complete operational rule set where subordinate instruments provide the detailed requirement.

---

## 8. Organization and Authority Boundary

Previous brainstorming proposed possible functional structures and post-holder concepts, including Accountable Manager, Quality, Maintenance, CAME/MOE-related functions, and other roles.

These remain **ideas / design inputs only**.

They are not approved organizational design.

Do not:

- add a four-functional/Post Holder structure to DOM-001;
- infer formal authority from current job titles;
- create MOE/CAME-type controlled documents at this stage;
- define maintenance release authority before the applicable regulatory and internal authority basis is established.

Maintain the distinction:

`Activity ≠ Responsibility ≠ Authority ≠ Regulatory Applicability ≠ Organizational Position`

---

## 9. Explicit Non-Changes

This checkpoint does **not** authorize:

- redesign of AB-2.0;
- removal or alteration of the architecture freeze;
- conversion of draft semantic artifacts into approved artifacts;
- treating civil aviation provisions as automatically applicable to Police Aviation;
- treating MOE/CAME/Part-145/CAMO concepts as statutory TPAD requirements without evidence;
- adding unapproved organizational structures to controlled architecture;
- creating SOPs/forms/systems before the relevant design/control has been reviewed and approved;
- treating missing records alone as proof of non-compliance;
- changing approved governance identifiers merely because similar terminology appears in another domain.

---

## 10. Immediate Next Controlled Deliverable

The next reviewable deliverable is:

### **Regulatory Applicability — Provision-Level Evidence Matrix**

Minimum structure:

`Provision → Requirement → Applies to whom → TPAD Police Aviation applicability → Evidence → Confidence → Unresolved issue`

Priority areas:

1. Maintenance / airworthiness provisions
2. Maintenance organisation / maintenance unit provisions
3. Aircraft technical records / journey log
4. Defect / inspection provisions
5. Police / government aviation applicability provisions
6. Sections 18/1–18/3 and their exceptions
7. Relevant subordinate regulatory instruments where the parent Act delegates or prescribes detail

This matrix is an analysis/review deliverable, not a legal opinion and not an authorization to implement controls.

---

## 11. One-Deliverable / Approval Gate

The program continues to follow:

`Understand current state → Evidence → Applicability → Review → Approval → Controlled design → Implementation`

Do not create multiple parallel controlled deliverables merely because related design questions are visible.

Before implementation or repository changes to controlled artifacts:

- review the proposed deliverable;
- obtain the required approval;
- then perform the controlled change.

---

## 12. Handoff Instruction for Next Session

Start from this checkpoint and the repository `main`.

First read:

1. `docs/governance/checkpoints/TPAD-CHECKPOINT-2026-09-12.md`
2. `README.md`
3. relevant governance artifacts referenced by the checkpoint
4. the current regulatory-chain / REG-PILOT-002 artifacts
5. the Air Navigation Act source used for the applicability analysis

Then continue with **Regulatory Applicability — Provision-Level Evidence Matrix**.

Do not restart the program from a blank state.

Do not redesign AB-2.0.

Do not promote draft semantic artifacts.

Do not assume civil aviation requirements apply to TPAD Police Aviation.

Do not begin MOE/CAME/Part-145/CAMO document production.

Produce one reviewable deliverable at a time and stop before controlled implementation unless approval is given.

---

## 13. Checkpoint End State

At this checkpoint, TPAD Transformation is in **Phase 3 under AB-2.0 Architecture Freeze**. Maintenance AS-IS discovery has established a dual in-house/outsourced maintenance model and identified significant information, records, defect-tracking, and fleet-status visibility gaps. The program has now entered provision-level Regulatory Applicability analysis, with Section 5 of the Air Navigation Act established as a key legal boundary and maintenance/journey-log provisions requiring further applicability cross-checking.

The immediate next action is to produce the **Regulatory Applicability — Provision-Level Evidence Matrix** before moving to the Maintenance Operating Model target-state design.
