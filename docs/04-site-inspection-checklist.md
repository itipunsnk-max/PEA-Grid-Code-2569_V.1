# 04 — Site Inspection & Handover Checklist (25 รายการ)

[← กลับหน้าหลัก](../README.md) · [← Matrix](03-compliance-matrix.md) · [ต่อไป: TOR →](05-tor-specification-templates.md)

> **หมายเหตุด้านการใช้งาน:** เนื้อหานี้เรียบเรียงจาก HTML และภาพสรุปที่แนบมา ไม่ใช่ประกาศหรือหนังสืออนุมัติอย่างเป็นทางการของ กฟภ. ก่อนนำตัวเลข/ข้อกำหนดไปใช้ใน TOR, BOQ, งานออกแบบ หรือยื่นเชื่อมต่อ ให้ตรวจเอกสาร กฟภ. ฉบับเต็มและหนังสืออนุมัติเฉพาะโครงการอีกครั้ง

ใช้ร่วมกับ **Approved SLD, ITP, FAT/SAT, Protection Setting Sheet, As-built Drawing** และข้อกำหนดการทดสอบที่ กฟภ. อนุมัติ

> **GitHub tip:** Checkbox ใน Markdown เหมาะสำหรับเปิดอ่าน/คัดลอกเป็น template; การติ๊ก checkbox บนหน้า README ของ GitHub ไม่ใช่ระบบบันทึกผลตรวจหน้างานโดยอัตโนมัติ หากต้องการจัดการสถานะควรใช้ GitHub Issue หรือไฟล์ที่แก้ไขผ่าน commit

## Design / งานออกแบบ (6 รายการ)

- [ ] **QA-01 — Roof structural**  
  ตรวจ: ตรวจ Dead/Live/Wind load, existing condition, anchor detail ก่อน install  
  หลักฐาน: Signed structural calc, anchor shop drawing  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-02 — Farm civil**  
  ตรวจ: ตรวจ Geotech, pile embedment, Flood level, Drainage, earthwork grading  
  หลักฐาน: Geotech report, foundation drawing  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-03 — PV array**  
  ตรวจ: คำนวณ PV Voc at low temp, Isc, string counts, MPPT range  
  หลักฐาน: DC sizing & MPPT report  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-04 — DC cable**  
  ตรวจ: ตรวจ cable ampacity, derating, UV/weather suitability, voltage drop  
  หลักฐาน: DC cable schedule & datasheets  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-05 — AC cable**  
  ตรวจ: ตรวจ cable ampacity, fault withstand, voltage drop, earth conductor  
  หลักฐาน: AC cable calc + cable schedule  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-06 — Earthing**  
  ตรวจ: ตรวจ earthing, bonding, surge protection & lightning risk  
  หลักฐาน: Earthing SLD, ground resistance report  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code

## Construction / งานติดตั้ง (8 รายการ)

- [ ] **QA-07 — Structure acceptance**  
  ตรวจ: Torque marking, corrosion protection, anchor pull tests ตาม Design  
  หลักฐาน: Torque records, inspection photos  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-08 — Roof waterproofing**  
  ตรวจ: ทดสอบจุดเจาะ/ซีลป้องกันรั่วซึมหลังติดตั้ง  
  หลักฐาน: Water-tightness inspection  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-09 — Cable routing**  
  ตรวจ: แยก AC/DC, metal trays bonding, cable labels, bending radius  
  หลักฐาน: Cable route inspection  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-10 — PV module**  
  ตรวจ: Visual quality, serial no, clamps positions, shade clearance  
  หลักฐาน: Module inspection & register  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-11 — DC polarity**  
  ตรวจ: ตรวจ polarity ก่อนเข้าขั้ว inverter, insulation resistance (ตาม test plan)  
  หลักฐาน: Polarity, insulation test  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-12 — AC termination**  
  ตรวจ: ตรวจขัน terminal torque และอุณหภูมิหลัง load test  
  หลักฐาน: Termination test, thermal image  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-13 — Safety**  
  ตรวจ: LOTO, barriers, live-work and fall protection review  
  หลักฐาน: Method statement, PTW/JSA  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-14 — Equipment labels**  
  ตรวจ: Warning: DC live when irradiated, switching points, fire map  
  หลักฐาน: As-built label plan  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code

## Grid Connection / จุดเชื่อมต่อ (7 รายการ)

- [ ] **QA-15 — PEA interface**  
  ตรวจ: ยืนยัน PCC, SLD, breaker/relay setpoints จาก PEA ก่อน energized  
  หลักฐาน: Approved PEA SLD, relay setting  
  อ้างอิง/สถานะ: C ข้อ 2.3; Annex 7.1
- [ ] **QA-16 — Export limiter**  
  ตรวจ: Test under minimum load/high PV, CT-loss / comms-loss fail-safe  
  หลักฐาน: EXL log and event test  
  อ้างอิง/สถานะ: C ข้อ 2.2.4; 3.3.1
- [ ] **QA-17 — Anti-islanding**  
  ตรวจ: ทดสอบ loss of PEA source within 1s  
  หลักฐาน: Anti-islanding test report  
  อ้างอิง/สถานะ: C ข้อ 2.9.6
- [ ] **QA-18 — Inverter protections**  
  ตรวจ: ตรวจ OV/UV/OF/UF and ride-through setting  
  หลักฐาน: Approved inverter parameter sheet  
  อ้างอิง/สถานะ: C ข้อ 2.9.3-2.9.5
- [ ] **QA-19 — PQ meter**  
  ตรวจ: ทดสอบ Class A/S, UPS 15min, logging 30days  
  หลักฐาน: PQM acceptance report  
  อ้างอิง/สถานะ: C Annex 7.2 ข้อ 4
- [ ] **QA-20 — SCADA**  
  ตรวจ: ทดสอบ remote breaker controls, SOE, data points, setpoints  
  หลักฐาน: SCADA SAT & I/O checklist  
  อ้างอิง/สถานะ: C Annex 7.3
- [ ] **QA-21 — PEA approval to energize**  
  ตรวจ: เก็บหลักฐาน PEA ร่วมตรวจ, ทดสอบ และอนุญาตก่อนเชื่อม  
  หลักฐาน: PEA inspection report  
  อ้างอิง/สถานะ: S ข้อ 3.3.3

## Commissioning / ทดสอบ (2 รายการ)

- [ ] **QA-22 — I-V curve**  
  ตรวจ: เก็บ commissioning baseline ราย string ตามสภาพหน้างาน  
  หลักฐาน: IV curve record  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-23 — Thermal scan**  
  ตรวจ: ถ่าย Infrared ของ Combiner, inverter, AC cabinet ขณะจ่ายกำลัง  
  หลักฐาน: Thermography report  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code

## Handover / ส่งมอบ (2 รายการ)

- [ ] **QA-24 — As-built & O&M**  
  ตรวจ: ส่ง SLD, string map, relay settings, inverter FW, O&M, warranty  
  หลักฐาน: Handover dossier  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code
- [ ] **QA-25 — Training**  
  ตรวจ: อบรม Emergency shutdown, communications, inspection schedule  
  หลักฐาน: Training attendance  
  อ้างอิง/สถานะ: แนวทางวิศวกรรมเพิ่มเติม ไม่ใช่ค่าเกณฑ์ใน Grid Code

## ข้อมูลบันทึกผลตรวจ

| รายการ | ข้อมูลกรอก |
|---|---|
| โครงการ | ................................................ |
| สถานที่ / PCC | ................................................ |
| วันที่ตรวจ | ................................................ |
| ผู้ตรวจ / ผู้รับจ้าง | ................................................ |
| Drawing Revision / SLD | ................................................ |
| รายการค้างแก้ไข (Punch List) | ................................................ |
| สถานะการอนุญาตจาก กฟภ. | ................................................ |

[ดาวน์โหลด Checklist CSV](../data/inspection-checklist.csv) · [กลับหน้าหลัก](../README.md)
