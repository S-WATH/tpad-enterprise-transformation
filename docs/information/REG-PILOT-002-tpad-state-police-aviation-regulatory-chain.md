---
id: REG-PILOT-002
title: TPAD State/Police Aviation Regulatory Chain — Documents and Information Required for Flight
type: information
status: draft
version: 0.2.0
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

The consolidated Air Navigation Act provided for this project defines the State/Police Aviation boundary through Section 5.

Section 5 states that the Act does not apply to air navigation in military, police, customs, and other government services prescribed by Ministerial Regulation, except that flight planning under Section 18/1 and compliance with rules of the air under Sections 18/2 and 18/3 remain governed as provided in the Act.

Project evidence source:

- `พระราชบัญญัติการเดินอากาศ-2497-และที่แก้ไขเพิ่มเติม-จนถึงฉบับที่-14-Consolidated-text.pdf`
- Section 5, together with Sections 16/1 and 18/1–18/3.

This establishes a statutory applicability boundary for Police Aviation. It does **not** mean that Police Aviation is unregulated; it means that the general civil aviation regime cannot be assumed to apply wholesale. Applicable State/Police Aviation controls must be traced separately, while the expressly retained provisions remain applicable.

## 5. Downstream Trace — Sections 16/1, 18/1, 18/2 and 18/3

### 5.1 Section 18/1 — Flight plan

The parent Act requires every aircraft operating in the Kingdom to prepare a flight plan and notify the air traffic service unit. The flight plan is to follow the form, criteria and procedures prescribed in the applicable requirement.

The current CAAT downstream instrument identified is:

**CAAT Requirement No. 114 — TCAR ANS Part-ROA (Rules of the Air)**

- Published: 18 November 2025
- Replaces CAAT Requirement No. 94
- Authority basis includes Air Navigation Act Section 18/1.
- Current CAAT publication identifies the associated TCAR ANS Part-ROA as the current rules-of-the-air / flight-planning instrument.

Within TCAR ANS Part-ROA, the flight-plan provisions are located in Section 4:

- `ROA.4001` — Submission of a flight plan
- `ROA.4005` — Contents of a flight plan
- `ROA.4006` — Acceptance of a flight plan
- `ROA.4010` — Completion of a flight plan
- `ROA.4015` — Changes to a flight plan
- `ROA.4020` — Closing a flight plan

The current CAAT ROA publication states that a flight plan is required for the operation of any flight in the Bangkok FIR and specifies submission timing, contents, changes and closing procedures.

**Regulatory status:** DOWNSTREAM INSTRUMENT IDENTIFIED

**Applicability to TPAD:** DIRECTLY RELEVANT / PRESERVED BY SECTION 5

**Important qualification:** The present record establishes the existence and subject matter of the downstream civil regulatory instrument. It does not yet establish every TPAD-specific operational exception, coordination arrangement, or internal procedure. Those remain control-design and applicability-detail work.

### 5.2 Section 18/2 — Rules of the air

The parent Act requires aircraft flying or moving in the Kingdom to comply with rules of the air prescribed in the applicable regulation.

The current downstream instrument identified is:

**CAAT Requirement No. 114 — TCAR ANS Part-ROA (Rules of the Air), Issue 01 Revision 01**

The CAAT publication states that the rules of the air apply to all aircraft within Thailand. It also contains explicit State-aircraft provisions, including provisions allowing or exempting State aircraft in specified operational circumstances.

Key provisions relevant to the TPAD State/Police Aviation chain include:

- `ROA.2001` — rules of the air apply to all aircraft within Thailand;
- `ROA.2005` — aircraft operations shall comply with the rules of the air;
- `ROA.5001` — VMC minima, including a State-aircraft provision within activated TRA or AMC Manageable Area;
- `ROA.5005` — VFR requirements, including specific State-aircraft provisions;
- Section 11 — interference, emergency contingencies and interception;
- `ROA.11015` — interception.

**Regulatory status:** DOWNSTREAM INSTRUMENT IDENTIFIED

**Applicability to TPAD:** DIRECTLY RELEVANT / PRESERVED BY SECTION 5

**Key finding:** Unlike the civil Part-NCC document-carrying rule, the current Rules of the Air instrument expressly addresses State aircraft in several operational provisions. Therefore the project should not treat the entire TCAR ROA as merely a civil comparative reference; the retained Section 18/2 legal chain creates a direct relevance pathway for State/Police Aviation.

### 5.3 Section 18/3 — State aircraft outside Thailand

The parent Act provides that aircraft registered under the Act and Thai State aircraft operating outside Thailand must comply with the rules of air prescribed by the State whose territory they are operating in. If the aircraft is not within the territory of any State, it must comply with the rules prescribed in the applicable regulation.

The current CAAT TCAR ANS Part-ROA contains a directly relevant high-seas provision:

- `ROA.1001` — for all aircraft registered in Thailand and Thai State aircraft operating over the high seas, the rules of the air apply without exception.

For operations within another State's territory, the primary operational rule remains the law/rules of the State being overflown, consistent with Section 18/3.

**Regulatory status:** PARENT RULE VERIFIED; DOWNSTREAM HIGH-SEAS RULE IDENTIFIED

**Applicability to TPAD:** DIRECTLY RELEVANT when TPAD State aircraft operate outside Thailand

**Downstream discovery required:** Yes — for each foreign State/territory in which TPAD may operate, identify the applicable State rules, diplomatic/State-aircraft permissions, and operational arrangements. The project should not infer foreign-state applicability from the Thai TCAR alone.

### 5.4 Section 16/1 — Journey log

Section 16/1 requires the aircraft registrant to provide a journey log for the aircraft, while where an air operator exists the responsibility rests with the air operator.

The current CAAT downstream instrument identified is:

**CAAT Requirement No. 69 — Journey Log**

- Published: 18 October 2024
- Authority basis includes Air Navigation Act Section 16/1 paragraphs two and three.
- It replaced the earlier Civil Aviation Board Regulation No. 5 on Journey Logs, which is recorded by CAAT as repealed.

**Regulatory status:** DOWNSTREAM CIVIL INSTRUMENT IDENTIFIED

**Applicability to TPAD:** NOT DIRECTLY ESTABLISHED

The reason is structural rather than evidentiary: Section 16/1 is not one of the provisions expressly retained by Section 5 for the excluded police aviation regime. Therefore Requirement No. 69 must not be imported into TPAD merely because it implements Section 16/1 for civil aviation.

**Next discovery required:** Determine whether TPAD State aircraft are registered under the Air Navigation Act framework in a manner that activates Section 16/1, and separately identify any State/Police Aviation journey-log or flight-record requirement imposed by another Thai legal or organisational instrument.

## 6. Current Downstream Regulatory Chain Matrix

| Parent provision | Downstream instrument | Current finding | TPAD applicability | Next action |
|---|---|---|---|---|
| Section 16/1 | CAAT Requirement No. 69 — Journey Log | Identified | NOT DIRECTLY ESTABLISHED | Determine registration/status basis and State/Police alternative control |
| Section 18/1 | CAAT Requirement No. 114 — TCAR ANS Part-ROA | Identified | DIRECTLY RELEVANT / RETAINED | Trace TPAD flight-plan procedure and interfaces |
| Section 18/2 | CAAT Requirement No. 114 — TCAR ANS Part-ROA | Identified | DIRECTLY RELEVANT / RETAINED | Trace State-aircraft provisions into TPAD operational controls |
| Section 18/3 | Foreign State rules + CAAT ROA.1001 for high seas | Identified | DIRECTLY RELEVANT for external operations | Build destination/airspace applicability matrix |

## 7. Civil-Aviation Comparative Record: REG-KR-001-002

The pilot previously identified `TCAR OPS Part-NCC — NCC.GEN.140` as a detailed civil-aviation provision concerning documents, manuals and information to be carried on each flight.

Current CAAT evidence identifies TCAR OPS Part-NCC under CAAT Requirement No. 116 as the regulation for non-commercial operations with complex motor-powered aircraft.

`NCC.GEN.140` remains a **civil-aviation comparative baseline**, not a confirmed TPAD obligation.

The new downstream trace does not change that conclusion. The distinction is now clearer:

- **Section 18/1 and 18/2 chain:** retained by Section 5 and therefore directly relevant to State/Police Aviation;
- **Section 16/1 chain:** not expressly retained by Section 5, therefore applicability to TPAD remains unresolved;
- **Part-NCC/NCC.GEN.140:** civil operational requirement and not directly established as applicable to TPAD.

## 8. Applicability Determination

### 8.1 Current conclusion

**TPAD State/Police Aviation is not to be treated as a wholesale civil Part-NCC operation.**

However, the downstream trace demonstrates that the statutory exclusion in Section 5 does **not** remove all civil aviation regulatory interfaces. Sections 18/1, 18/2 and 18/3 are expressly retained and therefore form part of the direct regulatory chain for State/Police Aviation.

### 8.2 Updated applicability status

| Element | Current determination | Evidence state |
|---|---|---|
| Police aviation is expressly addressed by Section 5 | YES | Verified in consolidated Air Navigation Act |
| Flight planning under Section 18/1 is retained | YES | Verified in parent Act |
| Current downstream flight-plan instrument identified | YES — CAAT Requirement No. 114 / TCAR ANS Part-ROA | CAAT current publication |
| Rules of the air under Section 18/2 are retained | YES | Verified in parent Act |
| Current downstream Rules of Air instrument identified | YES — CAAT Requirement No. 114 / TCAR ANS Part-ROA | CAAT current publication |
| TCAR ROA contains State-aircraft provisions | YES | Current CAAT ROA publication |
| Section 18/3 high-seas downstream rule identified | YES — ROA.1001 | Current CAAT ROA publication |
| Section 16/1 downstream civil instrument identified | YES — CAAT Requirement No. 69 | CAAT current publication |
| Requirement No. 69 directly applies to TPAD | NOT ESTABLISHED | Section 5 does not expressly retain Section 16/1 |
| TCAR OPS Part-NCC / NCC.GEN.140 directly applies to TPAD | NOT ESTABLISHED | Civil scope/applicability evidence insufficient |
| TPAD equivalent document/record control chain | PARTIAL | Flight plan and rules-of-air chain advanced; journey-log/state records remain incomplete |

## 9. State/Police Aviation Regulatory Discovery Path

The updated discovery path is:

```text
Air Navigation Act Section 5
        |
        +---- Section 18/1 Flight Plan
        |          |
        |          +---- CAAT Requirement No. 114 / TCAR ANS Part-ROA
        |                    |
        |                    +---- ROA.4001–4020
        |                    |
        |                    +---- TPAD flight-plan control
        |
        +---- Section 18/2 Rules of Air
        |          |
        |          +---- CAAT Requirement No. 114 / TCAR ANS Part-ROA
        |                    |
        |                    +---- ROA.2001 / 2005 and State-aircraft provisions
        |                    |
        |                    +---- TPAD rules-of-air control
        |
        +---- Section 18/3 State Aircraft Outside Thailand
        |          |
        |          +---- Foreign State rules
        |          +---- ROA.1001 for high seas
        |          +---- TPAD international-operation control
        |
        +---- Section 16/1 Journey Log
                   |
                   +---- CAAT Requirement No. 69
                   |
                   +---- TPAD applicability unresolved
                   +---- Search State/Police record-control regime
```

The discovery process must distinguish:

- a legal requirement;
- a regulatory implementation requirement;
- a State/Police applicability rule;
- an internal TPAD control;
- an operational procedure; and
- evidence demonstrating implementation.

## 10. ICAO Baseline

Chicago Convention Article 3 provides the international State-aircraft framework. Aircraft used in military, customs and police services are treated as State aircraft for purposes of the Convention.

The ICAO baseline supports the distinction between civil and State aircraft but does not, by itself, supply the complete TPAD document-carrying control set.

Therefore ICAO is used as the international normative baseline and source-discovery guide, not as a direct substitution for Thai law.

## 11. EASA Strategic Baseline

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
                         +---- retained public-interest rules
                         |
                         +---- separate State framework
                         |
                         +---- deliberate adoption of selected civil standards
```

The project should therefore consider whether TPAD should deliberately adopt selected civil/ICAO/EASA-derived controls as internal standards after the Thai legal chain is established. Such a decision belongs to the later standards/control-design stage, not this applicability assessment.

## 12. Regulatory Knowledge Graph Implications

This pilot establishes **Regulatory Applicability Pattern C — State/Police Aviation Exclusion with Retained Air Navigation Controls**:

```text
Parent Civil Aviation Law
        |
        +---- Civil Regulatory Instrument
        |          |
        |          +---- Civil Requirement
        |
        +---- Statutory State/Police Exclusion
                   |
                   +---- Retained Flight Plan / Rules of Air Controls
                   |          |
                   |          +---- Downstream TCAR ANS Part-ROA
                   |
                   +---- Separate State/Police Regulatory Chain
                   |
                   +---- TPAD Control / Standard
```

The absence of a civil provision from the TPAD chain must not be recorded automatically as an evidence gap. It may be an intentional applicability boundary requiring discovery of the corresponding State/Police control.

## 13. Findings

### Finding F-002-01 — Civil applicability boundary established

Police aviation is expressly excluded from the general application of the Air Navigation Act under Section 5, subject to stated exceptions. Therefore civil TCAR requirements must pass an applicability test before being treated as TPAD obligations.

### Finding F-002-02 — Retained flight-plan and rules-of-air chain identified

Sections 18/1 and 18/2 are expressly retained by Section 5. Current CAAT downstream evidence identifies Requirement No. 114 / TCAR ANS Part-ROA as the current implementation instrument, including detailed flight-plan provisions and rules-of-air provisions that expressly address State aircraft in specified circumstances.

### Finding F-002-03 — Section 18/3 external-operation chain identified at two levels

For operations outside Thailand, Section 18/3 directs compliance with the rules of the State concerned. For high-seas operations, CAAT TCAR ANS Part-ROA `ROA.1001` expressly applies the rules of the air to Thai State aircraft without exception.

### Finding F-002-04 — Journey-log downstream source identified but TPAD applicability unresolved

CAAT Requirement No. 69 implements Section 16/1 for journey logs, but Section 16/1 is not expressly retained by Section 5. TPAD applicability therefore remains unresolved and requires a separate State/Police registration and record-control assessment.

### Finding F-002-05 — NCC.GEN.140 remains comparative only

NCC.GEN.140 remains a useful civil-aviation baseline for documents and information required for flight, but the downstream State/Police chain now provides a more appropriate route for identifying TPAD obligations.

### Finding F-002-06 — Regulatory chain has progressed from parent law to implementation instrument

The pilot has moved beyond the parent-law applicability gate for Sections 18/1, 18/2 and 18/3. The next work is now requirement-level extraction and TPAD operational-control mapping rather than further high-level applicability debate.

## 14. Evidence Quality Status

`REG-PILOT-002 = DRAFT / DOWNSTREAM TRACE ESTABLISHED FOR SECTIONS 18/1, 18/2 AND 18/3 / SECTION 16/1 APPLICABILITY UNRESOLVED / TPAD CONTROL DESIGN NOT YET APPROVED`

No legal opinion is asserted. No TPAD SOP or compliance requirement is approved by this record.

## 15. Next Controlled Action

The next controlled action is to extract the **specific requirement-level controls from TCAR ANS Part-ROA relevant to TPAD operations**, beginning with:

1. `ROA.4001–4020` — flight-plan lifecycle;
2. `ROA.2001 / 2005` and State-aircraft provisions — rules of the air;
3. `ROA.1001` — high-seas State-aircraft operations; and
4. the applicable Section 16/1 / Requirement No. 69 provisions, only after confirming whether the TPAD aircraft/operation falls within their applicability.

Only after requirement-level extraction should the project construct the TPAD control/evidence layer and perform requirement-level ICAO/EASA comparison.
