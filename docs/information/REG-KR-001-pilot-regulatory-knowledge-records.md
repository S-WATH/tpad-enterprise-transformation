---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Regulatory Chain Model
type: information
status: draft
version: 0.6.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-08-20
updated: 2026-09-07
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

The provision requires specified documents, manuals and information to be carried on each flight as originals or copies unless otherwise specified. The list includes, among other items, the AFM/equivalent, certificate of registration, certificate of airworthiness, noise certificate, applicable authorisations, specific approvals, aircraft radio licence where applicable, third-party liability insurance certificate(s), journey log/equivalent, ATS flight-plan details where applicable, suitable aeronautical charts, interception information, search-and-rescue information, relevant operations-manual material, MEL/CDL, NOTAM/AIS material, meteorological information, applicable passenger/cargo manifests, and other pertinent or State-required documentation. citeturn0search23

### 3.2 Parent-to-Subordinate Evidence

The CAAT Cover Regulation for TCAR OPS Part NCC/NCO establishes the scope of the non-commercial operations regulatory set and states that TCAR OPS Parts NCC and NCO lay down requirements for non-commercial operations, including requirements for non-commercial operations with complex motor-powered aircraft. citeturn1search0

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

The next applicability assessment must separately examine:

1. aircraft status/category;
2. operation type;
3. operator/organisation status;
4. whether the operation is within the scope of the civil aviation regulatory regime; and
5. any State-aircraft or public-service treatment applicable to the operation.

No equivalence between `TPAD state aircraft` and `Part NCC non-commercial operation` is inferred.

### 3.4 REG-KR-001-001 — Director Requirements

The generic label **“Director Requirements” is retired as an evidence-complete record concept.**

It is replaced for pilot purposes by a narrower discovery record:

**`REG-KR-001-001A — Director General–Issued Air Operations Requirements`**

Scope:

> Identify a specific air-operations subject for which the CAAT Director General has issued or approved a detailed requirement under the applicable statutory and regulatory authority.

The record is a **discovery container**, not a generic requirement statement.

The TCAR OPS Part-NCC source states that `must`/`shall` indicates where the Director General requires an organisation, owner or operator to comply with the defined requirement. citeturn1view0

This establishes the role of Director General requirements within the subordinate instrument, but it does not justify treating “Director Requirements” as one universal provision.

Current status:

`SUBJECT-SPECIFIC PROVISION REQUIRED`

The next step is to select one concrete subject from the existing pilot corpus and create a provision-specific record.

## 4. Updated Pilot Record Status

| Record | Parent level | Downstream level | Applicability | Current status |
|---|---|---|---|---|
| REG-KR-001-001 | Authority identified | Generic record retired | N/A | `REFINED → 001A` |
| REG-KR-001-001A | Director General authority identified | Subject-specific instrument not yet selected | `UNASSESSED` | `SUBJECT-SPECIFIC PROVISION REQUIRED` |
| REG-KR-001-002 | Parent framework identified | `TCAR OPS Part-NCC — NCC.GEN.140` | `UNASSESSED` | `DOWNSTREAM PROVISION IDENTIFIED` |
| REG-KR-001-003 | `มาตรา ๔๑/๘๘`, `๔๑/๘๙` | Not required for current assertion | `UNASSESSED` | `VERIFIED — PARENT PROVISION` |
| REG-KR-001-004 | `มาตรา ๔๑/๙๓`, `๔๑/๙๔` | Not required for current assertion | `UNASSESSED` | `VERIFIED — PARENT PROVISION` |
| REG-KR-001-005 | `มาตรา ๕๐/๑๖`, `๕๐/๒๗` | Actor-specific detail may require downstream trace | `UNASSESSED` | `PARENT FRAMEWORK VERIFIED` |

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

Comparative analysis remains deferred until the Thai provision's applicability and regulatory level are sufficiently established.

When comparison begins, it must operate at the corresponding requirement level:

```text
Thai Regulatory Chain
        ↓
Applicable Detailed Requirement
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

The discovery result demonstrates the regulatory-chain method and identifies a concrete downstream provision, but does not approve TPAD applicability or release the pilot record set.

## 8. Next Controlled Action

Perform a formal applicability assessment for `REG-KR-001-002 / NCC.GEN.140` against the TPAD operation category before selecting ICAO and EASA comparison provisions.

In parallel, select one specific subject for `REG-KR-001-001A` rather than continuing to search for a generic “Director Requirements” provision.
