---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Air Navigation Act
type: information
status: draft
version: 0.2.0
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

Create reusable provision-level regulatory knowledge records from the five pilot records in REG-PILOT-001 while preserving source provenance and keeping TPAD applicability explicitly unassessed.

This deliverable is a controlled implementation test. It does not create legal conclusions, TPAD controls, procedures, or ICAO/EASA equivalence.

## 2. Source Basis

Primary source:

`พระราชบัญญัติการเดินอากาศ พ.ศ. 2497 และที่แก้ไขเพิ่มเติมจนถึงฉบับที่ 14 (Consolidated Text)`

The project-provided consolidated text is the source of record. Provision verification is recorded only where the current source search provides sufficient section-level evidence.

## 3. Record Model

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
| Provision target | Director-prescribed requirements; exact provision retained as pilot target |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PARTIALLY VERIFIED — EXACT SUBORDINATE REQUIREMENT NOT IDENTIFIED` |

**Source-derived assertion:** The Act contains provisions under which requirements may be prescribed by the Director. The current source evidence also shows provisions where the Director sets criteria, qualifications, procedures, or conditions by prescribed requirements.

**Control boundary:** The existence of a Director-prescribed requirement does not by itself establish its content, applicability, or TPAD obligation.

### REG-KR-001-002 — Documents Required for Flight

| Field | Value |
|---|---|
| Identifier | REG-KR-001-002 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation |
| Provision target | Pilot record target retained; exact provision citation not established in this verification pass |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING — EXACT PROVISION TEXT/CITATION RETRIEVAL` |

**Source-derived assertion:** The pilot corpus identifies a statutory requirement concerning documents to be carried or available with an aircraft for flight, subject to the conditions and exceptions in the Act.

**Evidence boundary:** The current source-search evidence retrieved for this verification cycle does not expose the complete text needed to establish the exact provision citation. Therefore the record is not promoted to evidence-complete status and no citation is inferred.

### REG-KR-001-003 — Airworthiness / No-Fly Conditions

| Field | Value |
|---|---|
|---|---|
| Identifier | REG-KR-001-003 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement context |
| Provision target | `มาตรา ๔๑/๘๘` and `มาตรา ๔๑/๘๙` |
| TPAD applicability | `UNASSESSED` |
| Verification status | `VERIFIED — SECTION-LEVEL` |

**Source-derived assertion:** Section 41/88 states that where the aircraft controller considers the aircraft not capable of safe flight, the aircraft maintenance engineer must be notified to restore the aircraft to a safe-flight condition before flight. Section 41/89 prohibits flight in specified conditions, including absence or loss/suspension of an airworthiness certificate and other listed conditions.

The project source explicitly identifies these provisions. fileciteturn74file11

**Control boundary:** This record does not determine how these provisions apply to TPAD state-aircraft operations.

### REG-KR-001-004 — Maintenance Organisation Controls

| Field | Value |
|---|---|
| Identifier | REG-KR-001-004 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement |
| Provision target | `มาตรา ๔๑/๙๓` and `มาตรา ๔๑/๙๔` |
| TPAD applicability | `UNASSESSED` |
| Verification status | `VERIFIED — SECTION-LEVEL` |

**Source-derived assertion:** Section 41/93 states that operating a maintenance organisation in Thailand requires a maintenance-organisation certificate and distinguishes three certificate types: aircraft maintenance, major aircraft components, and aircraft equipment/parts. Section 41/94 prohibits operation of a maintenance organisation without the required certificate from the Director.

The project source explicitly identifies sections 41/93 and 41/94 and the three certificate types. fileciteturn78file5

**Control boundary:** This record does not conclude that the statutory certification regime applies directly to TPAD or its internal maintenance organisation.

### REG-KR-001-005 — Aviation Security Plans

| Field | Value |
|---|---|
| Identifier | REG-KR-001-005 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement context |
| Provision target | `มาตรา ๕๐/๑๖`, `มาตรา ๕๐/๒๗`, and related security-plan provisions |
| TPAD applicability | `UNASSESSED` |
| Verification status | `VERIFIED — SECTION-LEVEL FOR SECURITY-PLAN FRAMEWORK` |

**Source-derived assertion:** Section 50/16 establishes the National Civil Aviation Security Plan and requires CAAT to prepare it as a framework for aviation security and prevention of unlawful interference. Section 50/27 identifies the national security plan, national security training plan, national security quality-control plan, and airport security plan as part of the security framework.

The source also contains provisions concerning security plans for specific aviation actors, including air operators and air traffic service providers. fileciteturn72file18 fileciteturn73file2

**Control boundary:** This record does not establish a TPAD security-plan obligation without a separate applicability assessment.

## 5. Evidence Status Summary

| Record | Verification state |
|---|---|
| REG-KR-001-001 | Partially verified — subordinate requirement not identified |
| REG-KR-001-002 | Pending exact provision retrieval |
| REG-KR-001-003 | Verified — sections 41/88 and 41/89 |
| REG-KR-001-004 | Verified — sections 41/93 and 41/94 |
| REG-KR-001-005 | Verified — security-plan framework sections |

The record set is therefore **not yet evidence-complete as a whole**.

```text
Pilot Record
    ↓
Provision verification
    ↓
Evidence-complete record
    ↓
Applicability assessment
    ↓
Potential TPAD control
```

## 6. ICAO / EASA Comparison Boundary

No ICAO or EASA comparative assertion is populated in this record set.

This is intentional. REG-001 requires an explicit authoritative source provision before comparative analysis is recorded.

The next comparison cycle may select matching ICAO and EASA provisions for individual records, but comparison must remain separate from Thai legal applicability.

## 7. Lifecycle Boundary

`REG-KR-001` remains `draft` because the five-record set is not yet evidence-complete.

Approval of the record set will not itself determine legal applicability to TPAD.

## 8. Next Controlled Action

Complete exact provision retrieval for REG-KR-001-001 and REG-KR-001-002. Do not infer missing citations. Then perform a final evidence verification pass before Quality Review of REG-KR-001.
