---
id: GOV-DLS-001
title: Document Lifecycle Standard
type: standard
status: draft
version: 1.0.0
owner: TPAD Enterprise Transformation Team
created: 2026-07-08
updated: 2026-07-08
tags:
  - governance
  - document
  - lifecycle
---

# Document Lifecycle Standard

## Purpose

กำหนดวงจรชีวิตของเอกสารภายใน TPAD Enterprise Transformation Program เพื่อให้ทุกเอกสารมีสถานะที่ชัดเจน สามารถตรวจสอบย้อนกลับได้ และมีการควบคุมการเปลี่ยนแปลงอย่างเป็นระบบ

---

# Lifecycle

```text
Draft
    ↓
Review
    ↓
Approved
    ↓
Released
    ↓
Archived
```

---

# Status Definitions

| Status | Description |
|---------|-------------|
| Draft | เอกสารอยู่ระหว่างการจัดทำ ยังไม่สามารถใช้อ้างอิงอย่างเป็นทางการ |
| Review | อยู่ระหว่างการตรวจสอบและให้ข้อเสนอแนะ |
| Approved | ได้รับการอนุมัติด้านเนื้อหา พร้อมเผยแพร่ |
| Released | ประกาศใช้เป็นเอกสารทางการของโครงการ |
| Archived | ยกเลิกการใช้งาน แต่ยังเก็บไว้เพื่อการอ้างอิงย้อนหลัง |

---

# Lifecycle Rules

1. เอกสารทุกฉบับต้องเริ่มต้นด้วยสถานะ **Draft**
2. การเปลี่ยนจาก **Draft → Review** ต้องเกิดเมื่อผู้จัดทำเห็นว่าเนื้อหาครบถ้วน
3. การเปลี่ยนจาก **Review → Approved** ต้องได้รับความเห็นชอบจาก Program Sponsor
4. การเปลี่ยนจาก **Approved → Released** ต้องผ่านการ Commit และ Push เข้าสู่ Repository หลัก
5. เอกสารที่ถูกแทนที่หรือเลิกใช้ ให้เปลี่ยนสถานะเป็น **Archived** ห้ามลบออกจาก Repository

---

# Versioning

- การแก้ไขเล็กน้อย (Minor Edit) เพิ่มเลขเวอร์ชันรอง
- การเปลี่ยนแปลงสำคัญ (Major Change) เพิ่มเลขเวอร์ชันหลัก
- ทุกการเปลี่ยนแปลงต้องสามารถตรวจสอบย้อนหลังผ่าน Git History ได้

---

# Responsibilities

| Role | Responsibility |
|------|----------------|
| Author | จัดทำและปรับปรุงเอกสาร |
| Reviewer | ตรวจสอบความถูกต้อง |
| Program Sponsor | อนุมัติเนื้อหา |
| Repository Maintainer | ดูแลมาตรฐานและความสอดคล้องของ Repository |

---

# Notes

มาตรฐานนี้ใช้กับเอกสารทุกประเภทภายใน Repository เว้นแต่จะมีมาตรฐานเฉพาะกำหนดไว้เป็นอย่างอื่น