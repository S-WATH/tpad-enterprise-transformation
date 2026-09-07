---
id: REG-PILOT-002
title: TPAD State/Police Aviation Regulatory Chain — Documents and Information Required for Flight
type: information
status: draft
version: 0.1.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-09-07
updated: 2026-09-07
related:
  - REG-001
  - REG-KR-001
  - REG-KR-001-002
  - REG-KR-001-001A
  - KB-001
  - DOM-001
  - AB-2.0
  - SEM-002
  - OBJ-001
  - REL-001
---

# REG-PILOT-002 — TPAD State/Police Aviation Regulatory Chain

## 1. Purpose

Establish the first TPAD State/Police Aviation regulatory-chain record for the subject:

> **Documents and information required for flight**

The purpose is to identify the authoritative Thai legal/regulatory basis applicable to TPAD, distinguish it from civil-aviation comparative requirements, and preserve a traceable path from authority to operational evidence.

This pilot does not create a new architecture, does not declare legal equivalence, and does not convert a civil aviation requirement into a TPAD requirement without an applicability determination.

## 2. Controlled Regulatory Chain

The pilot uses the approved REG-001 chain:

```text
Authority / Legal Basis
        |
        v
Legal / Regulatory Instrument
        |
        v
Detailed Provision
        |
        v
Requirement / Obligation
        |
        v
Applicability
        |
        v
TPAD Control / Standard
        |
        v
Evidence
```

For State/Police Aviation, an additional applicability gate is required before a civil-aviation provision can be treated as a TPAD obligation:

```text
Civil Aviation Provision
        |
        v
Scope / Applicability Test
        |
        +----> Applicable to TPAD
        |
        +----> Not directly applicable
        |          |
        |          v
        |     Search State/Police control regime
        |
        +----> Applicability unresolved
```

## 3. Subject Definition

**Subject:** Documents and information required to be carried, maintained, or otherwise available in connection with a flight.

The subject is intentionally broader than a single document list because the Thai legal framework may distribute controls across flight-plan, journey-log, personnel, aircraft-status, airworthiness, operational, security, and other regulatory provisions.

The pilot therefore does not assume that one provision must contain the complete document set.

## 4. Thai Parent-Law Applicability Gate

The consolidated Air Navigation Act provided for this project defines **"อากาศยานราชการ" (State aircraft / government aircraft)** by reference to Section 5.

Section 5 states that the Act does not apply to air navigation in military, police, customs, and other government services prescribed by Ministerial Regulation, except that flight planning under Section 18/1 and compliance with rules of the air under Sections 18/2 and 18/3 remain governed as provided in the Act.

Project evidence source:

- `พระราชบัญญัติการเดินอากาศ-2497-และที่แก้ไขเพิ่มเติม-จนถึงฉบับที่-14-Consolidated-text.pdf`
- Section 5, project source page 8 / parsed lines corresponding to the Section 5 text.

This establishes a statutory applicability boundary for Police Aviation. It does **not** mean that Police Aviation is unregulated; it means that the general civil aviation regime cannot be assumed to apply wholesale. Applicable State/Police Aviation controls must be traced separately, while the expressly retained provisions remain applicable.

## 5. Directly Relevant Parent-Law Controls Identified

### 5.1 Flight plan

Section 18/1 provides that every aircraft operating in the Kingdom must prepare a flight plan and notify the air traffic service unit, with the flight plan following the form, criteria and procedures prescribed in the applicable requirement.

This provision is expressly preserved by Section 5 for the excluded government services.

**Regulatory status:** PARENT PROVISION VERIFIED

**Applicability to TPAD:** DIRECTLY RELEVANT / PRESERVED BY SECTION 5

**Downstream discovery required:** Yes — identify the current detailed flight-plan form, criteria, procedures and applicable operational interfaces.

### 5.2 Rules of the air

Section 18/2 requires aircraft flying or moving in the Kingdom to comply with rules of the air prescribed in the applicable regulation.

Section 18/3 addresses aircraft registered under the Act and State aircraft operating outside the Kingdom, requiring compliance with the rules of the State concerned, or the prescribed rules where outside the territory of any State.

**Regulatory status:** PARENT PROVISIONS VERIFIED

**Applicability to TPAD:** DIRECTLY RELEVANT / PRESERVED BY SECTION 5

**Downstream discovery required:** Yes — identify the current detailed Rules of the Air instrument and determine the specific State-aircraft provisions applicable to TPAD operations.

### 5.3 Journey log / flight record

Section 16/1 provides that the aircraft registrant must provide a journey log for the aircraft, while where an air operator exists the responsibility rests with the air operator.

This provision must be read together with the Section 5 applicability boundary before being generalized to every TPAD aircraft and operation.

**Regulatory status:** PARENT PROVISION IDENTIFIED

**Applicability to TPAD:** REQUIRES OPERATION/REGISTRATION-SPECIFIC ASSESSMENT

**Downstream discovery required:** Yes.

## 6. Civil-Aviation Comparative Record: REG-KR-001-002

The pilot previously identified `TCAR OPS Part-NCC — NCC.GEN.140` as a detailed civil-aviation provision concerning documents, manuals and information to be carried on each flight.

Current CAAT evidence identifies TCAR OPS Part-NCC as the regulation for **non-commercial operations with complex motor-powered aircraft**. The current Issue 01 Revision 00 is dated 30 January 2026.

NCC.GEN.140 lists, among other items, the AFM/equivalent, registration and airworthiness certificates, noise certificate, authorisations, specific approvals, radio licence where applicable, third-party liability insurance, journey log/equivalent, flight-plan details where applicable, aeronautical charts, interception information, search-and-rescue information, relevant operations-manual material, MEL/CDL, NOTAM/AIS information, meteorological information, applicable manifests, and other pertinent or State-required documents.

Authoritative external source references:

- CAAT Requirement No. 116, TCAR OPS Part-NCC
- CAAT TCAR OPS Part-NCC, Issue 01 Revision 00, 30 January 2026
- CAAT Cover Regulation to TCAR OPS Part NCC/NCO

`NCC.GEN.140` remains a **civil-aviation comparative baseline**, not a confirmed TPAD obligation.

## 7. Applicability Determination

### 7.1 Current conclusion

**TCAR OPS Part-NCC / NCC.GEN.140: NOT DIRECTLY APPLICABLE TO TPAD ON CURRENT EVIDENCE**

This is an applicability conclusion, not a finding that the subject is unregulated.

The basis is:

1. The Thai Air Navigation Act expressly excludes police aviation from the general application of the Act under Section 5, subject to specifically retained provisions including flight planning and rules of the air.
2. TCAR OPS Part-NCC is a civil aviation regulation for non-commercial operations with complex motor-powered aircraft.
3. The evidence reviewed does not establish that a TPAD police/state-aircraft operation falls within the civil Part-NCC scope despite the operation potentially being non-commercial in an ordinary economic sense.
4. Therefore, the civil Part-NCC document-carrying requirement cannot be imported into TPAD merely because its operational subject is relevant.

### 7.2 Applicability status

| Element | Current determination | Evidence state |
|---|---|---|
| TPAD is a government/police aviation organisation | YES, project organizational context | Project authority / organisational evidence required for final record |
| Police aviation is expressly addressed by Section 5 | YES | Verified in consolidated Air Navigation Act |
| General civil aviation regime applies wholesale to police aviation | NO | Contradicted by Section 5 exclusion |
| TCAR OPS Part-NCC is a civil aviation regulation | YES | CAAT Requirement No. 116 / Part-NCC |
| NCC.GEN.140 applies directly to TPAD | NOT ESTABLISHED | No sufficient applicability evidence |
| TPAD has document/information controls for flight | YES as a control objective | Specific regulatory/control chain still to be discovered |
| Equivalent TPAD regulatory source identified | PARTIAL | Sections 16/1, 18/1, 18/2, 18/3 identified; downstream detail remains to be traced |

## 8. State/Police Aviation Regulatory Discovery Path

The next discovery path is therefore:

```text
Air Navigation Act Section 5
        |
        +---- Section 18/1 Flight Plan
        |
        +---- Section 18/2 Rules of Air
        |
        +---- Section 18/3 State Aircraft Outside Thailand
        |
        +---- Section 16/1 Journey Log
        |
        v
Detailed subordinate provisions / applicable requirements
        |
        v
Police / State aviation organisational controls
        |
        v
TPAD operational standards and procedures
        |
        v
Objective evidence
```

The discovery process must distinguish:

- a legal requirement;
- a regulatory implementation requirement;
- an internal TPAD control;
- an operational procedure; and
- evidence demonstrating implementation.

## 9. ICAO Baseline

Chicago Convention Article 3 provides the international State-aircraft framework. Aircraft used in military, customs and police services are treated as State aircraft for purposes of the Convention.

The ICAO material reviewed for this pilot supports the distinction between civil and State aircraft but does not, by itself, supply the complete TPAD document-carrying control set.

Therefore ICAO is used as the international normative baseline and source-discovery guide, not as a direct substitution for Thai law.

## 10. EASA Strategic Baseline

EASA Regulation (EU) 2018/1139 provides a useful comparative architecture. Article 2(3)(a) excludes aircraft conducting military, customs, police, search and rescue, firefighting, border control, coastguard or similar public-interest activities under Member State control from the Regulation's normal civil aviation scope.

EASA also documents an Article 2(6) mechanism under which a Member State may choose to apply specified sections of the Regulation to some or all of those otherwise excluded activities where the provisions can be effectively applied.

This is used only as a **strategic benchmark** for TPAD. It does not create an obligation for TPAD to comply with EASA rules.

The comparative lesson for TPAD is:

```text
Civil Aviation Regulatory Regime
            |
            +---- Civil operations
            |
            +---- State / Police operations
                         |
                         +---- separate State framework
                         |
                         +---- optional / deliberate adoption of civil standards
```

The project should therefore consider whether TPAD should deliberately adopt selected civil/ICAO/EASA-derived controls as internal standards after the Thai legal chain is established. Such a decision belongs to the later standards/control-design stage, not this applicability assessment.

## 11. Regulatory Knowledge Graph Implications

This pilot establishes **Regulatory Applicability Pattern C — State/Police Aviation Exclusion**:

```text
Parent Civil Aviation Law
        |
        +---- Civil Regulatory Instrument
        |          |
        |          +---- Detailed Civil Requirement
        |
        +---- Statutory State/Police Exclusion
                   |
                   +---- Retained Parent-Law Requirements
                   |
                   +---- Separate State/Police Regulatory Chain
                   |
                   +---- TPAD Control / Standard
```

The absence of a civil provision from the TPAD chain must not be recorded as an evidence gap. It may instead be an intentional applicability boundary requiring discovery of the corresponding State/Police control.

## 12. Findings

### Finding F-002-01 — Civil applicability boundary established

Police aviation is expressly excluded from the general application of the Air Navigation Act under Section 5, subject to stated exceptions. Therefore civil TCAR requirements must pass an applicability test before being treated as TPAD obligations.

### Finding F-002-02 — NCC.GEN.140 retained as comparative baseline

NCC.GEN.140 remains a valid and useful civil-aviation reference for the subject "documents and information required for flight", but it is not a confirmed TPAD legal obligation.

### Finding F-002-03 — TPAD equivalent control chain remains incomplete

Parent-law controls relevant to flight planning, rules of the air and journey logs have been identified. The detailed subordinate provisions and TPAD operational controls have not yet been fully traced.

### Finding F-002-04 — EASA confirms strategic architecture pattern

The EASA State-activity exclusion and opt-in mechanism provide a useful benchmark for designing a deliberate State/Police aviation safety-control framework without conflating civil regulatory applicability with State operations.

## 13. Evidence Quality Status

`REG-PILOT-002 = DRAFT / DISCOVERY COMPLETE FOR APPLICABILITY GATE / DOWNSTREAM TRACE INCOMPLETE`

No legal opinion is asserted. No TPAD SOP or compliance requirement is approved by this record.

## 14. Next Controlled Action

The next controlled action is to trace the **downstream requirements for Sections 16/1, 18/1, 18/2 and 18/3** and identify the specific Thai regulatory instruments, forms, rules, orders, or operational requirements applicable to TPAD.

Only after that chain is sufficiently complete should the project construct the TPAD control/evidence layer and perform requirement-level ICAO/EASA comparison.
