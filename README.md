# TPAD Enterprise Transformation Program

> Enterprise Architecture, Regulatory Framework, Enterprise Knowledge Management, and Digital Transformation for the Police Aviation Division (TPAD).

---

## 1. Program Purpose

The **TPAD Enterprise Transformation Program** is the controlled enterprise-transformation program for the Police Aviation Division.

This repository is the program's **Enterprise Knowledge Repository** and **Repository Source of Truth** for architecture, governance, semantic models, regulatory analysis, knowledge management, transformation evidence, and controlled deliverables.

Core principles:

> **Repository-first · Standard-first · Semantic-first · Evidence-first · AI-ready by Design**

The program combines Enterprise Architecture, Systems Engineering, Regulatory Architecture, Enterprise Knowledge Management, Docs as Code, Knowledge as Code, Quality Management, and evidence-based traceability.

---

## 2. Current Authority State

| Item | Current State |
|---|---|
| Architecture Baseline | **AB-2.0** |
| Architecture Freeze | **ACTIVE** |
| Current Phase | **Phase 3 — Enterprise Knowledge Implementation** |
| Repository Source of Truth | **`main`** |
| Current Checkpoint | **`TPAD-CHECKPOINT-2026-09-12`** |
| Phase 2 | **Completed** |
| WS-300 — Repository Bootstrap | **CLOSED** |
| WS-310 — Controlled Baseline Synchronization | **CLOSED** |

AB-2.0 remains the controlling architecture baseline. The architecture freeze remains active. A checkpoint records project state and handoff; it does **not** create a new architecture baseline or authorize architecture redesign.

The current checkpoint also establishes that the project uses **date-based checkpoint identifiers**; no historical numeric checkpoint sequence is asserted.

---

## 3. Current Phase 3 Position

Phase 3 has progressed from knowledge-foundation establishment into controlled regulatory-applicability analysis and maintenance transformation discovery.

### Completed / Controlled

- `KB-001` — Enterprise Knowledge Foundation Baseline — **APPROVED**
- `DOM-001` — Enterprise Knowledge Domain Architecture — **APPROVED**
- `REG-001` — Regulatory & Standards Knowledge Domain Baseline — **APPROVED v0.2.0**
- `REG-PILOT-001` — quality review **PASS; pilot continuation authorized**
- Phase 2 approved-artifact synchronization — **completed**
- `WS-300` — Repository Bootstrap — **CLOSED**
- `WS-310` — Controlled Baseline Synchronization — **CLOSED**

### Current Working Streams

- `REG-PILOT-002` — active regulatory-chain analysis for TPAD State/Police Aviation
- `REG-KR-001` — draft regulatory knowledge record set
- Maintenance transformation — current major controlled transformation workstream
- `MNT-001` — draft AS-IS maintenance discovery artifact

The authoritative handoff for these statuses is `docs/governance/checkpoints/TPAD-CHECKPOINT-2026-09-12.md`.

---

## 4. Phase 2 Semantic Foundation

The following six semantic artifacts remain under controlled repository governance and remain **draft** unless their individual lifecycle evidence states otherwise:

| Artifact | Purpose | Current Lifecycle |
|---|---|---|
| `SEM-001` | Enterprise Semantic Principles | `draft` |
| `SEM-002` | Enterprise Identifier Standard | `draft` |
| `CON-001` | Enterprise Concept Catalog | `draft` |
| `GLO-001` | Enterprise Glossary | `draft` |
| `OBJ-001` | Enterprise Object Model | `draft` |
| `REL-001` | Enterprise Relationship Model | `draft` |

Maintain the distinction:

```text
Project Authority Approval
        ≠
Repository Synchronization
        ≠
Document Lifecycle Promotion
```

An artifact being present in Git does not by itself mean that it is approved or released.

---

## 5. Enterprise Knowledge Domain Architecture

`DOM-001` establishes the current semantic/business domains:

1. Governance & Strategy
2. Regulatory & Standards
3. Aviation Operations
4. Safety & Security
5. Airworthiness & Maintenance
6. Training & Competency
7. Resources & Support
8. Quality & Assurance

> **Knowledge Domain ≠ Organization**

These domains are semantic/business boundaries. They must not be used to infer reporting lines, post-holder structures, formal authority, or organizational design unless separately evidenced and approved.

---

## 6. Regulatory & Standards Architecture

The program distinguishes among:

```text
Legal Obligation
        ≠
Regulatory Requirement
        ≠
International Standard
        ≠
Comparative Regulatory Baseline
        ≠
Adopted Standard
        ≠
Internal TPAD Requirement
        ≠
Reference / Benchmark
```

The standing comparative model is:

```text
Thai Authority
      +
ICAO
      +
EASA
      +
Other Relevant Standards
      ↓
Comparative Analysis
      ↓
TPAD Strategic Decision
```

EASA is a **strategic comparative regulatory baseline** unless an authoritative applicability basis establishes otherwise. It is not automatically a Thai legal obligation, CAAT requirement, or TPAD mandatory requirement.

The same principle applies to ICAO Annexes, civil aviation requirements, Part-145, CAMO, MOE, CAME, Part-M, and similar external frameworks: reference or comparative use does not by itself create a TPAD legal or organizational obligation.

---

## 7. Regulatory Knowledge Traceability

Regulatory knowledge should be traceable through:

```text
Authority
   ↓
Source Document
   ↓
Provision / Citation
   ↓
Requirement / Obligation
   ↓
Applicability Assessment
   ↓
TPAD Control / Standard
   ↓
Procedure
   ↓
Evidence
```

The current regulatory work has moved to **provision-level applicability analysis** rather than broad regulatory labeling.

Mandatory interpretation rules:

1. Do not assume civil aviation requirements automatically apply to TPAD State/Police Aviation.
2. Use of a civil maintenance provider does not by itself change the legal status of the aircraft or import a civil regulatory regime.
3. Do not treat Part-145, CAMO, MOE, CAME, EASA, Part-M, or similar concepts as statutory TPAD requirements without authoritative applicability evidence.
4. Use provision-level evidence rather than broad regulatory labels.
5. Evidence gap ≠ proven non-compliance.
6. Exclusion from a civil regime ≠ unregulated activity.
7. A parent legal instrument is not necessarily the complete operational rule set where subordinate instruments provide the detail.

---

## 8. Current Regulatory Applicability Work

The immediate controlled deliverable is:

### **Regulatory Applicability — Provision-Level Evidence Matrix**

Minimum structure:

```text
Provision
→ Requirement
→ Applies to whom
→ TPAD Police Aviation applicability
→ Evidence
→ Confidence
→ Unresolved issue
```

Priority areas:

1. Maintenance / airworthiness provisions
2. Maintenance organisation / maintenance unit provisions
3. Aircraft technical records / journey log
4. Defect / inspection provisions
5. Police / government aviation applicability provisions
6. Sections 18/1–18/3 and their exceptions
7. Relevant subordinate regulatory instruments where the parent Act delegates or prescribes detail

The current checkpoint identifies **Section 5 of the Air Navigation Act** as a critical applicability boundary. The working position is therefore not that Police Aviation is completely outside the Act; applicability must be established provision by provision.

This matrix is an analysis/review deliverable. It is not a legal opinion and does not authorize implementation.

---

## 9. Maintenance Transformation — Current State

Maintenance is currently the major transformation workstream.

Required sequence:

```text
AS-IS Maintenance
      ↓
Regulatory Applicability
      ↓
Maintenance Operating Model
      ↓
Maintenance / Continuing Airworthiness Boundary
      ↓
Roles & Authority
      ↓
Target-State Architecture
      ↓
International Benchmark Mapping
      ↓
Internal Standards
      ↓
Procedures
      ↓
Controlled Documents
      ↓
Records / Evidence / Assurance
```

### 9.1 Current Maintenance Execution

Current-state evidence establishes two major modes:

1. **In-house maintenance** through the TPAD / Police Aviation aircraft maintenance group.
2. **Outsourced maintenance** through Thai Airways under an annual contract, with aircraft groups managed through defined TPAD/Thai Airways coordination arrangements.

Scheduled maintenance generally follows:

```text
TPAD aircraft list / flight hours / schedule
        ↓
Thai Airways plan
        ↓
TPAD review
        ↓
Agreed maintenance timing
```

For unscheduled defects, the current-state description indicates immediate correction where possible, followed by inspection and, where required, test flight and command authorization for return to operational use.

### 9.2 Current Information / Records State

The current-state material indicates that in-house maintenance remains predominantly document-centric:

- no systematic Work Order / Work Sheet model in normal practice;
- fragmented maintenance history and difficult retrieval;
- records may become scattered when aircraft are stationed at flight units;
- older paper records are difficult to retrieve and may be lost over time;
- technical manuals are mainly maintained through manufacturer subscriptions;
- parts requisition and parts history exist but are not yet systematic/easy to search;
- defect reporting exists through official correspondence and aircraft logbook / aircraft record book entries;
- no dedicated central defect-tracking system;
- no systematic tracking for minor flyable defects;
- no single real-time source of truth for fleet status.

These are **current-state observations**, not conclusions of regulatory non-compliance.

### 9.3 Current Maintenance Findings

- **F1** — Dual Maintenance Execution Model
- **F2** — Outsourced Maintenance Contract-Based Interface
- **F3** — In-house Maintenance Records are Document-Centric
- **F4** — Historical Records Retrieval Gap
- **F5** — Defect Recording Exists; Defect Tracking Lacks Central System
- **F6** — Parts History Information Gap
- **F7** — Fleet Status Visibility Gap

---

## 10. MNT-001 — Current Draft State

`MNT-001 — Maintenance Operating Model — AS-IS Discovery`

**Status:** Draft / not approved

Purpose: evidence-based current-state discovery. It is **not** a target-state operating model and must not be treated as approved organizational design.

Scope:

1. Current maintenance activities
2. Internal vs outsourced maintenance
3. Responsibility / authority as currently evidenced
4. Technical data / records
5. Interfaces
6. Evidence gaps

Proposed evidence classification:

- `E0` = no evidence identified
- `E1` = reported / interview
- `E2` = documentary
- `E3` = cross-validated
- `E4` = controlled authoritative

Interpretation rules:

- No evidence identified ≠ activity does not exist.
- Evidence gap ≠ proven non-compliance.
- Job title ≠ proof of formal authority.

---

## 11. Organization and Authority Boundary

Possible functional structures, post-holder concepts, Accountable Manager / Quality / Maintenance arrangements, and MOE/CAME-related concepts remain **ideas / design inputs only** unless formally evidenced, reviewed, and approved.

Do not:

- add an unapproved four-functional / post-holder structure to `DOM-001`;
- infer formal authority from current job titles;
- create MOE/CAME-type controlled documents at this stage;
- define maintenance release authority before the applicable regulatory and internal authority basis is established.

Maintain:

```text
Activity
  ≠
Responsibility
  ≠
Authority
  ≠
Regulatory Applicability
  ≠
Organizational Position
```

---

## 12. Transformation and Governance Sequence

The program uses a controlled sequence:

```text
Authority / Strategy
        ↓
Semantic Foundation
        ↓
Knowledge Domain
        ↓
Knowledge Baseline
        ↓
Controlled Evidence
        ↓
Traceability
        ↓
Quality Review
        ↓
Lifecycle Approval
        ↓
Controlled Design
        ↓
Implementation
```

Operationally:

```text
Understand current state
        ↓
Evidence
        ↓
Applicability
        ↓
Review
        ↓
Approval
        ↓
Controlled design
        ↓
Implementation
```

The program follows a **one-deliverable / approval-gate** model. Related design questions may be visible, but controlled work proceeds through reviewable deliverables rather than uncontrolled parallel implementation.

---

## 13. Repository Structure

The repository is managed as a controlled knowledge system. The current tree includes:

```text
/
├── README.md
├── bootstrap/
│   ├── PROJECT-MANIFEST.yaml
│   ├── CURRENT-STATE.md
│   ├── ROADMAP.md
│   ├── CHANGELOG.md
│   └── ...
├── docs/
│   ├── adr/
│   ├── architecture/
│   └── governance/
│       ├── checkpoints/
│       ├── quality/
│       └── ...
└── ...
```

Key governance areas cover architecture, governance, document lifecycle, metadata, quality reviews, checkpoints, baseline evidence, and controlled repository configuration.

The detailed governance artifacts under `docs/governance/` remain authoritative for lifecycle, metadata, quality-gate, and architecture-control rules.

---

## 14. Quality, Approval, and Lifecycle

Operating rule:

```text
Review
  ↓
Approval
  ↓
Controlled Change
  ↓
Quality Validation
  ↓
Lifecycle Promotion / Release
```

`Approved` and `Released` are distinct lifecycle states.

Repository synchronization is not lifecycle approval.

A draft artifact must not be treated as an approved standard merely because it is version-controlled, referenced by another document, or present in `main`.

---

## 15. AI Collaboration Model

AI tools are used according to defined roles and project governance. They are not competing sources of project authority.

| AI Platform | Primary Role |
|---|---|
| ChatGPT | Enterprise Architecture Program Office; architecture, governance, evidence, and transformation review |
| NotebookLM | Research and source-oriented analysis |
| Claude | Technical and documentation assistance |
| Codex | Repository engineering when available |

AI output is subordinate to controlled project evidence, approved architecture, governance rules, and authoritative source documents.

---

## 16. Standards & Regulatory Reference Framework

Transformation work should maintain appropriate linkage among:

- ICAO standards and recommended practices
- EASA regulatory framework as a strategic comparative baseline
- Thai aviation law and regulations
- CAAT regulatory instruments
- Police laws and regulations
- Administrative law
- Government procurement requirements
- ISO 9001 and applicable quality-management standards
- Other recognized standards where relevant

Each source retains its own authority, provenance, and applicability. Comparative use does not automatically create a TPAD obligation.

---

## 17. Checkpoints and Cross-Session Continuity

The program uses **date-based checkpoints** as controlled state/handoff references.

Current checkpoint:

`docs/governance/checkpoints/TPAD-CHECKPOINT-2026-09-12.md`

The current checkpoint records that:

- AB-2.0 remains active;
- the architecture freeze remains active;
- Phase 3 is current;
- maintenance AS-IS discovery has been established;
- regulatory work has moved to provision-level applicability analysis;
- the immediate next controlled deliverable is the Regulatory Applicability — Provision-Level Evidence Matrix.

For cross-session work:

1. Read the current checkpoint.
2. Read this `README.md`.
3. Read the relevant governance artifacts referenced by the checkpoint.
4. Continue from the current controlled workstream.
5. Do not reconstruct or redesign the program from a blank state.

---

## 18. Explicit Non-Changes

The current controlled state does **not** authorize:

- redesign of AB-2.0;
- removal or alteration of the architecture freeze;
- promotion of draft semantic artifacts without lifecycle evidence;
- assuming civil aviation requirements automatically apply to Police Aviation;
- treating MOE/CAME/Part-145/CAMO concepts as statutory TPAD requirements without evidence;
- adding unapproved organizational structures to the controlled architecture;
- creating SOPs, forms, systems, or other implementation artifacts before the relevant design/control is reviewed and approved;
- treating missing records alone as proof of non-compliance;
- changing approved governance identifiers merely because similar terminology appears in another domain.

---

## 19. Current Status at a Glance

```text
ARCHITECTURE
  AB-2.0                     ACTIVE BASELINE
  Architecture Freeze        ACTIVE

PHASE
  Phase 3                    ENTERPRISE KNOWLEDGE IMPLEMENTATION

WORKSTREAMS
  WS-300                     CLOSED
  WS-310                     CLOSED
  REG-PILOT-001              PASS / CONTINUATION AUTHORIZED
  REG-PILOT-002              ACTIVE
  MNT-001                    DRAFT / AS-IS DISCOVERY

APPROVED KNOWLEDGE FOUNDATION
  KB-001                     APPROVED
  DOM-001                    APPROVED
  REG-001                    APPROVED v0.2.0

SEMANTIC FOUNDATION
  SEM-001 / SEM-002          DRAFT
  CON-001 / GLO-001          DRAFT
  OBJ-001 / REL-001          DRAFT

CURRENT CHECKPOINT
  TPAD-CHECKPOINT-2026-09-12

NEXT CONTROLLED DELIVERABLE
  Regulatory Applicability — Provision-Level Evidence Matrix
```

---

## 20. Getting Started

For project participants and collaborating AI/system agents:

1. Read `README.md` to establish the current project position.
2. Read `docs/governance/checkpoints/TPAD-CHECKPOINT-2026-09-12.md` for the latest controlled handoff state.
3. Review the applicable governance, architecture, quality, and evidence artifacts.
4. Confirm the relevant approved baseline before proposing change.
5. Work on one reviewable deliverable at a time.
6. Obtain approval before controlled implementation or lifecycle promotion.

**Do not restart the program from a blank state.**

---

## Maintainers

**TPAD Enterprise Transformation Team**

---

> **"Build the Organization before Building the Documents."**
