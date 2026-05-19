# DLP Implement Assessment — Static Web

แบบสอบถามออนไลน์สำหรับ **Workshop · Presales · Scoping · SOW Input**  
ใช้ประกอบการ Implement Microsoft Purview DLP (Data Loss Prevention)

**🌐 Live Site:** https://dekbacom.github.io/DLP-Implement-Assessment/

---

## ภาพรวม (Overview)

เครื่องมือนี้ช่วย Consultant / Pre-sales / Security Engineer รวบรวมข้อมูลจากลูกค้าอย่างเป็นระบบก่อนเริ่ม DLP Project ครอบคลุม 10 หมวดหลัก 57 ข้อ พร้อม auto-save และ export หลาย format

---

## ฟีเจอร์ทั้งหมด (Features)

| ฟีเจอร์ | รายละเอียด |
|---|---|
| **10 Assessment Sections** | ครอบคลุมตั้งแต่ Project Scope จนถึง Rollout & Adoption (57 คำถาม) |
| **Industry Recommendation** | คำแนะนำ Design Decision + Policy baseline ตามประเภทอุตสาหกรรม |
| **License Suggestion** | แจ้ง license tier ที่ต้องการ (E3 / E5 / Purview Add-on / Copilot) แบบ real-time ตามฟีเจอร์ที่เลือก |
| **Search & Filter** | ค้นหาคำถามด้วย keyword · กรอง All / Done / Open |
| **Export CSV** | ดาวน์โหลด .csv สำหรับ Excel / Google Sheets (พร้อม BOM ภาษาไทย) |
| **Export JSON** | ดาวน์โหลด .json สำหรับนำไปประมวลผลหรือ import กลับ |
| **Export PDF** | สร้าง A4 report พร้อมข้อมูลครบทุก section ผ่าน browser Print dialog |
| **Auto-save** | บันทึกอัตโนมัติลง localStorage ทุก keystroke — ไม่ต้องกด Save |
| **วิธีใช้งาน** | คู่มือการใช้งาน 8 ขั้นตอนเป็นภาษาไทย (กดปุ่ม "วิธีใช้งาน" ในหน้าเว็บ) |

---

## หมวดคำถาม (Assessment Sections)

| # | Section | จำนวนคำถาม |
|---|---|---|
| 1 | Project Scope & Objective | 5 |
| 2 | Current Environment & Licensing | 6 |
| 3 | Data Classification & Sensitive Information | 8 |
| 4 | User Groups, Departments & Policy Targeting | 5 |
| 5 | DLP Use Cases | 9 |
| 6 | Enforcement Model & Override | 5 |
| 7 | Alert, Approval & Incident Handling | 6 |
| 8 | Monitoring, Reporting & Validation | 6 |
| 9 | Compliance, Audit & Retention | 5 |
| 10 | Testing, Rollout & Adoption | 7 |

---

## License Suggestion Logic

ระบบตรวจจับ license tier อัตโนมัติจากคำตอบที่กรอก:

| ฟีเจอร์ที่เลือก | License ที่ต้องการ |
|---|---|
| Endpoint DLP (Windows / macOS) | M365 E5 หรือ Purview Add-on |
| Exact Data Match (EDM) | M365 E5 หรือ Purview Add-on |
| Auto-labeling (Advanced) | M365 E5 หรือ Purview Add-on |
| Activity Explorer & Data Explorer | M365 E5 หรือ Purview Add-on |
| Approval Workflow | M365 E5 หรือ Purview Add-on |
| Microsoft 365 Copilot DLP | M365 Copilot Add-on |
| ไม่มีฟีเจอร์พิเศษ | ✅ M365 E3 เพียงพอ |

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

## วิธีใช้งาน (How to Use)

1. **กรอก Metadata** — Customer Name, Industry, Next Step, Date, Prepared By
2. **ตอบคำถาม** — Customer Answer + Comments + Design Decision + Recommended Policy
3. **ดู License Suggestion** — การ์ดอัพเดต real-time ตามฟีเจอร์ที่เลือก
4. **Apply Industry Rec.** — เติม Decision & Policy ตาม industry อัตโนมัติ (ไม่ทับค่าที่กรอกแล้ว)
5. **Search & Filter** — ค้นหา / กรอง Done / Open เพื่อโฟกัสคำถามที่ยังเหลือ
6. **Export** — CSV (Excel) · JSON (re-import) · PDF (รายงาน A4)
7. **Auto-save** — บันทึกอัตโนมัติ ไม่ต้องกด Save
8. **Reset** — ล้างทั้งหมดเมื่อต้องการเริ่มใหม่

> กดปุ่ม **"วิธีใช้งาน"** (สีฟ้า) ในหน้าเว็บเพื่อดูคู่มือฉบับเต็ม

---

## วิธี Deploy (GitHub Pages)

1. Fork หรือ Clone repo นี้
2. Push ขึ้น GitHub
3. ไปที่ **Settings → Pages → Source: main / (root)**
4. Site จะ live ที่ `https://<username>.github.io/<repo-name>/`

ไม่ต้องติดตั้ง Node.js หรือ build — ใช้ไฟล์ `index.html` ไฟล์เดียว

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript (ไม่ใช้ framework ไม่มี build step)
- [Tailwind CSS](https://tailwindcss.com) via CDN
- Browser localStorage สำหรับ auto-save
- Browser Print API สำหรับ Export PDF

---

## ผู้พัฒนา (Contributor)

**Mr. Abdulloh Etaeluengoh**  
📧 Abdulloh.eg@gmail.com

---

*Microsoft Purview DLP Implementation Assessment Tool — v1.0*
