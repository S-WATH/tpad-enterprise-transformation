---
id: REG-KR-001
title: Pilot Regulatory Knowledge Records — Regulatory Chain Model
type: information
status: draft
version: 0.4.0
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

This revision adds a **Parent–Subordinate Regulatory Traceability Model** discovered during pilot implementation. The model recognizes that a primary statute may establish broad authority while detailed requirements may be specified in subordinate instruments such as CAAT regulations, TCAR, notifications, orders, or other instruments issued under delegated authority.

This deliverable does not create legal conclusions, TPAD controls, procedures, or ICAO/EASA equivalence.

## 2. Regulatory Source Model

A regulatory knowledge record shall not assume that the requirement of interest is fully specified in the parent Act.

The controlled search model is:

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

The exact relationship between instruments must be established from authoritative evidence. The diagram is a conceptual traceability pattern and does not create a universal legal hierarchy.

## 3. Regulatory Search Rule

When a pilot assertion cannot be located at the parent-law level, the correct next action is **not** to infer that the assertion is unsupported.

The search shall proceed through potentially relevant subordinate instruments where the parent instrument provides authority or framework for them.

Potential subordinate sources include, where applicable:

- CAAT regulations or requirements;
- TCAR and related regulatory instruments;
- notifications or orders issued under statutory authority;
- applicable ministerial or governmental regulations;
- technical standards or requirements issued under delegated authority; and
- other authoritative implementing instruments.

The existence and legal effect of a subordinate instrument must be verified from its own source.

## 4. Pilot Records and Regulatory-Chain Status

### REG-KR-001-001 — Director Requirements

| Field | Value |
|---|---|
| Identifier | REG-KR-001-001 |
| Parent source | Air Navigation Act B.E. 2497 consolidated text |
| Current chain status | `CHAIN-SEARCH REQUIRED` |
| Knowledge role | Regulation / Requirement context |
| TPAD applicability | `UNASSESSED` |
| Evidence status | `PARENT-AUTHORITY IDENTIFIED; DETAILED REQUIREMENT NOT YET TRACED` |

**Finding:** The parent Act contains multiple provisions under which the Director may determine criteria, conditions, procedures, or requirements. The generic pilot assertion “Director Requirements” is therefore too broad to map safely to one citation.

**Required next step:** Identify the specific subject matter intended by the record, then trace the relevant statutory authority to the subordinate instrument that specifies the detailed requirement, if one exists.

**Control boundary:** Do not create a generic reusable requirement record from the parent-law authority alone.

### REG-KR-001-002 — Documents Required for Flight

| Field | Value |
|---|---|
| Identifier | REG-KR-001-002 |
| Parent source | Air Navigation Act B.E. 2497 consolidated text |
| Current chain status | `CHAIN-SEARCH REQUIRED` |
| Knowledge role | Legal Obligation / Regulatory Requirement context |
| TPAD applicability | `UNASSESSED` |
| Evidence status | `PARENT-SOURCE INSUFFICIENT FOR DETAILED ASSERTION` |

**Finding:** The pilot assertion concerns specific aircraft documents required for flight. The parent Act alone should not be assumed to contain the complete operational detail.

**Required next step:** Trace the statutory authority to the relevant CAAT/TCAR or other subordinate instrument, then identify the exact detailed requirement and its exceptions/conditions.

**Control boundary:** No exact citation or TPAD applicability conclusion is inferred until the regulatory chain is verified.

### REG-KR-001-003 — Airworthiness / No-Fly Conditions

| Field | Value |
|---|---|
| Identifier | REG-KR-001-003 |
| Parent source | Air Navigation Act B.E. 2497 consolidated text |
| Provision | `มาตรา ๔๑/๘๘` and `มาตรา ๔๑/๘๙` |
| Chain status | `PARENT PROVISION VERIFIED` |
| TPAD applicability | `UNASSESSED` |
| Evidence status | `VERIFIED — SECTION-LEVEL` |

The parent Act itself provides relevant provisions addressing restoration to safe-flight condition and specified no-fly conditions. The record therefore does not require a subordinate-instrument citation merely to establish the source-derived assertion at this level. fileciteturn74file11

**Control boundary:** Applicability to TPAD state-aircraft operations remains unassessed.

### REG-KR-001-004 — Maintenance Organisation Controls

| Field | Value |
|---|---|
| Identifier | REG-KR-001-004 |
| Parent source | Air Navigation Act B.E. 2497 consolidated text |
| Provision | `มาตรา ๔๑/๙๓` and `มาตรา ๔๑/๙๔` |
| Chain status | `PARENT PROVISION VERIFIED` |
| TPAD applicability | `UNASSESSED` |
| Evidence status | `VERIFIED — SECTION-LEVEL` |

The parent Act itself identifies the maintenance-organisation certification framework and related prohibition. fileciteturn78file5

**Control boundary:** The record does not determine direct applicability to TPAD.

### REG-KR-001-005 — Aviation Security Plans

| Field | Value |
|---|---|
| Identifier | REG-KR-001-005 |
| Parent source | Air Navigation Act B.E. 2497 consolidated text |
| Provision | `มาตรา ๕๐/๑๖`, `มาตรา ๕๐/๒๗`, and related security-plan provisions |
| Chain status | `PARENT FRAMEWORK VERIFIED; ACTOR-SPECIFIC DETAIL MAY REQUIRE SUBORDINATE TRACE` |
| TPAD applicability | `UNASSESSED` |
| Evidence status | `VERIFIED — SECTION-LEVEL FOR SECURITY-PLAN FRAMEWORK` |

The parent Act establishes the national aviation-security plan framework and identifies related security-plan elements. Actor-specific requirements may require further regulatory-chain tracing. fileciteturn72file18 fileciteturn73file2

**Control boundary:** No TPAD security-plan obligation is inferred.

## 5. Evidence Status Summary

| Record | Current status |
|---|---|
| REG-KR-001-001 | Parent authority identified; subordinate-chain search required |
| REG-KR-001-002 | Parent source insufficient for detailed assertion; subordinate-chain search required |
| REG-KR-001-003 | Parent provision verified |
| REG-KR-001-004 | Parent provision verified |
| REG-KR-001-005 | Parent framework verified; detailed actor applicability may require subordinate trace |

The two earlier evidence gaps are therefore reclassified as **regulatory-chain discovery tasks**, not unsupported assertions.

## 6. ICAO / EASA Comparative Boundary

Comparative analysis shall be performed at the **corresponding requirement level**, not merely by comparing parent statutes with foreign detailed regulations.

```text
Thai Parent / Subordinate Chain
             |
             v
      Detailed Requirement
             |
      +------+------+
      |             |
     ICAO          EASA
      |             |
      +------+------+
             |
             v
    Comparative Analysis
             |
             v
      TPAD Strategic Decision
```

An ICAO or EASA provision may be recorded only when the corresponding authoritative provision has been explicitly selected and verified.

EASA remains a Strategic Comparative Regulatory Baseline under REG-001.

## 7. Methodology Finding

The pilot demonstrates that regulatory knowledge extraction must support **multi-level regulatory provenance**.

A parent Act may answer:

> “Who has authority and what framework exists?”

while a subordinate instrument may answer:

> “What exactly must the regulated party do?”

The repository must preserve both levels and their evidence-backed relationship.

## 8. Lifecycle Boundary

`REG-KR-001` remains `draft`.

This revision changes the methodology and traceability model but does not approve any new legal applicability, regulatory requirement, or TPAD control.

## 9. Next Controlled Action

Perform regulatory-chain discovery for `REG-KR-001-001` and `REG-KR-001-002` using the parent statutory authority as the starting point and the relevant CAAT / TCAR / subordinate instruments as the next evidence layer.

Do not promote either record to evidence-complete until the detailed provision and its authoritative source have been verified.
