---
id: REG-PILOT-001
title: Regulatory Knowledge Pilot Corpus — Air Navigation Act
type: information
status: draft
version: 0.2.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-08-20
updated: 2026-08-20
related:
  - AB-2.0
  - KB-001
  - DOM-001
  - REG-001
  - SEM-002
  - OBJ-001
  - REL-001
source_documents:
  - "พระราชบัญญัติการเดินอากาศ พ.ศ. 2497 และที่แก้ไขเพิ่มเติมจนถึงฉบับที่ 14 (Consolidated text)"
---

# REG-PILOT-001 — Regulatory Knowledge Pilot Corpus

## 1. Purpose

Establish the first controlled pilot corpus for D02 — Regulatory & Standards using one project-provided source document.

The pilot tests whether REG-001 can represent source identity, provision-level citation, requirement/obligation context, applicability boundaries, provenance, and evidence without converting interpretation into an authoritative legal conclusion.

## 2. Pilot Source

**Source:** พระราชบัญญัติการเดินอากาศ พ.ศ. 2497 และที่แก้ไขเพิ่มเติมจนถึงฉบับที่ 14 — Consolidated text.

**Source status:** Project-provided source document.

**Pilot status:** Controlled extraction draft.

This pilot does not claim that the consolidated source is the complete current regulatory corpus.

## 3. Pilot Objectives

1. Test source and provision identity.
2. Test requirement/obligation representation.
3. Test traceability from provision to evidence.
4. Test distinction between statutory text and subordinate requirements/regulations.
5. Preserve uncertainty where TPAD applicability has not been determined.

## 4. Evidence Register

| Record | Provision target | Source-derived observation | Knowledge role | Domain context | Applicability |
|---|---|---|---|---|---|
| RP-001-001 | Section 15/2 and related provisions | The Act contains provisions referring to requirements determined or prescribed by the Director. | Regulatory Requirement context | D02 | UNASSESSED |
| RP-001-002 | Section 16 | The Act requires specified aircraft documents/items for flight, including registration, airworthiness, journey log and crew licences, subject to stated exceptions. | Legal Obligation context | D02 / D03 | UNASSESSED |
| RP-001-003 | Sections 41/83–41/89 | The Act contains controls concerning unsafe aircraft, prohibition of flight, airworthiness certificate status, and conditions associated with maintenance/certification and flight. | Legal Obligation context | D02 / D03 / D05 | UNASSESSED |
| RP-001-004 | Sections 41/103–41/105 | The Act contains requirements concerning maintenance organisations, records, personnel, training policy, quality/assurance systems and related Director requirements. | Legal Obligation + Regulatory Requirement context | D02 / D05 / D06 / D08 | UNASSESSED |
| RP-001-005 | Sections 50/28–50/31 | The Act contains requirements concerning civil aviation security plans and related security/training controls. | Legal Obligation + Regulatory Requirement context | D02 / D04 | UNASSESSED |

The table records source-derived targets and observations. It is not a complete legal interpretation of any provision.

## 5. Provision-Level Evidence Notes

### RP-001-001 — Director Requirements

The source contains provisions that refer to requirements, criteria, procedures, conditions, or limitations prescribed by the Director. The pilot records this as a regulatory-requirement context and does not create the subordinate requirement unless its authoritative source is separately identified.

Evidence anchor: Section 15/2 and related provisions in the project-provided consolidated text.

### RP-001-002 — Documents Required for Flight

The source states that an aircraft shall not fly unless specified documents/items are present, including registration documentation, certificate of airworthiness, journey log and crew licences, subject to stated exceptions.

Evidence anchor: Section 16 in the project-provided consolidated text.

### RP-001-003 — Airworthiness / Flight Prohibition

The source contains controls concerning aircraft that are unsafe and circumstances in which flight is prohibited or an airworthiness certificate is temporarily invalid. The source also contains provisions addressing necessary flight to a registered operator base, maintenance organisation, or safe location under specified circumstances.

Evidence anchor: Sections 41/83–41/90 in the project-provided consolidated text.

### RP-001-004 — Maintenance Organisation Controls

The source contains provisions concerning maintenance organisation responsibilities and controls, including facilities/tools, manuals and records, quality control/quality assurance, maintenance records, personnel and training policy, together with requirements prescribed by the Director.

Evidence anchor: Sections 41/103–41/105 in the project-provided consolidated text.

### RP-001-005 — Aviation Security Plans

The source contains provisions concerning civil aviation security plans and associated security controls. The pilot records these provisions as source evidence for later controlled analysis without asserting direct TPAD applicability.

Evidence anchor: Sections 50/28–50/31 in the project-provided consolidated text.

## 6. Traceability Test

The pilot represents the target chain as:

```text
Thai Statutory Authority
        ↓
Air Navigation Act
        ↓
Section / Provision
        ↓
Requirement or Obligation
        ↓
[Applicability Assessment]
        ↓
[TPAD Control / Standard — only when established]
        ↓
[Procedure — only when established]
        ↓
Evidence
```

Bracketed stages remain unpopulated until appropriate evidence and authorized decisions exist.

## 7. Applicability Boundary

Applicability remains `UNASSESSED` for all five pilot records.

The Act contains differentiated regulated entities, activities, exceptions, certificates, and delegated requirements. Therefore the pilot must not infer direct TPAD applicability merely from the existence of a statutory provision.

No statement in this document is a legal opinion.

## 8. Semantic and Cross-Domain Boundary

The pilot does not create new Enterprise Object classes or relationship types.

Domain context is recorded separately from object identity and must remain compatible with OBJ-001 and REL-001.

Example:

```text
D02 Regulatory & Standards
        |
        +---- D03 Aviation Operations
        +---- D04 Safety & Security
        +---- D05 Airworthiness & Maintenance
        +---- D06 Training & Competency
        +---- D08 Quality & Assurance
```

These are domain-context examples only; actual relationships require evidence and REL-001.

## 9. ICAO / EASA Comparison Boundary

This version remains a **Thai-source extraction pilot**.

No individual pilot record is currently assigned an ICAO or EASA counterpart because the corresponding authoritative provisions have not yet been explicitly selected and verified for that record.

The REG-001 strategic baseline remains:

```text
Thai Authority
      +
ICAO
      +
EASA
      ↓
Comparative Analysis
```

Comparison will be performed only after the relevant ICAO/EASA provisions are explicitly identified and evidence-linked.

## 10. Evidence Quality Rules

A pilot record is acceptable for Quality Review only when:

- source identity is explicit;
- provision reference is sufficiently precise;
- source text is distinguished from interpretation;
- applicability is not inferred without evidence;
- domain context does not replace object identity;
- unsupported ICAO/EASA equivalence is not asserted; and
- the record remains within the controlled pilot boundary.

## 11. Out of Scope

- Full Act extraction.
- Legal applicability determination.
- Legal advice or authoritative legal interpretation.
- Complete CAAT regulatory corpus.
- Complete ICAO comparison.
- Complete EASA comparison.
- Compliance matrix.
- TPAD SOP creation.
- Knowledge Graph implementation.
- RAG implementation.

## 12. Current Decision State

```text
REG-001              APPROVED
        ↓
REG-PILOT-001        DRAFT v0.2.0
        ↓
Provision extraction READY FOR QUALITY REVIEW
        ↓
Quality Review       NOT STARTED
```

This artifact does not change AB-2.0, KB-001, DOM-001, or REG-001.

## 13. Source Evidence Notes

The project-provided consolidated Act contains, among other provisions, requirements and controls concerning aircraft documents for flight, airworthiness and flight prohibition, maintenance organisation controls, and civil aviation security. These source-derived observations form the limited basis of this pilot corpus.
