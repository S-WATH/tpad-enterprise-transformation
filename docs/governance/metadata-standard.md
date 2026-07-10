---
id: GOV-MDS-001
title: Metadata Standard
type: standard
status: draft
version: 1.0.0
domain: governance
owner: TPAD Enterprise Transformation Team
created: 2026-07-10
updated: 2026-07-10
tags:
  - metadata
  - governance
---

# Metadata Standard

## Purpose

เอกสารนี้กำหนดมาตรฐาน Metadata สำหรับ TPAD Enterprise Knowledge Base เพื่อให้เอกสารทุกฉบับมีโครงสร้างที่สม่ำเสมอ รองรับการค้นหา การเชื่อมโยง การตรวจสอบย้อนกลับ และการประยุกต์ใช้กับระบบสารสนเทศในอนาคต

---

# Design Principles

- Metadata First
- Keep Required Fields Minimal
- Human Readable
- Machine Readable
- Technology Agnostic
- Extensible by Design

---

# Metadata Classification

Metadata แบ่งออกเป็น 3 ระดับ

| Level | Description |
|--------|-------------|
| Mandatory | ทุกเอกสารต้องมี |
| Recommended | ควรมีในเอกสารส่วนใหญ่ |
| Optional | ใช้เมื่อจำเป็น |

---

# Mandatory Fields

| Field | Description |
|--------|-------------|
| id | Persistent Identifier (PID) ของเอกสาร |
| title | ชื่อเอกสาร |
| type | ประเภทเอกสาร |
| status | สถานะของเอกสาร |
| version | เวอร์ชัน |
| domain | หมวดองค์ความรู้หลัก |

---

# Recommended Fields

| Field | Description |
|--------|-------------|
| owner | ผู้รับผิดชอบเอกสาร |
| created | วันที่สร้าง |
| updated | วันที่แก้ไขล่าสุด |
| tags | คำสำคัญสำหรับการค้นหา |

---

# Optional Fields

| Field | Description |
|--------|-------------|
| reviewers | ผู้ตรวจทาน |
| approver | ผู้อนุมัติ |
| related | เอกสารที่เกี่ยวข้อง |
| references | เอกสารอ้างอิง |
| parent | เอกสารแม่ |
| children | เอกสารลูก |
| summary | สรุปเนื้อหา |

---

# Metadata Template

```yaml
---
id:
title:
type:
status:
version:
domain:

owner:
created:
updated:
tags:
---
```

---

# Status Values

ค่าที่อนุญาต

- draft
- review
- approved
- released
- archived

---

# Domain Values

ตัวอย่าง Domain

- governance
- foundation
- mission
- capability
- regulation
- requirement
- organization
- process
- information
- application
- technology
- ai
- history

---

# Naming Rules

- Field Name ใช้ภาษาอังกฤษทั้งหมด
- ใช้ lowercase
- ห้ามใช้ช่องว่างในชื่อ Field
- Field ใหม่ต้องผ่าน Architecture Decision Record (ADR)

---

# Future Expansion

หากมีความจำเป็น สามารถเพิ่ม Metadata Field ได้ผ่าน ADR โดยต้องไม่ทำลาย Compatibility กับ Metadata Version ก่อนหน้า