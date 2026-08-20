---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Air Navigation Act
type: information
status: draft
version: 0.1.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-08-20
updated: 2026-08-20
related:
  - REG-001
  - REG-PILOT-001
  - QR-REG-PILOT-001
  - KB-001
  - DOM-001
  - AB-2.0
---

# REG-KR-001 — Pilot Regulatory Knowledge Records

## 1. Purpose

Create reusable provision-level regulatory knowledge records from the five approved pilot records in REG-PILOT-001, while preserving source provenance and keeping TPAD applicability explicitly unassessed.

This deliverable is a controlled implementation test. It does not create legal conclusions, TPAD controls, procedures, or ICAO/EASA equivalence.

## 2. Source Basis

Primary source:

`พระราชบัญญัติการเดินอากาศ พ.ศ. 2497 และที่แก้ไขเพิ่มเติมจนถึงฉบับที่ 14 (Consolidated Text)`

The source file is the project-provided consolidated text. Exact provision verification remains a required evidence step before downstream reuse.

## 3. Record Model

Each record uses the following conceptual structure:

```text
Identifier
  ↓
Source / Authority
  ↓
Provision / Citation
  ↓
Source-derived Assertion
  ↓
Knowledge Role
  ↓
Applicability Status
  ↓
Evidence / Verification Status
```

## 4. Pilot Records

### REG-KR-001-001 — Director Requirements

| Field | Value |
|---|---|
| Identifier | REG-KR-001-001 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Regulation / Requirement context |
| Provision target | Corresponding provision identified in REG-PILOT-001 RP-001-001 |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING PROVISION-LEVEL VERIFICATION` |

**Source-derived assertion:** The Act contains provisions under which requirements may be prescribed by the Director.

**Control boundary:** The existence of a Director-prescribed requirement does not by itself establish the content, applicability, or TPAD obligation of that requirement.

### REG-KR-001-002 — Documents Required for Flight

| Field | Value |
|---|---|
| Identifier | REG-KR-001-002 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation |
| Provision target | Corresponding provision identified in REG-PILOT-001 RP-001-002 |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING PROVISION-LEVEL VERIFICATION` |

**Source-derived assertion:** The Act identifies documents that must be carried or available with an aircraft for flight, subject to the conditions and exceptions stated in the Act.

**Evidence note:** Exact section/article citation must be recorded before downstream reuse.

### REG-KR-001-003 — Airworthiness / No-Fly Conditions

| Field | Value |
|---|---|
| Identifier | REG-KR-001-003 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement context |
| Provision target | Corresponding provision identified in REG-PILOT-001 RP-001-003 |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING PROVISION-LEVEL VERIFICATION` |

**Source-derived assertion:** The Act contains provisions concerning airworthiness and circumstances in which an aircraft may be prohibited from flight, including conditions relating to maintenance or certification.

**Control boundary:** This record does not determine how the provisions apply to TPAD state-aircraft operations.

### REG-KR-001-004 — Maintenance Organisation Controls

| Field | Value |
|---|---|
| Identifier | REG-KR-001-004 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement |
| Provision target | Corresponding provision identified in REG-PILOT-001 RP-001-004 |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING PROVISION-LEVEL VERIFICATION` |

**Source-derived assertion:** The Act contains requirements concerning certification and operation of aircraft maintenance organisations.

The project source identifies a provision stating that operation of a maintenance organisation in Thailand requires a maintenance-organisation certificate and distinguishes certificate types for aircraft, major components, and aircraft equipment/parts.

**Control boundary:** This record does not conclude that the statutory certification regime applies directly to TPAD or its internal maintenance organisation.

### REG-KR-001-005 — Aviation Security Plans

| Field | Value |
|---|---|
|---|---|
| Identifier | REG-KR-001-005 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement context |
| Provision target | Corresponding provision identified in REG-PILOT-001 RP-001-005 |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING PROVISION-LEVEL VERIFICATION` |

**Source-derived assertion:** The Act contains provisions relating to aviation security measures and security requirements.

The project source also contains airport-area security requirements, including requirements concerning access to aircraft parking areas.

**Control boundary:** This record does not establish a TPAD security-plan obligation without applicability evidence.

## 5. Evidence Status

The five records are reusable **pilot records**, but they are not yet evidence-complete regulatory knowledge objects for downstream decision-making.

```text
Pilot Record
    ↓
Provision-level verification
    ↓
Evidence-complete record
    ↓
Applicability assessment
    ↓
Potential TPAD control
```

## 6. ICAO / EASA Comparison Boundary

No ICAO or EASA comparative assertion is populated in this first record set.

This is intentional. REG-001 requires an explicit authoritative source provision before comparative analysis is recorded.

The next comparison cycle may select matching ICAO and EASA provisions for individual records, but comparison must remain separate from Thai legal applicability.

## 7. Lifecycle Boundary

`REG-KR-001` remains `draft` until its records have undergone the applicable quality and evidence verification cycle.

Approval of the record set will not itself determine legal applicability to TPAD.

## 8. Next Controlled Action

Verify the exact provision citation and source evidence for the five records, then update the records from `PENDING PROVISION-LEVEL VERIFICATION` to an evidence-supported state before introducing applicability analysis or ICAO/EASA comparison.
