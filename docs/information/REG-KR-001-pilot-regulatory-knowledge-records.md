---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Air Navigation Act
type: information
status: draft
version: 0.3.0
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

The project-provided consolidated text is the source of record. Provision verification is recorded only where the current source evidence provides sufficient section-level evidence.

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
| Provision target | Director-prescribed requirements; exact provision not established |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING — EXACT PROVISION NOT IDENTIFIED` |

**Verification result:** The source contains multiple provisions under which the Director may determine criteria, conditions, procedures, or other requirements. The current source evidence does not establish a single provision that can safely be used as the exact citation for the generic pilot assertion “Director Requirements”.

**Control boundary:** No generic Director-prescribed requirement is represented as a reusable evidence-complete record until its exact provision is identified.

### REG-KR-001-002 — Documents Required for Flight

| Field | Value |
|---|---|
| Identifier | REG-KR-001-002 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation |
| Provision target | Pilot record target retained; exact provision citation not established |
| TPAD applicability | `UNASSESSED` |
| Verification status | `PENDING — EXACT PROVISION TEXT/CITATION NOT RETRIEVED` |

**Verification result:** The current source-search evidence does not expose sufficient provision-level text to establish the exact citation for the pilot assertion concerning documents to be carried or available with an aircraft for flight.

**Control boundary:** No citation is inferred and the record is not promoted to evidence-complete status.

### REG-KR-001-003 — Airworthiness / No-Fly Conditions

| Field | Value |
|---|---|
| Identifier | REG-KR-001-003 |
| Source | Air Navigation Act B.E. 2497 consolidated text |
| Source family | Thai aviation law |
| Knowledge role | Legal Obligation / Regulatory Requirement context |
| Provision target | `มาตรา ๔๑/๘๘` and `มาตรา ๔๑/๘๙` |
| TPAD applicability | `UNASSESSED` |
| Verification status | `VERIFIED — SECTION-LEVEL` |

**Source-derived assertion:** Section 41/88 addresses restoration of an aircraft to a safe-flight condition before flight when the aircraft is considered unsafe for flight. Section 41/89 prohibits flight in specified conditions, including circumstances involving the airworthiness certificate.

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

**Source-derived assertion:** Section 41/93 addresses the requirement for a maintenance-organisation certificate and distinguishes three certificate types. Section 41/94 prohibits operation of a maintenance organisation without the required certificate from the Director.

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

**Source-derived assertion:** Section 50/16 establishes the National Civil Aviation Security Plan and section 50/27 identifies national security plans and related security-plan elements within the security framework.

The source also contains provisions concerning security plans for specific aviation actors. fileciteturn72file18 fileciteturn73file2

**Control boundary:** This record does not establish a TPAD security-plan obligation without a separate applicability assessment.

## 5. Final Evidence Verification Status

| Record | Final verification state |
|---|---|
| REG-KR-001-001 | **Pending — exact provision not identified** |
| REG-KR-001-002 | **Pending — exact provision text/citation not retrieved** |
| REG-KR-001-003 | **Verified — sections 41/88 and 41/89** |
| REG-KR-001-004 | **Verified — sections 41/93 and 41/94** |
| REG-KR-001-005 | **Verified — security-plan framework sections** |

Final result:

```text
Evidence-complete records     3 / 5
Evidence gaps                 2 / 5
```

The record set is therefore **not evidence-complete as a whole** and remains `draft`.

The two unresolved records are deliberately retained as controlled evidence gaps rather than being assigned inferred citations.

## 6. ICAO / EASA Comparison Boundary

No ICAO or EASA comparative assertion is populated in this record set.

This is intentional. REG-001 requires an explicit authoritative source provision before comparative analysis is recorded.

The next comparison cycle may select matching ICAO and EASA provisions for individual verified records, but comparison must remain separate from Thai legal applicability.

## 7. Lifecycle Boundary

`REG-KR-001` remains `draft` because two of the five records are not evidence-complete.

Approval of the record set will not itself determine legal applicability to TPAD.

## 8. Verification Decision

**Evidence Verification Result: PARTIAL PASS**

The pilot demonstrates that provision-level regulatory knowledge records can be constructed with controlled provenance and explicit evidence status. It does not yet demonstrate evidence completeness for all five records.

No further citation inference is authorized for REG-KR-001-001 or REG-KR-001-002 without additional source evidence.

## 9. Next Controlled Action

Proceed to Quality Review of REG-KR-001 as a **partial-evidence pilot**, with the two unresolved records explicitly recorded as non-blocking evidence gaps for this implementation test.
