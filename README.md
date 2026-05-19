# DLP Implement Assessment — Static Web

แบบสอบถามสำหรับการทำ **Workshop / Presales / Scoping / SOW Input** สำหรับการ Implement Microsoft Purview DLP (Data Loss Prevention)

**Live Site:** https://dekbacom.github.io/DLP-Implement-Assessment/

---

## Features

| Feature | Description |
|---|---|
| 10 Assessment Sections | ครอบคลุมตั้งแต่ Project Scope จนถึง Rollout & Adoption |
| Industry Recommendation | คำแนะนำ baseline ตามประเภทอุตสาหกรรม |
| Search & Filter | ค้นหาคำถาม / กรอง Done / Open |
| Export CSV | ดาวน์โหลด .csv สำหรับ Excel / Google Sheets |
| Export JSON | ดาวน์โหลด .json สำหรับนำไปประมวลผลต่อ |
| Export PDF | สร้าง PDF report ผ่าน browser Print dialog |
| Auto-save | บันทึกอัตโนมัติลง localStorage ทุก keystroke |
| วิธีใช้งาน | คู่มือการใช้งานภาษาไทย (กดปุ่ม "วิธีใช้งาน" ในหน้าเว็บ) |

---

## Assessment Sections

1. Project Scope & Objective
2. Current Environment & Licensing
3. Data Classification & Sensitive Information
4. User Groups, Departments & Policy Targeting
5. DLP Use Cases
6. Enforcement Model & Override
7. Alert, Approval & Incident Handling
8. Monitoring, Reporting & Validation
9. Compliance, Audit & Retention
10. Testing, Rollout & Adoption

---

## Industry Recommendations

| Industry | Design Decision | Primary Policy |
|---|---|---|
| Banking & Financial | Enforce - Block | EXO DLP |
| Government | Enforce - Warn | Sensitivity Labels |
| State Enterprise | Enable (Pilot/Test) | SharePoint & OneDrive DLP |
| Manufacturing & Industry | Enable (Baseline) | Endpoint DLP |
| Other Enterprise | Enable (Pilot/Test) | Teams DLP |

---

## How to Deploy (GitHub Pages)

1. Fork or clone this repo
2. Push to GitHub
3. Go to **Settings → Pages → Source: main / (root)**
4. Site goes live at `https://<username>.github.io/<repo-name>/`

No build step or server required — single `index.html` file only.

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript (no frameworks, no build step)
- [Tailwind CSS](https://tailwindcss.com) via CDN
- Browser localStorage for auto-save
- Browser Print API for PDF export

---

## Usage

Each question card has four fields:

| Field | Purpose |
|---|---|
| **Customer Answer** | คำตอบที่ได้จาก customer หรือ workshop |
| **Comments & Notes** | บันทึกเพิ่มเติม ข้อสมมติ ความเสี่ยง |
| **Design Decision** | ผลการตัดสินใจ (เช่น Enforce - Block) |
| **Recommended DLP Policy** | Policy ที่แนะนำสำหรับ use case นี้ |

---

*Prepared by DekBaCom — Microsoft Purview DLP Implementation Assessment Tool*
