---
id: REG-001
title: Regulatory & Standards Knowledge Domain Baseline
type: information
status: draft
version: 0.2.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-08-20
updated: 2026-08-20
tags:
  - regulatory
  - standards
  - aviation
  - ICAO
  - EASA
  - traceability
  - compliance
related:
  - AB-2.0
  - KB-001
  - DOM-001
  - SEM-001
  - SEM-002
  - OBJ-001
  - REL-001
---

# REG-001 — Regulatory & Standards Knowledge Domain Baseline

## 1. Purpose

Define the minimum conceptual foundation for managing TPAD Regulatory & Standards Knowledge within D02 — Regulatory & Standards.

REG-001 establishes identity, authority, provenance, applicability, comparison, and traceability boundaries for regulatory and standards knowledge. It is a knowledge-domain baseline, not a legal compliance assessment and not a substitute for competent legal or regulatory determination.

## 2. Authority and Baseline Context

| Field | Value |
|---|---|
| Architecture Baseline | AB-2.0 |
| Architecture Freeze | Active |
| Phase | Phase 3 — Enterprise Knowledge Implementation |
| Foundation | KB-001 — Enterprise Knowledge Foundation Baseline |
| Domain architecture | DOM-001 — Enterprise Knowledge Domain Architecture |
| Domain | D02 — Regulatory & Standards |

REG-001 does not modify AB-2.0, KB-001, DOM-001, or the existing semantic foundation.

## 3. Scope

REG-001 covers regulatory and standards knowledge concerning:

- aviation law and regulation;
- international aviation standards and frameworks;
- administrative law and public-sector regulatory requirements;
- government procurement requirements where relevant to TPAD; and
- comparative aviation regulatory and standards baselines.

## 4. Knowledge-Role Taxonomy

REG-001 uses the following knowledge roles for D02 context. These roles do not replace the canonical Enterprise Object classes in OBJ-001.

```text
Regulatory / Standards Source
        |
        +-- Law
        +-- Regulation
        +-- Standard
        +-- Requirement
        +-- Obligation
        +-- Guidance
        +-- Administrative Decision / Order
```

The role indicates how the source or assertion functions within regulatory knowledge. It does not by itself establish legal effect.

## 5. Semantic Boundaries

The following concerns must remain distinct:

```text
Legal Obligation
        !=
Regulatory Requirement
        !=
International Standard
        !=
Comparative Regulatory Baseline
        !=
Adopted Standard
        !=
Internal TPAD Requirement
        !=
Reference / Benchmark
```

In particular, a comparative source must not be represented as a legal obligation merely because it is authoritative in another jurisdiction.

## 6. Strategic Regulatory & Standards Baseline

TPAD regulatory and standards analysis shall consider the following source classes, where relevant to the subject matter:

| Source class | Strategic role | Default authority meaning for TPAD |
|---|---|---|
| Thai law and national regulation | National legal/regulatory baseline | Potential direct legal authority, subject to applicability and competent interpretation. |
| CAAT regulatory instruments | National aviation regulatory baseline | Regulatory authority within its applicable scope. |
| Police laws and regulations | Organizational/public-sector authority | Authority within applicable TPAD scope. |
| ICAO framework | International aviation baseline | International standards/recommended framework; applicability depends on the relevant legal and organizational context. |
| EASA regulatory framework | Strategic comparative aviation baseline | Comparative regulatory baseline; not automatically a Thai legal obligation. |
| ISO and other recognized standards | Strategic management/technical reference | Reference or adopted standard only when an applicable decision/evidence establishes adoption. |

### 6.1 EASA Strategic Baseline Principle

EASA regulatory material shall be considered as a **strategic comparative baseline** whenever relevant to the aviation subject being analyzed.

The default semantic status of EASA material within this program is:

```text
EASA Regulatory Material
        |
        v
Comparative Regulatory Baseline
        |
        v
Comparative Analysis
        |
        v
TPAD Strategic Decision
```

EASA material shall not automatically be represented as a Thai legal obligation, CAAT requirement, or TPAD mandatory requirement.

### 6.2 Comparative Analysis

Where sufficient evidence exists, comparison may identify differences such as:

- equivalent approach;
- more stringent approach;
- less stringent approach;
- different regulatory approach; or
- no meaningful counterpart.

These comparison labels are analytical classifications and do not themselves constitute legal conclusions.

## 7. Authority and Provenance

Every material regulatory assertion shall identify its source and authority sufficiently to support traceability.

The minimum conceptual chain is:

```text
Authority
    |
    v
Source Document
    |
    v
Provision / Citation
    |
    v
Requirement / Obligation
```

A source reference should be sufficiently precise to locate the underlying provision, such as an applicable article, section, regulation, standard paragraph, or equivalent source identifier.

## 8. Regulatory Traceability

The target traceability model is:

```text
AUTHORITY
   |
   v
SOURCE DOCUMENT
   |
   v
PROVISION
   |
   v
REQUIREMENT / OBLIGATION
   |
   v
APPLICABILITY ASSESSMENT
   |
   v
TPAD CONTROL / STANDARD
   |
   v
PROCEDURE
   |
   v
EVIDENCE
```

This is a conceptual traceability model. Not every source will require every node type.

## 9. Applicability

REG-001 does not reduce applicability to a simple Yes/No field.

The conceptual model is:

```text
Source
   |
   v
Requirement
   |
   v
Applicability Assessment
   |
   v
Decision / Basis
   |
   v
Evidence
```

Possible analytical outcomes may include direct applicability, partial relevance, non-applicability, benchmark/reference use, organizational adoption, or another evidence-supported determination.

No outcome shall be interpreted as a legal conclusion unless made or validated by the competent authority.

## 10. TPAD Standard Relationship

A TPAD standard may be derived, adopted, or informed by multiple sources.

The model is:

```text
Thai Authority   ICAO   EASA   Other Standards
       \           |       |        /
        \          |       |       /
         +---------+-------+------+
                           |
                           v
                 Comparative Analysis
                           |
                           v
                  TPAD Strategic Decision
                           |
                           v
                    TPAD Standard
```

The existence of an external source does not by itself establish that TPAD has adopted that source.

## 11. Initial Pilot Corpus Boundary

The initial implementation pilot should use a limited, controlled corpus rather than ingesting the complete regulatory universe.

Candidate pilot sources already available to the program include:

1. Air Navigation Act B.E. 2497 and amendments/consolidated text.
2. Administrative Procedure Act B.E. 2539.
3. Public Procurement and Supplies Administration Act B.E. 2560.

The Chicago Convention and EASA material should be introduced after the relevant provisions have been selected and verified for the specific comparison task.

This section defines a pilot boundary only. It does not constitute a legal applicability determination.

## 12. Minimum Conceptual Regulatory Record

A regulatory knowledge record should be capable of representing, where applicable:

| Element | Purpose |
|---|---|
| Identifier | Persistent identity under SEM-002. |
| Source / Authority | Identifies originating authority or source family. |
| Source type | Identifies law, regulation, standard, guidance, etc. |
| Citation | Precise source location. |
| Provision / assertion | The relevant requirement or knowledge assertion. |
| Status | Applicable governed lifecycle/status context. |
| Effective information | Effective date or relevant temporal information where available. |
| Applicability assessment | TPAD relevance and basis, when assessed. |
| Comparative baseline | ICAO/EASA/other comparison context when applicable. |
| Evidence | Supporting evidence for the representation or assessment. |
| Relationships | Explicit REL-001 relationships where applicable. |

These are conceptual requirements and do not modify the existing Metadata Standard.

## 13. Evidence Model

The regulatory knowledge record must distinguish:

```text
Source Evidence
        !=
Interpretation
        !=
Applicability Decision
        !=
TPAD Standard
        !=
Implementation Evidence
```

Where interpretation or applicability has not been formally established, the repository must preserve that uncertainty rather than presenting an inferred conclusion as authoritative.

## 14. Scope Boundary

REG-001 does not:

- determine legal applicability for TPAD;
- provide legal advice;
- create a compliance matrix;
- create SOPs or procedures;
- establish regulatory hierarchy beyond what is supported by authoritative evidence;
- modify OBJ-001 or REL-001;
- modify AB-2.0, KB-001, or DOM-001;
- ingest the complete regulatory corpus;
- create a Knowledge Graph schema;
- create a database schema; or
- define AI/RAG architecture.

## 15. Relationship to D02 and Other Domains

D02 provides the regulatory and standards basis that may constrain or inform other knowledge domains.

Examples include:

```text
D02 Regulatory & Standards
        |
        +---- constrains ----> D03 Aviation Operations
        |
        +---- constrains ----> D04 Safety & Security
        |
        +---- constrains ----> D05 Airworthiness & Maintenance
        |
        +---- requires ------> D06 Training & Competency
        |
        +---- constrains ----> D08 Quality & Assurance
```

These are conceptual examples only. Actual object relationships must use REL-001 and supporting evidence.

## 16. Quality and Change Control

REG-001 is subject to the existing Enterprise Quality Governance framework and applicable document lifecycle controls.

Changes to the regulatory/standards taxonomy or baseline principles must be evidence-based and reviewed before controlled implementation.

EASA, ICAO, Thai legal/regulatory, and other source comparisons shall preserve source provenance and must not silently convert comparative findings into mandatory TPAD requirements.

## 17. Review Decision

This is **Review Draft v0.2** incorporating the approved project direction that EASA regulatory material is a standing strategic comparative baseline alongside Thai authority and ICAO sources where relevant.

This draft is not approved, released, or a legal applicability determination.

## 18. References

- AB-2.0 Architecture Baseline
- KB-001 — Enterprise Knowledge Foundation Baseline
- DOM-001 — Enterprise Knowledge Domain Architecture
- SEM-001 — Enterprise Semantic Principles
- SEM-002 — Enterprise Identifier Standard
- OBJ-001 — Enterprise Object Model
- REL-001 — Enterprise Relationship Model
- Enterprise Quality Management Framework
- Applicable Thai aviation, administrative, procurement, ICAO, EASA, and other authoritative source materials used in subsequent controlled implementation
