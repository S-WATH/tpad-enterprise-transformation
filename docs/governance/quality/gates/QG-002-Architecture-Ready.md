---
id: QG-002
title: Architecture Ready
type: checklist
status: draft
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-23
updated: 2026-07-23
tags:
  - governance
  - quality
  - architecture
  - quality-gate
---

# QG-002 — Architecture Ready

## Objective

Confirm that an architecture artefact is sufficiently defined, traceable, and governed for review or for use by downstream work.

## Entry Condition

An architecture artefact is proposed for formal review, a decision, or downstream elaboration.

## Criteria and Required Evidence

| Criterion | Pass condition | Evidence |
|---|---|---|
| Purpose and scope | The artefact states the problem, scope, and intended use. | Artefact purpose and scope sections. |
| Traceability | Relevant mission, capability, requirement, regulation, or other upstream relationships are identified where applicable. | Metadata relationships or documented references. |
| Standard conformance | Required metadata, document type, naming, and lifecycle status conform to the applicable standards. | Reviewed front matter and document structure. |
| Decision governance | Material architectural choices and unresolved decisions are recorded through the applicable governance mechanism. | ADR or decision-record reference where applicable. |
| Review readiness | Assumptions, constraints, dependencies, and known gaps are explicit enough for a reviewer to assess. | Review record or artefact sections. |

## Outcome

- **Pass:** the artefact is ready for its stated review or downstream use.
- **Conditional pass:** only explicitly recorded, non-blocking gaps remain, with an owner and due action.
- **Fail:** scope, traceability, conformance, decision governance, or review evidence is insufficient.

## Record

Record the gate outcome with the architecture review or related work record, including evidence links and any approved exceptions.
