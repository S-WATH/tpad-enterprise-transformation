---
id: GOV-PID-001
title: Persistent Identifier (PID) System
type: standard
status: draft
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-10
updated: 2026-07-10
tags:
  - governance
  - pid
  - identifier
---

# Persistent Identifier (PID) System

## Purpose

กำหนดระบบ Persistent Identifier (PID) สำหรับ Enterprise Objects ทั้งหมดของ TPAD Enterprise Knowledge Base เพื่อให้สามารถอ้างอิง เชื่อมโยง และติดตามวัตถุต่าง ๆ ได้ตลอดวงจรชีวิต โดยไม่ขึ้นกับชื่อไฟล์ ชื่อเอกสาร หรือเทคโนโลยีที่ใช้จัดเก็บ

---

# Design Principles

- Persistent
- Unique
- Human Readable
- Machine Readable
- Technology Agnostic
- Globally Extensible

---

# PID Structure

```
<OBJECT>-<DOMAIN>-<NUMBER>
```

Example

```
MIS-FLT-001
REQ-MX-012
SOP-OPS-005
MAN-CAMO-001
```

---

# Object Prefix Registry

| Prefix | Enterprise Object |
|---------|-------------------|
| MIS | Mission |
| CAP | Capability |
| REG | Regulation |
| REQ | Requirement |
| ORG | Organization |
| PRO | Process |
| SOP | Standard Operating Procedure |
| MAN | Manual |
| WI | Work Instruction |
| FRM | Form |
| CHK | Checklist |
| TMP | Template |
| ADR | Architecture Decision Record |
| WS | Working Session |
| CP | Checkpoint |
| REL | Release |
| RSK | Risk |
| ISS | Issue |
| AST | Asset |
| POS | Position |
| COM | Competency |
| TRN | Training |

---

# Domain Registry

| Domain | Description |
|---------|-------------|
| FLT | Flight Operations |
| MX | Maintenance |
| CAMO | Continuing Airworthiness |
| TRG | Training |
| LOG | Logistics |
| SUP | Support |
| GOV | Governance |
| HR | Human Resources |
| SAF | Safety |
| QMS | Quality Management |

---

# Numbering Rules

- ใช้เลข 3 หลัก เริ่มจาก 001
- ห้ามนำ PID ที่ยกเลิกแล้วกลับมาใช้ใหม่
- PID เป็น Permanent Identifier
- การเปลี่ยนชื่อ Object ไม่มีผลต่อ PID

---

# PID Lifecycle

Reserved

↓

Assigned

↓

Active

↓

Retired

PID ที่ Retired ต้องคงอยู่ใน Registry เพื่อรักษา Traceability

---

# PID Authority

การกำหนด PID อยู่ภายใต้การควบคุมของ TPAD Governance Team

หน้าที่ประกอบด้วย

- สงวน Prefix
- อนุมัติ Domain ใหม่
- ป้องกัน PID ซ้ำ
- ดูแล PID Registry

---

# Future Expansion

รองรับการเพิ่ม Namespace เช่น

```
TPAD-MIS-FLT-001
```

โดยไม่กระทบ PID เดิม