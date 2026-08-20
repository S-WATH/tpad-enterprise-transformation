---
id: REG-PILOT-001
title: Regulatory Knowledge Pilot Corpus — Air Navigation Act
 type: information
status: draft
version: 0.1.0
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

Establish the first controlled pilot corpus for D02 — Regulatory & Standards using one authoritative source document already held in the TPAD project repository/file set.

The pilot tests whether REG-001 can represent regulatory source identity, provision-level citation, requirement/obligation context, applicability boundaries, provenance, and evidence without converting interpretation into authoritative legal conclusions.

## 2. Pilot Source

**Source:** พระราชบัญญัติการเดินอากาศ พ.ศ. 2497 และที่แก้ไขเพิ่มเติมจนถึงฉบับที่ 14 — Consolidated text.

**Source status:** Project-provided source document.

**Pilot status:** Controlled extraction draft.

The pilot does not claim that the consolidated source is the complete current regulatory corpus. It is the selected source for this first implementation test.

## 3. Pilot Objectives

1. Test source and provision identity.
2. Test requirement/obligation representation.
3. Test traceability from Act provision to evidence.
4. Test distinction between statutory text and downstream Director requirements/regulations.
5. Test preservation of uncertainty where TPAD applicability has not been determined.

## 4. Controlled Extraction Boundary

The initial pilot intentionally selects a small set of provisions/themes visible in the source rather than extracting the entire Act.

| Pilot Record | Source reference | Knowledge theme | Initial role |
|---|---|---|---|
| RP-001-001 | Section 15/2 and related provisions referenced by the Act | Director authority / prescribed requirements | Regulatory Requirement context |
| RP-001-002 | Section 16 | Aircraft documents required for flight, including registration, airworthiness, journey log, crew licences and other prescribed items | Legal Obligation context |
| RP-001-003 | Sections 41/83–41/89 | Airworthiness safety controls, prohibition on flight in specified conditions, and restoration after maintenance/certification | Legal Obligation context |
| RP-001-004 | Section 41/103–41/105 | Approved maintenance organisation responsibilities, records, personnel, training policy, quality/assurance controls and Director requirements | Legal Obligation + Regulatory Requirement context |
| RP-001-005 | Sections 50/28–50/31 | Civil aviation security plans and approval requirements | Legal Obligation + Regulatory Requirement context |

The references above identify pilot targets. They are not a complete legal interpretation of the cited provisions.

## 5. Evidence Examples

### RP-001-001 — Director Requirements

The source contains provisions that delegate or refer to requirements determined by the Director, including provisions where applications or activities are to follow criteria and procedures specified in requirements.

Evidence example: the Act refers to criteria and procedures specified in the requirements for certain aircraft modification and production activities.

Classification:

```text
Source Type: Law
Knowledge Role: Regulatory Requirement context
Authority: Thai statutory framework
Applicability: UNASSESSED
Evidence: Source provision / citation required
```

### RP-001-002 — Documents Required for Flight

The source states that an aircraft shall not fly unless specified documents/items are present, including registration certificate, nationality and registration marks, certificate of airworthiness, journey log, crew licences, and other specified items, subject to stated exceptions.

Classification:

```text
Source Type: Law
Knowledge Role: Legal Obligation context
Applicability to TPAD: UNASSESSED
Evidence: Section 16 source text
```

### RP-001-003 — Airworthiness / No-Fly Conditions

The source provides controls concerning aircraft that are unsafe, including a Director power to prohibit flight and conditions under which an aircraft may fly after maintenance/certification. The source also specifies circumstances in which a certificate of airworthiness is temporarily invalid and identifies conditions prohibiting flight.

Classification:

```text
Source Type: Law
Knowledge Role: Legal Obligation context
Domain relevance: Airworthiness & Maintenance / Aviation Operations
Applicability to TPAD: UNASSESSED
Evidence: Sections 41/83–41/89 source text
```

### RP-001-004 — Maintenance Organisation Controls

The source specifies responsibilities of certificate holders and maintenance organisations, including facilities, tools, regulatory/airworthiness records, management and maintenance manuals, quality control and quality assurance systems, maintenance records, personnel, training policy, and reporting.

Classification:

```text
Source Type: Law
Knowledge Role: Legal Obligation + Regulatory Requirement context
Domain relevance: Airworthiness & Maintenance / Quality & Assurance / Training & Competency
Applicability to TPAD: UNASSESSED
Evidence: Sections 41/103–41/105 source text
```

### RP-001-005 — Aviation Security Plans

The source contains requirements concerning approved civil aviation security plans and related training/security-plan controls for relevant aviation entities.

Classification:

```text
Source Type: Law
Knowledge Role: Legal Obligation + Regulatory Requirement context
Domain relevance: Safety & Security
Applicability to TPAD: UNASSESSED
Evidence: Sections 50/28–50/31 source text
```

## 6. Traceability Test

The pilot shall be able to represent the following chain without inventing missing links:

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

Square-bracketed stages remain empty until evidence and authorized decisions exist.

## 7. Applicability Boundary

This pilot does **not** determine whether every selected provision applies directly to TPAD.

In particular, the Act contains definitions, exceptions, differentiated aviation activities, and provisions directed to particular regulated entities. The pilot therefore records applicability as `UNASSESSED` unless an authoritative assessment is available.

No statement in this document should be treated as a legal opinion.

## 8. Cross-Domain Context

The selected pilot records demonstrate why regulatory knowledge cannot be isolated from other domains:

```text
D02 Regulatory & Standards
        |
        +----> D03 Aviation Operations
        |
        +----> D04 Safety & Security
        |
        +----> D05 Airworthiness & Maintenance
        |
        +----> D06 Training & Competency
        |
        +----> D08 Quality & Assurance
```

These are domain-context examples only. Enterprise Object relationships must be established using OBJ-001 and REL-001 with supporting evidence.

## 9. EASA / ICAO Comparison Boundary

REG-PILOT-001 is intentionally a **Thai-source extraction pilot**.

ICAO and EASA are not yet asserted as comparative counterparts for individual pilot records in this version because the corresponding authoritative provisions have not been selected and verified for each specific comparison.

The REG-001 principle remains active:

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

## 10. Quality Acceptance Criteria

The pilot is ready for Quality Review only when the review can verify:

- each record has a source identity;
- each record has a sufficiently precise provision reference;
- source text is distinguished from interpretation;
- applicability is not inferred without evidence;
- domain context does not replace Enterprise Object identity;
- no unsupported ICAO/EASA equivalence is asserted; and
- the extraction remains limited to the approved pilot boundary.

## 11. Out of Scope

- Full Act extraction.
- Legal applicability determination.
- Legal advice or interpretation.
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
REG-PILOT-001        DRAFT
        ↓
Source extraction    IN PROGRESS
        ↓
Quality Review       NOT STARTED
```

This document is an implementation pilot artifact and does not change AB-2.0, KB-001, DOM-001, or REG-001.

## 13. Source Evidence Notes

The pilot source contains, among other provisions, requirements concerning aircraft documents carried for flight, airworthiness/no-fly conditions, maintenance organisation responsibilities, and aviation security plans. These source-derived observations are the basis for the selected pilot records.
