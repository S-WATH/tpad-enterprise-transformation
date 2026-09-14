---
id: REG-PILOT-003
title: Regulatory Applicability — Provision-Level Evidence Matrix
type: information
status: draft
version: 0.1.0
domain: regulatory-and-standards
owner: TPAD Enterprise Transformation Team
created: 2026-09-14
updated: 2026-09-14
tags:
  - regulatory
  - applicability
  - evidence
  - state-aviation
  - police-aviation
  - maintenance
related:
  - REG-001
  - REG-KR-001
  - REG-PILOT-001
  - REG-PILOT-002
  - MNT-001
  - AB-2.0
---

# REG-PILOT-003 — Regulatory Applicability — Provision-Level Evidence Matrix

## 1. Status and Purpose

**Status:** Draft — not approved.

This document is the Phase 3 provision-level regulatory applicability analysis deliverable. It translates the current regulatory-chain work into an evidence matrix at provision level, with particular attention to the statutory State/Police Aviation boundary and the maintenance/airworthiness interface.

This document is an **applicability and evidence analysis**, not a legal opinion. It does not authorize implementation, establish a maintenance organisation, confer authority on any post-holder, or adopt a civil aviation standard as an internal TPAD requirement.

The analysis uses the controlled project sources currently available in the repository/project context, especially:

- `REG-001` — Regulatory and Standards Knowledge Domain Baseline;
- `REG-PILOT-002` — TPAD State/Police Aviation Regulatory Chain;
- `MNT-001` — Maintenance Operating Model — AS-IS Discovery;
- `พระราชบัญญัติการเดินอากาศ-2497-และที่แก้ไขเพิ่มเติม-จนถึงฉบับที่-14-Consolidated-text.pdf`;
- `กฏหมายการเดินอากาศระหว่างประเทศ (อนุสัญญาชิคาโก ค.ศ.1944)_1.pdf`.

## 2. Applicability Decision Rules

The matrix distinguishes the following states:

- **Directly relevant / retained** — the parent law expressly retains the provision for State/Police Aviation or otherwise establishes a direct applicability pathway.
- **Not directly applicable through the parent civil regime** — the provision belongs to a civil aviation regime excluded by the statutory State/Police boundary; a separate State/Police control must be traced before treating it as a TPAD obligation.
- **Applicability unresolved** — the available evidence is insufficient to determine whether another legal instrument, registration status, or State/Police-specific instrument activates the requirement.
- **Comparative baseline only** — useful for benchmarking or future deliberate internal adoption, but not a confirmed legal obligation.

Evidence confidence is expressed as:

- **High** — provision and applicability boundary are directly visible in a controlled source;
- **Medium** — provision is identified, but downstream or TPAD-specific applicability evidence remains incomplete;
- **Low** — indication exists, but the available source set is insufficient for a reliable determination.

## 3. Provision-Level Evidence Matrix

| ID | Provision | Requirement / effect | Applies to whom | TPAD Police Aviation applicability | Evidence | Confidence | Unresolved issue |
|---|---|---|---|---|---|---|---|
| RAE-001 | Air Navigation Act §5 | General Act does not apply to military, police, customs and other prescribed government air navigation, subject to stated exceptions. | Military, police, customs and prescribed government aviation; exceptions remain. | **Direct statutory boundary.** TPAD Police Aviation is within the stated police-aviation exclusion unless another provision or instrument establishes a separate pathway. | Consolidated Act, p.8, §5. | High | Identify all other Thai State/Police Aviation instruments that regulate the excluded activity. |
| RAE-002 | Air Navigation Act §5 exception + §18/1 | Flight planning under §18/1 remains governed by the Act even for excluded State/Police Aviation. | Aircraft operating in Thailand, including the retained State/Police interface. | **Directly relevant / retained.** | Consolidated Act, p.8, §5; p.25, §18/1. | High | Trace TPAD flight-plan procedure, submission interface and any State-aircraft exceptions in the downstream instrument. |
| RAE-003 | Air Navigation Act §18/1 | Every aircraft flying in Thailand must make and notify a flight plan according to prescribed requirements. | Aircraft operating in Thailand. | **Directly relevant / retained by §5.** | Consolidated Act, p.25, §18/1; REG-PILOT-002 identifies CAAT Requirement No. 114 / TCAR ANS Part-ROA as the downstream instrument. | High | Establish the exact TPAD operational control and any applicable State-aircraft procedures. |
| RAE-004 | Air Navigation Act §18/2 | Aircraft flying or moving in Thailand must comply with prescribed rules of the air. | Aircraft flying or moving in Thailand. | **Directly relevant / retained by §5.** | Consolidated Act, p.25, §18/2; REG-PILOT-002 identifies CAAT Requirement No. 114 / TCAR ANS Part-ROA. | High | Map State-aircraft provisions in ROA into TPAD operational controls and evidence. |
| RAE-005 | Air Navigation Act §18/3 | Thai-registered aircraft and Thai State aircraft outside Thailand follow the rules of the State concerned; if over no State, follow prescribed rules. | Thai-registered aircraft and Thai State aircraft outside Thailand. | **Directly relevant for external operations.** | Consolidated Act, p.25, §18/3; REG-PILOT-002 identifies ROA.1001 for high-seas operations. | High | Build destination/airspace-specific applicability records for each foreign operation. |
| RAE-006 | Air Navigation Act §16/1 | Registrant must provide a journey log; where an air operator exists, responsibility rests with the air operator; detailed form/retention/recording follows prescribed requirements. | Aircraft registrants / air operators within the Act's applicable regime. | **Applicability unresolved.** §16/1 is not one of the provisions expressly retained by §5 for excluded police aviation. | Consolidated Act, pp.23–24, §16/1; REG-PILOT-002 identifies CAAT Requirement No. 69 as downstream civil instrument. | Medium | Determine TPAD aircraft registration/status basis and identify State/Police journey-log or equivalent flight-record control. |
| RAE-007 | Air Navigation Act §41/77 | Aircraft with a certificate of airworthiness must be maintained in safe usable condition; maintenance criteria, methods and intervals follow Director's requirements. | Aircraft with certificates of airworthiness within the Act's airworthiness regime. | **Not directly applicable through the general civil regime to Police Aviation under §5.** Do not import as a TPAD obligation without a separate applicability basis. | Consolidated Act, p.55, §41/77; §5 at p.8. | High | Identify State/Police airworthiness and maintenance legal/control regime applicable to TPAD aircraft. |
| RAE-008 | Air Navigation Act §41/79 | Replacement parts used in maintenance must satisfy specified product/standard-part conditions. | Maintenance of aircraft with certificates of airworthiness within the Act's regime. | **Not directly applicable through the general civil regime to Police Aviation under §5.** | Consolidated Act, p.55, §41/79; §5 at p.8. | High | Identify TPAD-specific part-acceptance, traceability and release requirements from the State/Police regime. |
| RAE-009 | Air Navigation Act §41/80 | Registrant must maintain maintenance history and supporting airworthiness certificates, prepare maintenance reports and comply with prescribed procedures. | Aircraft registrants / air operators within the Act's regime. | **Not directly applicable through the general civil regime to Police Aviation under §5.** This provision is nevertheless highly relevant as a comparative control model for the MNT-001 evidence gaps. | Consolidated Act, pp.55–56, §41/80; §5 at p.8; MNT-001. | High | Determine the legally required TPAD maintenance-record set and retention/reporting regime independently. |
| RAE-010 | Air Navigation Act §§41/81–41/84 | Inspection, defect correction, safety notification and return-to-service certification mechanisms are established within the civil airworthiness regime. | Aircraft and responsible parties within that regime. | **Not directly applicable through the general civil regime to Police Aviation under §5.** | Consolidated Act, pp.56–57, §§41/81–41/84; §5 at p.8. | High | Identify TPAD State/Police defect escalation, inspection and return-to-service authority/control basis. |
| RAE-011 | Air Navigation Act §41/88 | If the aircraft controller considers the aircraft unsafe to fly, the controller must notify a mechanic for maintenance before flight. | Controller/mechanic within the applicable airworthiness regime. | **Not directly established for TPAD through the general civil regime.** | Consolidated Act, p.57, §41/88; §5 at p.8. | High | Establish TPAD defect-to-maintenance escalation and formal authority from documentary evidence; do not infer authority from job titles. |
| RAE-012 | Air Navigation Act §§41/94–41/104 | Certification, scope, management, release certification, authorised signatories, records, quality systems and subcontracting controls for certified maintenance organisations. | Certified maintenance organisations and associated personnel within the Act's civil maintenance regime. | **Not directly applicable through the general civil regime to Police Aviation under §5.** | Consolidated Act, pp.59–62, §§41/94–41/104; §5 at p.8. | High | Determine whether TPAD maintenance is governed by another State/Police instrument and, separately, whether TPAD deliberately adopts equivalent controls as an internal standard. |
| RAE-013 | Chicago Convention Art. 3(a) | Convention applies to civil aircraft and not to State aircraft. | Contracting States / civil and State aircraft distinction. | **International normative boundary / comparative baseline.** Supports the civil-versus-State distinction; does not by itself define the TPAD control set. | Chicago Convention source, Article 3(a). | High | Confirm the Thai implementation and any State-aircraft operational instruments relevant to TPAD. |
| RAE-014 | Chicago Convention Art. 3(b) | Aircraft used in military, customs and police services are deemed State aircraft. | Military, customs and police services. | **Directly relevant as international State-aircraft classification baseline.** | Chicago Convention source, Article 3(b). | High | Preserve distinction between international classification and specific Thai domestic obligations. |
| RAE-015 | Chicago Convention Art. 3(c) | State aircraft shall not fly over another State or land there without authorisation by special agreement or otherwise and according to its terms. | State aircraft operating internationally. | **Relevant for TPAD international operations.** | Chicago Convention source, Article 3(c); Thai Act §18/3. | High | Identify diplomatic/State-aircraft permissions and foreign-state operational requirements for actual TPAD missions. |
| RAE-016 | TCAR OPS Part-NCC / NCC.GEN.140 | Civil operational requirement concerning documents, manuals and information carried on each flight. | Civil non-commercial operations with complex motor-powered aircraft within the stated civil scope. | **Comparative baseline only; not established as a TPAD legal obligation.** | REG-PILOT-002 records NCC.GEN.140 and CAAT Requirement No. 116 as civil instruments; §5 excludes Police Aviation from wholesale civil treatment. | Medium | Decide later whether selected controls should be deliberately adopted as TPAD internal standards after legal chain and control design are complete. |

## 4. Maintenance Applicability Finding

The provision-level analysis materially changes the treatment of the maintenance findings in `MNT-001`.

The consolidated Air Navigation Act contains a substantial civil airworthiness and maintenance regime, including continuing airworthiness, maintenance records, defect correction, return-to-service certification, certified maintenance organisations, authorised signatories, quality systems and subcontracting controls. However, Section 5 establishes that the Act does not generally apply to police aviation. The Act expressly retains flight planning and rules of the air under Sections 18/1–18/3, but does not expressly retain the cited maintenance provisions.

Therefore:

1. **The civil maintenance provisions are not to be treated as confirmed TPAD legal obligations.**
2. They remain **important comparative control references** for assessing whether the current TPAD maintenance model has equivalent control needs.
3. The next legal discovery task is to identify the **State/Police Aviation maintenance and airworthiness regime** applicable to TPAD aircraft.
4. `MNT-001` findings such as document-centric records, historical retrieval gaps, parts-history gaps, defect-tracking gaps and fleet-status visibility gaps are **evidence/control-design issues**, not findings of legal non-compliance with §§41/77–104.

## 5. Relationship to MNT-001

| MNT-001 finding | Regulatory implication from this matrix | Current action |
|---|---|---|
| F1 Dual Maintenance Execution Model | Civil maintenance-organisation provisions cannot be assumed to govern both internal and outsourced work. | Identify State/Police authority and control basis for each execution mode. |
| F2 Outsourced Maintenance Contract-Based Interface | Civil subcontracting rules are not automatically applicable. Contract controls still require separate procurement/authority/evidence analysis. | Trace applicable State/Police requirements and procurement controls. |
| F3 Document-Centric Maintenance Records | Civil §41/80 provides a strong comparative record-control model, but is not confirmed TPAD law. | Identify TPAD legal record requirements and define evidence model later. |
| F4 Historical Records Retrieval Gap | Record availability is a control concern regardless of whether §41/80 applies. | Validate documentary evidence and retention requirements. |
| F5 Defect Tracking Gap | Civil §§41/81–84 provide a comparative defect/safety control pattern. | Trace TPAD defect reporting, escalation and return-to-service authority. |
| F6 Parts History Information Gap | Civil §41/79 and §41/80 provide comparative traceability controls. | Identify TPAD parts acceptance and traceability basis. |
| F7 Fleet Status Visibility Gap | Civil airworthiness provisions indicate the importance of current aircraft status, but do not establish TPAD law. | Define TPAD status evidence only after State/Police control basis is established. |

## 6. Key Regulatory Conclusions

### 6.1 Established

- Section 5 establishes a statutory civil-versus-State/Police applicability boundary.
- Sections 18/1 and 18/2 are expressly retained for excluded State/Police aviation.
- Section 18/3 directly governs Thai State aircraft operating outside Thailand, together with the rules of the foreign State or applicable high-seas rules.
- The Act contains a detailed civil airworthiness and maintenance regime, but those provisions are not thereby converted into Police Aviation obligations.

### 6.2 Not Established

The current source set does **not** establish:

- that CAAT civil maintenance organisation requirements apply directly to TPAD Police Aviation;
- that Part-145, CAMO, MOE, CAME or Part-M concepts are statutory TPAD obligations;
- that CAAT Requirement No. 69 on journey logs directly applies to TPAD;
- that a TPAD post-holder has maintenance release authority merely from a job title;
- that current TPAD practice is compliant or non-compliant with any unverified civil maintenance provision.

### 6.3 Required Next Discovery

The next controlled regulatory work should trace the State/Police regime for:

1. aircraft registration/status and State-aircraft classification in Thailand;
2. maintenance and continuing-airworthiness responsibility;
3. technical records and journey/flight records;
4. defect reporting, inspection and return-to-service authority;
5. parts acceptance and traceability;
6. internal versus outsourced maintenance authority;
7. requirements imposed through contracts, procurement instruments or other Thai administrative instruments;
8. subordinate regulations or Director/CAAT instruments that may independently establish applicability to State/Police aviation.

## 7. Evidence and Governance Boundary

This matrix is a draft analytical record. It must not be read as an approval of any target operating model.

The evidence hierarchy remains:

```text
Source Document
      ↓
Provision / Citation
      ↓
Requirement / Obligation
      ↓
Applicability Assessment
      ↓
TPAD Control / Standard
      ↓
Procedure
      ↓
Evidence
```

The matrix deliberately stops before converting an applicability finding into an implemented TPAD control.

No identity, appointment, delegation or formal authority is inferred from a job title or organisational label.

## 8. Next Controlled Actions

1. Validate the E1 findings in `MNT-001` against documentary evidence.
2. Identify and analyse the State/Police Aviation maintenance and airworthiness instruments.
3. Build a separate State/Police provision matrix for maintenance, records, defects, parts and release authority.
4. Update evidence confidence and unresolved issues as documentary evidence is obtained.
5. When the analysis is sufficiently complete, submit `REG-PILOT-003` for Review under the document lifecycle.
6. Do not use this draft as authority to implement a civil maintenance organisation model or to declare TPAD compliant/non-compliant with civil aviation rules.

## 9. Lifecycle

`Draft → Review → Approved → Released → Archived`

No approval record is present in this draft.
