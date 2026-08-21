---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Regulatory Chain Model
type: information
status: draft
version: 0.5.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-08-20
updated: 2026-08-21
related:
  - REG-001
  - REG-PILOT-001
  - QR-REG-PILOT-001
  - KB-001
  - DOM-001
  - AB-2.0
  - SEM-002
  - OBJ-001
  - REL-001
---

# REG-KR-001 — Pilot Regulatory Knowledge Records

## 1. Purpose

Create reusable provision-level regulatory knowledge records while preserving source provenance, regulatory derivation, and TPAD applicability status.

The pilot has confirmed that a parent statute may establish authority and framework while detailed operational requirements are specified in subordinate instruments. Therefore the pilot uses a **Parent–Subordinate Regulatory Traceability Model**.

This deliverable does not create legal conclusions, TPAD controls, procedures, or ICAO/EASA equivalence.

## 2. Regulatory Chain Model

```text
Authority / Legal Basis
          |
          v
Parent Legal Instrument
          |
          | authorizes / delegates / establishes framework
          v
Subordinate Regulatory Instrument
          |
          | specifies / implements
          v
Detailed Provision
          |
          v
Requirement / Obligation
          |
          v
Applicability Assessment
          |
          v
TPAD Control / Standard
          |
          v
Evidence
```

The exact relationship between instruments must be established from authoritative evidence. This is a traceability pattern, not a universal legal hierarchy.

## 3. Regulatory-Chain Discovery Results

### 3.1 REG-KR-001-002 — Documents Required for Flight

**Discovery status: DOWNSTREAM PROVISION IDENTIFIED**

A detailed downstream requirement was identified in the current CAAT regulatory framework:

**Thailand Civil Aviation Regulation — Air Operations, Part NCC, `NCC.GEN.140 — Documents, manuals and information to be carried`.**

The provision states that specified documents, manuals and information are to be carried on each flight as originals or copies unless otherwise specified. The listed material includes, among other items, the AFM/equivalent, original certificate of registration, original certificate of airworthiness, noise certificate, applicable authorisations, specific approvals, aircraft radio licence where applicable, third-party liability insurance certificate(s), journey log/equivalent, filed ATS flight plan where applicable, current suitable aeronautical charts, interception information, and search-and-rescue information. citeturn0search23

The CAAT source identifies this as **TCAR OPS Part-NCC** and therefore provides the detailed downstream regulatory layer that the parent-law pilot record was unable to expose directly.

### 3.2 Parent-to-Subordinate Evidence

The current CAAT cover regulation for TCAR OPS Part NCC/NCO states that CAAT issues detailed requirements under the Air Navigation Act and identifies statutory powers and responsibilities under the Act as the legal basis for the TCAR OPS detailed requirements. It also states that the Director General issues the detailed aircraft-operation regulation and that TCAR OPS Parts contain the detailed requirements. citeturn1search14

This confirms the **regulatory-chain pattern** for the pilot:

```text
Air Navigation Act
        |
        v
CAAT statutory regulatory authority
        |
        v
TCAR OPS Air Operations
        |
        v
TCAR OPS Part NCC
        |
        v
NCC.GEN.140
        |
        v
Detailed document-carrying requirement
```

### 3.3 Applicability Boundary

`NCC.GEN.140` is evidence of a detailed CAAT requirement, but this discovery does **not** establish that the provision applies to TPAD state aircraft.

Applicability remains:

`UNASSESSED`

The pilot must separately determine whether the aircraft/activity/operator category covered by Part NCC corresponds to the TPAD operation under study. No equivalence is inferred.

### 3.4 REG-KR-001-001 — Director Requirements

The generic label **“Director Requirements” is not sufficiently specific to remain an evidence-complete reusable knowledge record.**

Chain discovery shows that the Director General's authority is exercised through specific regulatory instruments. For example, the current TCAR OPS cover regulation explicitly states that the Director General issues detailed regulations concerning aircraft operations under statutory authority, and that TCAR OPS Parts contain the detailed requirements. citeturn1search14

The TCAR ANS Part ROA also states that it is issued pursuant to Section 16/5 of the Air Navigation Act and that CAAT is responsible for issuing requirements on air navigation and flight operations; it further states that “shall” identifies requirements for which the Director General requires compliance. citeturn1search13

Therefore the correct modeling decision is:

```text
“Director Requirements”
        ↓
Too generic for a reusable record
        ↓
Replace with a subject-specific requirement
        ↓
Trace statutory authority → specific CAAT/TCAR instrument → provision
```

No single provision is assigned to the generic record.

## 4. Updated Pilot Record Status

| Record | Parent level | Downstream level | Current status |
|---|---|---|---|
| REG-KR-001-001 | Authority identified | Subject-specific instrument not selected | `REFINE RECORD SCOPE` |
| REG-KR-001-002 | Parent framework identified | `TCAR OPS Part NCC — NCC.GEN.140` identified | `DOWNSTREAM PROVISION IDENTIFIED` |
| REG-KR-001-003 | `มาตรา ๔๑/๘๘`, `๔๑/๘๙` | Not required for current assertion | `VERIFIED — PARENT PROVISION` |
| REG-KR-001-004 | `มาตรา ๔๑/๙๓`, `๔๑/๙๔` | Not required for current assertion | `VERIFIED — PARENT PROVISION` |
| REG-KR-001-005 | `มาตรา ๕๐/๑๖`, `๕๐/๒๗` | Actor-specific detail may require downstream trace | `PARENT FRAMEWORK VERIFIED` |

## 5. Important Methodological Result

The pilot has now demonstrated two different valid regulatory-record patterns:

### Pattern A — Requirement is sufficiently specified in the parent Act

```text
Parent Act
   ↓
Provision
   ↓
Requirement
```

Examples in this pilot include the identified airworthiness/no-fly and maintenance-organisation provisions.

### Pattern B — Parent Act establishes authority/framework; subordinate instrument specifies detail

```text
Parent Act
   ↓
Delegated / Regulatory Authority
   ↓
CAAT / TCAR Instrument
   ↓
Detailed Provision
   ↓
Requirement
```

`REG-KR-001-002` is the first confirmed pilot example of Pattern B.

## 6. ICAO / EASA Comparison Boundary

Comparative analysis must operate at the corresponding requirement level.

```text
Thai Regulatory Chain
        ↓
Detailed Requirement
        ↕
ICAO Corresponding Provision
        ↕
EASA Corresponding Provision
        ↓
Comparative Analysis
        ↓
TPAD Strategic Decision
```

EASA remains the Strategic Comparative Regulatory Baseline under REG-001.

No ICAO/EASA equivalence is asserted by this discovery.

## 7. Lifecycle Boundary

`REG-KR-001` remains `draft`.

The discovery result is sufficient to demonstrate the regulatory-chain method but is not sufficient to approve TPAD applicability or to release the pilot record set.

## 8. Next Controlled Action

Refine `REG-KR-001-001` into a specific subject-matter record rather than continuing to search for a generic “Director Requirements” provision.

For `REG-KR-001-002`, verify the exact applicability scope of TCAR OPS Part NCC and then select the corresponding ICAO and EASA provisions for comparative analysis.
