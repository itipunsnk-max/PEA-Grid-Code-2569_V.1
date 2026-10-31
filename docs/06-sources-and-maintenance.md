# 06 — แหล่งอ้างอิง ข้อจำกัด และการดูแลคู่มือ GitHub

[← กลับหน้าหลัก](../README.md)

## 1. ไฟล์ที่ใช้จัดทำคู่มือฉบับนี้

- **HTML แนบ:** [`source/PEA_Grid_Code_2569_Solar_Engineering_Guide.html`](../source/PEA_Grid_Code_2569_Solar_Engineering_Guide.html) — มีข้อมูลตาราง Engineering Matrix, Thresholds, Scenario, Checklist และ TOR อยู่ในไฟล์เดียว
- **ภาพที่ 1:** [`images/01-pea-grid-code-2569-overview.png`](../images/01-pea-grid-code-2569-overview.png) — สรุป Grid Code / ความแตกต่างระหว่างฉบับเก่าและใหม่
- **ภาพที่ 2:** [`images/02-pea-solar-pv-connection-patterns.png`](../images/02-pea-solar-pv-connection-patterns.png) — สรุปรูปแบบ Solar PV และอุปกรณ์ประกอบ

**ข้อเท็จจริงเกี่ยวกับการตรวจต้นทาง:** งานนี้นำข้อมูลจาก **HTML + PNG ทั้งสองภาพที่แนบในคำขอนี้** มาจัดรูปแบบใหม่ ไม่ได้มีไฟล์ PDF ประกาศ กฟภ. 4 ฉบับต้นทางเพื่อยืนยันข้อความและเลขข้อในแต่ละรายการโดยตรง และไม่ได้ทำการรับรองความถูกต้องทางกฎหมาย/วิศวกรรมของต้นฉบับ

## 2. ชื่อเอกสาร PEA ที่ HTML อ้างถึง

1. ประกาศ กฟภ. เรื่อง Grid Code พ.ศ. 2569 (HTML ระบุวันประกาศ 10 กันยายน 2569)
2. **Connection Code (C):** ข้อกำหนดเกี่ยวกับการเชื่อมต่อระบบโครงข่ายไฟฟ้า — ข้อ 2.1–2.11, 3.1–3.3 และ Annex 7.1–7.4
3. **Service Code (S):** ข้อกำหนดเกี่ยวกับการใช้บริการระบบโครงข่ายไฟฟ้า — การขอเชื่อมต่อและทดสอบ
4. **Operation Code (O):** ข้อกำหนดเกี่ยวกับการปฏิบัติการระบบโครงข่ายไฟฟ้า — การควบคุม ทดสอบ และ O&M

เว็บไซต์หน่วยงานสำหรับตรวจประกาศและเอกสารฉบับล่าสุด: [การไฟฟ้าส่วนภูมิภาค (PEA)](https://www.pea.co.th/)

> ไม่ได้แนบลิงก์ PDF รายฉบับ เพราะยังไม่ได้ตรวจสอบ URL ทางการที่เป็นเอกสารฉบับดังกล่าวในงานนี้

## 3. สิ่งที่ไม่ควรใช้คู่มือฉบับนี้แทน

- หนังสืออนุญาตเชื่อมต่อไฟฟ้า / สัญญารับซื้อไฟ / เงื่อนไขอนุญาตเฉพาะโครงการ
- Calculation งานโยธา ฐานราก และหลังคา
- DC String Sizing, Cable Sizing, Cable Routing, Earthing, Lightning และ Fire Safety ซึ่งต้องอ้างมาตรฐานเพิ่มเติม
- Protection Setting หรือ Commissioning Procedure ที่ลงนามอนุมัติ
- เอกสารอ้างอิงทางกฎหมายฉบับเต็ม/ประกาศแก้ไขเพิ่มเติมหลังวันจัดทำไฟล์ต้นทาง

## 4. โครงสร้างโฟลเดอร์สำหรับอัปโหลดเข้า GitHub

```text
PEA-Grid-Code-2569/
├── README.md
├── images/
│   ├── 01-pea-grid-code-2569-overview.png
│   └── 02-pea-solar-pv-connection-patterns.png
├── docs/
│   ├── 01-overview-and-connections.md
│   ├── 02-key-thresholds.md
│   ├── 03-compliance-matrix.md
│   ├── 04-site-inspection-checklist.md
│   ├── 05-tor-specification-templates.md
│   └── 06-sources-and-maintenance.md
├── data/
│   ├── source-data.json
│   ├── compliance-matrix.csv
│   ├── thresholds.csv
│   └── inspection-checklist.csv
└── source/
    └── PEA_Grid_Code_2569_Solar_Engineering_Guide.html
```

## 5. วิธีอัปโหลดขึ้น GitHub

1. สร้าง repository ใหม่บน GitHub เช่น `PEA-Grid-Code-2569` แล้วเปิด repository นั้น
2. เลือก **Add file → Upload files** (หรือใช้ `git add` และ `git push` ผ่าน Git)
3. นำ **ไฟล์และโฟลเดอร์ทั้งหมดที่อยู่ด้านใน `PEA-Grid-Code-2569/`** ลงที่ root ของ repository โดยตรง
4. ตรวจว่ามี `README.md` อยู่ที่ root; GitHub จะเรนเดอร์ README เป็นหน้าแรกอัตโนมัติ
5. ตรวจว่าไฟล์ภาพทั้งสองแสดงใน README; Path จะเริ่มด้วย `images/...`
6. ทดสอบลิงก์ `docs/...` และเปิดอ่าน CSV/HTML ต้นฉบับ

**ถ้าอัปโหลด ZIP โดยตรง:** GitHub จะเก็บเป็นไฟล์ ZIP แต่ **ไม่แตกไฟล์ให้** ต้องแตก ZIP ในเครื่องก่อนเลือก Upload files

## 6. วิธีแก้ไขและต่อยอด

- **แก้หน้าแรกหรือคำอธิบายภาพ:** แก้ `README.md`
- **แก้ตารางเกณฑ์:** แก้ `docs/02-key-thresholds.md` และไฟล์ CSV ที่เกี่ยวข้อง หากต้องการให้ CSV เป็นข้อมูลฉบับเดียวกัน
- **เพิ่ม/แก้ Compliance Matrix:** แก้ `docs/03-compliance-matrix.md` แล้วอัปเดต `data/compliance-matrix.csv` และ `data/source-data.json` ตามความเหมาะสม
- **แก้ Checklist:** แก้ `docs/04-site-inspection-checklist.md`
- **เพิ่มรูปภาพ:** ใส่ไฟล์ใน `images/` แล้วแทรก `![คำอธิบาย](../images/01-pea-grid-code-2569-overview.png)` สำหรับไฟล์ใน `docs/`
- **ติดตามประวัติ:** ใช้ Commit ของ GitHub เพื่อเปรียบเทียบการเปลี่ยนแปลงทีละรอบ และระบุวันที่ตรวจข้อกฎหมายล่าสุดทุกครั้ง

**หมายเหตุ:** HTML ใน `source/` เป็น snapshot ต้นทาง ไม่ได้ซิงก์อัตโนมัติกับ Markdown; GitHub README จะเรนเดอร์ Markdown แต่ไม่รัน JavaScript ใน HTML ต้นฉบับ

## 7. ข้อมูลเวอร์ชัน

| ประเด็น | รายละเอียด |
|---|---|
| ชุด Markdown | 31 ตุลาคม 2569 |
| HTML ต้นทาง | แสดง Rev. 22 ตุลาคม 2569 |
| รูปอินโฟกราฟิก | สองภาพที่ผู้ใช้แนบในคำขอ |
| จำนวนรายการ | Matrix 51; Thresholds 34; QA 25; TOR 6; Scenarios 8 |
| สถานะการตรวจยัน PDF ทางการ | ยังไม่ได้ตรวจยันในงานนี้ |
