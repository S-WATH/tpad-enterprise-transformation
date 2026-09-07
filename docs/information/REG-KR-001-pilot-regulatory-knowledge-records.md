---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Regulatory Chain Model
type: information
status: draft
version: 0.7.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-08-20
updated: 2026-09-07
related:
  - REG-001
  - REG-PILOT-001
  - REG-PILOT-002
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

The provision requires specified documents, manuals and information to be carried on each flight as originals or copies unless otherwise specified. The list includes, among other items, the AFM/equivalent, certificate of registration, certificate of airworthiness, noise certificate, applicable authorisations, specific approvals, aircraft radio licence where applicable, third-party liability insurance certificate(s), journey log/equivalent, ATS flight-plan details where applicable, suitable aeronautical charts, interception information, search-and-rescue information, relevant operations-manual material, MEL/CDL, NOTAM/AIS material, meteorological information, applicable passenger/cargo manifests, and other pertinent or State-required documentation. citeturn0search23

### 3.2 Parent-to-Subordinate Evidence

The CAAT Cover Regulation for TCAR Part NCC/NCO establishes the scope of the non-commercial operations regulatory set and states that TCAR OPS Parts NCC and NCO lay down requirements for non-commercial operations, including requirements for non-commercial operations with complex motor-powered aircraft. citeturn1search0

The TCAR OPS Part-NCC document identifies itself as the regulation for **non-commercial operations with complex motor-powered aircraft**, states that `must`/`shall` indicates requirements imposed by the Director General, and states that TCAR OPS is based on the consolidated EU Regulation 965/2012 framework with specified amendments. citeturn1view0

The resulting evidence chain is therefore:

```text
Air Navigation Act
        |
        v
CAAT statutory regulatory authority
        |
        v
TCAR OPS / Cover Regulation
        |
        v
TCAR OPS Part-NCC
        |
        v
NCC.GEN.140
        |
        v
Detailed document-carrying requirement
```

The chain demonstrates the **regulatory-source pattern**. It does not by itself establish TPAD applicability.

### 3.3 Applicability Boundary for `NCC.GEN.140`

The current source establishes that Part NCC concerns **non-commercial operations with complex motor-powered aircraft**. It does not, from the evidence reviewed in this cycle alone, establish that a TPAD state-aircraft operation falls within that regulatory category.

Therefore:

`TCAR OPS Part-NCC applicability to TPAD = UNASSESSED`

No equivalence between `TPAD state aircraft` and `Part NCC non-commercial operation` is inferred.

### 3.4 REG-KR-001-001 — Director Requirements

The generic label **“Director Requirements” is retired as an evidence-complete record concept.**

It is replaced for pilot purposes by a narrower discovery record:

**`REG-KR-001-001A — Director General–Issued Air Operations Requirements`**

Scope:

> Identify a specific air-operations subject for which the CAAT Director General has issued or approved a detailed requirement under the applicable statutory and regulatory authority.

Current status:

`SUBJECT-SPECIFIC PROVISION REQUIRED`

## 4. REG-KR-001-003 — Flight Plan Requirement Record

**Subject:** Flight planning for TPAD State/Police Aviation operations in Thailand.

**Parent provision:** Air Navigation Act Section 18/1.

Section 18/1 requires every aircraft operating in the Kingdom to prepare a flight plan and notify the air traffic service unit, with the flight plan following the form, criteria and procedures prescribed in the applicable requirement. Section 5 expressly retains Section 18/1 for the government-service categories otherwise excluded from general application of the Act.

**Downstream instrument identified:** CAAT Requirement No. 114 — TCAR ANS Part-ROA (Rules of the Air), current publication identified by CAAT as the applicable rules-of-the-air / flight-planning instrument.

**Requirement-level provisions extracted from the current TCAR ANS Part-ROA:**

| Requirement | Requirement-level meaning | TPAD treatment at this stage |
|---|---|---|
| `ROA.4001` Submission of a flight plan | Establishes submission of the flight plan to the appropriate ATS framework, subject to the detailed conditions in the provision. | Direct regulatory input; internal procedure not yet designed |
| `ROA.4005` Contents of a flight plan | Specifies the information to be included in the flight plan. The current provision includes items such as aircraft identification, flight rules/type, aircraft number/type, equipment, departure information, route, destination/ETE, alternate, endurance, persons on board, emergency/survival equipment and other information. | Direct regulatory input; TPAD data-field mapping required |
| `ROA.4006` Acceptance of a flight plan | The first receiving unit checks format/data conventions, completeness and, to the extent possible, accuracy; takes action if needed for ATS acceptability; and indicates acceptance. | Interface requirement; TPAD/ATS coordination procedure required |
| `ROA.4010` Completion of a flight plan | Requires the applicable flight-plan form information to be completed unless otherwise prescribed by the appropriate ATS units. | Direct regulatory input; TPAD completion control required |
| `ROA.4015` Changes to a flight plan | Changes for IFR or controlled VFR flights must be reported as soon as practicable; significant changes for other VFR flights must also be reported as soon as practicable, subject to the provision's conditions. | Direct regulatory input; change-control procedure required |
| `ROA.4020` Closing a flight plan | Establishes the flight-plan closing/arrival-report interface where required. Failure may cause disruption to ATS and unnecessary SAR action. | Direct regulatory input; closure/evidence control required |

**Source evidence:** Current CAAT TCAR ANS Part-ROA, Section 4 Flight Plans, including `ROA.4001`, `ROA.4005`, `ROA.4006`, `ROA.4010`, `ROA.4015` and `ROA.4020`. CAAT AMC/GM further identifies the ATS reporting-office interface, flight-plan form/message models, AIP route-planning reference, acceptance workflow and arrival-report implications. citeturn4search5turn4search8

### 4.1 Requirement decomposition

The requirement set can now be represented without yet creating an SOP:

```text
R-18/1-01  Flight plan must be prepared/submitted
R-18/1-02  Required flight-plan information must be supplied
R-18/1-03  Flight plan must pass ATS acceptance/interface
R-18/1-04  Applicable flight-plan information must be complete
R-18/1-05  Required changes must be reported
R-18/1-06  Flight plan must be closed / arrival reported when required
```

These identifiers are **working requirement identifiers for this pilot record only**. They are not yet enterprise-standard identifiers and must not be treated as approved semantic identifiers.

### 4.2 TPAD Control Design Boundary

The requirement extraction is now sufficiently detailed to begin a later control-design step, but this record deliberately does **not** prescribe the TPAD SOP.

The next control-design questions are:

1. Who is the TPAD accountable role for flight-plan preparation?
2. What system/form is the authoritative TPAD flight-plan record?
3. Which flight-plan fields must be generated from authoritative aircraft/crew/mission data?
4. Who verifies completeness before submission?
5. How is ATS acceptance recorded?
6. How are changes controlled and communicated?
7. How is closure/arrival reporting recorded?
8. What evidence is retained and for how long under the applicable record-control regime?

These questions belong to **TPAD Control / Standard Design**, not to the legal applicability assertion.

## 5. Updated Pilot Record Status

| Record | Parent level | Downstream level | Applicability | Current status |
|---|---|---|---|---|
| REG-KR-001-001 | Authority identified | Generic record retired | N/A | `REFINED → 001A` |
| REG-KR-001-001A | Director General authority identified | Subject-specific instrument not yet selected | `UNASSESSED` | `SUBJECT-SPECIFIC PROVISION REQUIRED` |
| REG-KR-001-002 | Parent framework identified | `TCAR OPS Part-NCC — NCC.GEN.140` | `UNASSESSED` | `DOWNSTREAM PROVISION IDENTIFIED` |
| REG-KR-001-003 | Air Navigation Act Section 18/1 | `CAAT Requirement No. 114 / TCAR ANS Part-ROA` | `DIRECTLY RELEVANT / RETAINED` | `REQUIREMENT EXTRACTION COMPLETE — CONTROL DESIGN PENDING` |
| REG-KR-001-004 | `มาตรา ๔๑/๙๓`, `๔๑/๙๔` | Not required for current assertion | `UNASSESSED` | `VERIFIED — PARENT PROVISION` |
| REG-KR-001-005 | `มาตรา ๕๐/๑๖`, `๕๐/๒๗` | Actor-specific detail may require downstream trace | `UNASSESSED` | `PARENT FRAMEWORK VERIFIED` |

## 6. Important Methodological Result

The pilot has now demonstrated three useful regulatory-record patterns:

### Pattern A — Requirement is sufficiently specified in the parent Act

```text
Parent Act
   ↓
Provision
   ↓
Requirement
```

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

### Pattern C — Parent Act explicitly retains a requirement for an otherwise excluded State/Police activity

```text
Section 5 exclusion
        ↓
Retained Section 18/1
        ↓
CAAT Requirement No. 114
        ↓
ROA.4001–4020
        ↓
TPAD operational requirement
        ↓
TPAD control / evidence
```

`REG-KR-001-003` is the first pilot record demonstrating Pattern C at requirement level.

## 7. ICAO / EASA Comparison Boundary

Comparative analysis remains deferred until the Thai provision's applicability and regulatory level are sufficiently established.

For the flight-plan subject, the next comparison should operate at requirement level rather than comparing the parent Act with an entire foreign regulatory framework:

```text
Thai ROA.4001–4020
        ↕
ICAO corresponding flight-plan provisions
        ↕
EASA corresponding flight-plan provisions
        ↓
Gap / alignment analysis
        ↓
TPAD strategic control decision
```

EASA remains the Strategic Comparative Regulatory Baseline under REG-001.

No ICAO/EASA equivalence is asserted by this discovery.

## 8. Lifecycle Boundary

`REG-KR-001` remains `draft`.

The flight-plan requirement extraction is complete for the current pilot evidence set, but TPAD control design, procedure approval, and enterprise release remain pending.

## 9. Next Controlled Action

Perform **TPAD Flight Plan Control Design** from the extracted requirement set, beginning with the authoritative data source, accountable role, submission workflow, ATS acceptance evidence, change handling, closure/arrival reporting, and retained evidence.

Only after the TPAD control design is established should the project perform requirement-level ICAO/EASA comparison and determine whether additional internal TPAD standards are desirable.
