---
id: GOV-DTS-001
title: Document Type Standard
type: standard
status: draft
version: 1.0.0
owner: TPAD Enterprise Transformation Team
created: 2026-07-08
updated: 2026-07-08
tags:
  - governance
  - document
  - standard
---

# Document Type Standard

## Purpose

กำหนดประเภทเอกสารมาตรฐานที่ใช้ภายใน TPAD Enterprise Transformation Program เพื่อให้ทุกเอกสารมีโครงสร้าง การจัดเก็บ และการอ้างอิงที่เป็นมาตรฐานเดียวกัน

---

# Design Principles

- One Purpose per Document
- One Document Type per File
- Every Document Has Metadata
- Every Document Has Unique ID
- Every Document Is Traceable

---

# Document Categories

## Governance

ใช้กำหนดกฎ มาตรฐาน และวิธีดำเนินงานของโครงการ

| Type | Description |
|------|-------------|
| Standard | มาตรฐานของโครงการ |
| Policy | นโยบาย |
| Guideline | แนวทางปฏิบัติ |
| ADR | Architecture Decision Record |
| Charter | เอกสารจัดตั้งโครงการ |

---

## Enterprise Architecture

ใช้สำหรับออกแบบองค์กร

| Type | Description |
|------|-------------|
| Mission | Mission Domain |
| Capability | Business Capability |
| Organization | Organization Design |
| Process | Business Process |
| Information | Information Model |
| Application | Application Architecture |
| Data | Data Architecture |

---

## Regulatory

| Type | Description |
|------|-------------|
| Regulation | กฎหมายและข้อบังคับ |
| Requirement | ข้อกำหนด |
| Compliance | Compliance Matrix |
| Reference | เอกสารอ้างอิง |

---

## Operational Documentation

| Type | Description |
|------|-------------|
| Manual | คู่มือ |
| SOP | Standard Operating Procedure |
| Work Instruction | วิธีปฏิบัติงาน |
| Checklist | Checklist |
| Form | แบบฟอร์ม |
| Template | Template |

---

## Project Management

| Type | Description |
|------|-------------|
| Working Session | บันทึกการทำงาน |
| Checkpoint | Baseline |
| Release | Release Note |
| Roadmap | Roadmap |
| Risk | Risk Register |
| Issue | Issue Register |
| Decision | Decision Log |

---

# Naming Rule

หนึ่งไฟล์สามารถมีได้เพียง Document Type เดียว

---

# Future Expansion

Document Types สามารถเพิ่มเติมได้ผ่าน ADR เท่านั้น