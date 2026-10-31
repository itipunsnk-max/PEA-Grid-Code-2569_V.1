# 03 — Engineering Compliance Matrix (51 รายการ)

[← กลับหน้าหลัก](../README.md) · [← ค่าพิกัด](02-key-thresholds.md) · [ต่อไป: Checklist →](04-site-inspection-checklist.md)

> **หมายเหตุด้านการใช้งาน:** เนื้อหานี้เรียบเรียงจาก HTML และภาพสรุปที่แนบมา ไม่ใช่ประกาศหรือหนังสืออนุมัติอย่างเป็นทางการของ กฟภ. ก่อนนำตัวเลข/ข้อกำหนดไปใช้ใน TOR, BOQ, งานออกแบบ หรือยื่นเชื่อมต่อ ให้ตรวจเอกสาร กฟภ. ฉบับเต็มและหนังสืออนุมัติเฉพาะโครงการอีกครั้ง

## วิธีใช้ Matrix

- เลือกงานที่เกี่ยวข้องจาก **Solar Roof / Solar Farm** และอ่าน **เกณฑ์ / Trigger** ทุกครั้งก่อนใส่รายการลง TOR หรือ BOQ
- คอลัมน์ **สิ่งที่ต้องทำ** เป็นแนวทางนำข้อกำหนดไปปฏิบัติและเอกสารที่ควรจัดทำ; อย่าตีความว่าเป็นข้อกฎหมายเพิ่มเติมโดยอัตโนมัติ
- รายการที่ระบุ **แนวทางวิศวกรรมเพิ่มเติม** ไม่ใช่ค่าเกณฑ์โดยตรงจาก Grid Code ใน HTML
- เลขข้อท้ายแต่ละรายการเป็น **Reference ตามไฟล์ต้นทาง** ซึ่งยังไม่ได้ตรวจยันกับ PDF ประกาศฉบับเต็มในงานนี้

## ไปยังช่วงงาน

- [สำรวจและกำหนดประเภท (4 รายการ)](#pre-design)
- [ศึกษาผลกระทบระบบไฟฟ้า (6 รายการ)](#study)
- [ออกแบบและเลือกอุปกรณ์ (29 รายการ)](#design)
- [การปฏิบัติการและ O&M (3 รายการ)](#operation)
- [ขออนุญาตและยื่นเอกสาร (3 รายการ)](#permit)
- [ติดตั้งและตรวจหน้างาน (1 รายการ)](#construction)
- [ทดสอบก่อนเชื่อมต่อ (2 รายการ)](#commissioning)
- [การเปลี่ยนแปลงระบบ (1 รายการ)](#change-control)
- [วิศวกรรมความปลอดภัยเพิ่มเติม (2 รายการ)](#site-safety)

## ดัชนีรายการทั้งหมด

| ID | ช่วงงาน | หัวข้อ | เกณฑ์/Trigger |
| --- | --- | --- | --- |
| [PEA-001](#pea-001) | สำรวจและกำหนดประเภท | วันมีผลบังคับ | ประกาศ 10 ก.ย. 2569; มีผล 10 ธ.ค. 2569 |
| [PEA-002](#pea-002) | สำรวจและกำหนดประเภท | จำแนก IPU / IPS / VSPP / SPP | IPU ผลิตใช้เอง; IPS ผลิตจ่ายผู้ใช้ไฟ; VSPP/SPP ขายไฟตามเงื่อนไข |
| [PEA-003](#pea-003) | สำรวจและกำหนดประเภท | ระบุ PCC และระดับแรงดัน | LV 220/380 V; MV 22/33 kV; HV 115 kV |
| [PEA-004](#pea-004) | สำรวจและกำหนดประเภท | แยกค่ากำลังไฟฟ้า | PV DC kWp / Inverter AC installed / export cap เป็นคนละค่า |
| [PEA-005](#pea-005) | วิเคราะห์ระบบ | กระแสพิกัดสาย/โหลด | ห้ามเกิน continuous ampacity |
| [PEA-006](#pea-006) | วิเคราะห์ระบบ | แรงดัน ณ PCC | ต้องอยู่ในกรอบ PEA voltage standards |
| [PEA-007](#pea-007) | วิเคราะห์ระบบ | Short Circuit headroom | Isc รวม ≤ 85% ของ interrupting capacity ของอุปกรณ์ตัด/ป้องกัน |
| [PEA-008](#pea-008) | วิเคราะห์ระบบ | Protection coordination | ห้ามทำให้รีเลย์/CB ไม่ประสานสัมพันธ์ |
| [PEA-009](#pea-009) | วิเคราะห์ระบบ | ทบทวนข้อจำกัด feeder & substation | 22 kV รวม ≤8 MW/วงจร; 33 kV ≤10 MW/วงจร; รวม ≤75% rating หม้อแปลงสถานี |
| [PEA-010](#pea-010) | วิเคราะห์ระบบ | ทบทวนเพดาน 115 kV | Overhead 115 kV single 120 MW; double 230 MW/วงจร |
| [PEA-011](#pea-011) | ออกแบบ/เลือกอุปกรณ์ | LV Export cap | LV 1 เฟส ≤5 kW/ราย; มากกว่า 1 เฟส ≤10 kW/ราย |
| [PEA-012](#pea-012) | ออกแบบ/เลือกอุปกรณ์ | หม้อแปลงจำหน่าย LV | กำลังจ่ายออกผู้ขอ+ผู้เชื่อมต่อทุกราย ≤25% kVA หม้อแปลง PEA |
| [PEA-013](#pea-013) | ออกแบบ/เลือกอุปกรณ์ | IPU/IPS Zero export | IPU/IPS ต้องไม่จ่ายไฟเข้าสู่ระบบโครงข่าย |
| [PEA-014](#pea-014) | ออกแบบ/เลือกอุปกรณ์ | VSPP export limiting | ห้ามเกินปริมาณที่ได้รับอนุญาต; PEA อาจสั่ง EXL |
| [PEA-015](#pea-015) | ออกแบบ/เลือกอุปกรณ์ | EXL LV trigger พิเศษ | >7 kW installed เพื่อขาย ≤5 kW 1 เฟส; multi-phase เกณฑ์ >10 หรือ >15 kW ตามปริมาณขาย |
| [PEA-016](#pea-016) | ออกแบบ/เลือกอุปกรณ์ | Anti-islanding | Grid ไม่มีไฟต้องแยก; สำหรับ inverter ภายใน 1 วินาที |
| [PEA-017](#pea-017) | ออกแบบ/เลือกอุปกรณ์ | Automatic Reclosing | โดยหลักไม่อนุญาต auto-reclose ของผู้เชื่อมต่อ; PEA พิจารณารายกรณี |
| [PEA-018](#pea-018) | ออกแบบ/เลือกอุปกรณ์ | Relay / CB / OCD | ขั้นต่ำตามรูปแบบใน Annex 7.1; CT/VT protection ตาม Annex 7.2 |
| [PEA-019](#pea-019) | ออกแบบ/เลือกอุปกรณ์ | หม้อแปลง Winding Connection | ต้องสอดคล้องรูปแบบและกำลังผลิต |
| [PEA-020](#pea-020) | ออกแบบ/เลือกอุปกรณ์ | Inverter tested/registered | ทดสอบตาม Annex 7.4 หรืออยู่ในทะเบียนอุปกรณ์ PEA |
| [PEA-021](#pea-021) | ออกแบบ/เลือกอุปกรณ์ | Active power reduction | ต้องลดจาก 100% ไป 0%; ลดได้อย่างน้อยครั้งละ 10% ต่อนาที |
| [PEA-022](#pea-022) | ออกแบบ/เลือกอุปกรณ์ | Power Factor control | 0.90 lagging ถึง 0.90 leading หรือดีกว่า ณ rated active power |
| [PEA-023](#pea-023) | ออกแบบ/เลือกอุปกรณ์ | Volt-Var / Volt-Watt | ต้องรองรับ Q(V), P(V) เริ่มทำงานที่ P≥20% rated |
| [PEA-024](#pea-024) | ออกแบบ/เลือกอุปกรณ์ | Voltage Fault Ride Through | Installed inverter >50 kW และ PCC ≥22 kV |
| [PEA-025](#pea-025) | ออกแบบ/เลือกอุปกรณ์ | Under/over voltage protection | V<50% <0.3s; 50–90% <2s; 110–120% <0.5s; >120% <0.16s |
| [PEA-026](#pea-026) | ออกแบบ/เลือกอุปกรณ์ | Frequency ride-through | Inverter ต้องคงเชื่อมต่อในช่วง 47–52 Hz |
| [PEA-027](#pea-027) | ออกแบบ/เลือกอุปกรณ์ | Frequency response MV | Installed inverter >50 kW และ PCC ≥22 kV |
| [PEA-028](#pea-028) | ปฏิบัติการ/O&M | ช่วง Frequency ใน Operation Code | VSPP 49.60–50.40 Hz; IPU/IPS 49.50–50.50 Hz (ตามเงื่อนไข >50kW MV) |
| [PEA-029](#pea-029) | ออกแบบ/เลือกอุปกรณ์ | PQM ตาม inverter รวม | Inverter installed รวม >250 kW ต้องจัดหา PQM |
| [PEA-030](#pea-030) | ออกแบบ/เลือกอุปกรณ์ | PQM Class A / Class S | >250 kW ถึง 1 MW: IEC 61000-4-30 Class A หรือ S; >1 MW: Class A + 4-7/4-15 |
| [PEA-031](#pea-031) | ออกแบบ/เลือกอุปกรณ์ | Monitoring quality + weather | Installed generation >1 MW ต้อง Monitoring; weather sensor PEA อาจเรียกร้อง |
| [PEA-032](#pea-032) | ออกแบบ/เลือกอุปกรณ์ | Harmonics & Flicker | Harmonics อ้างอิง IEEE 1547; Flicker IEC 61000-3 ที่เกี่ยวข้อง |
| [PEA-033](#pea-033) | ออกแบบ/เลือกอุปกรณ์ | DC injection | กระแส DC injected ≤0.5% rated inverter current |
| [PEA-034](#pea-034) | ออกแบบ/เลือกอุปกรณ์ | Inverter communication | อย่างน้อย Modbus RTU RS485 และ Modbus TCP Wi-Fi/4G-LTE หรือผ่าน Gateway |
| [PEA-035](#pea-035) | ออกแบบ/เลือกอุปกรณ์ | SCADA / RCS trigger | บังคับใน VSPP แบบ 1.3, 1.6 และ SPP รูปแบบ 3; หรือ PEA กำหนด |
| [PEA-036](#pea-036) | ออกแบบ/เลือกอุปกรณ์ | PPC / SCADA setpoints | VSPP >1 MW ต้องรองรับ MW/MVar/PF/Voltage setpoint ผ่าน SCADA ตามข้อ 2.6.2 |
| [PEA-037](#pea-037) | ออกแบบ/เลือกอุปกรณ์ | DNP 3.0 over IP | Remote system: DNP 3.0 over IP with Secure Authentication; FEP อย่างน้อย 6 หรือ PEA กำหนด |
| [PEA-038](#pea-038) | ออกแบบ/เลือกอุปกรณ์ | Voice communication | ≤1 MW อย่างน้อย 1 ช่อง; >1 MW อย่างน้อย 2 ช่อง (หนึ่งช่องวิทยุ) |
| [PEA-039](#pea-039) | ออกแบบ/เลือกอุปกรณ์ | Export / Import metering | Export / Import-Export meter ตามประเภท; Gen-Meter สำหรับ inverter มีข้อยกเว้น |
| [PEA-040](#pea-040) | ออกแบบ/เลือกอุปกรณ์ | Protection CT/VT + UPS | CT protection ≥5P20; VT protection ≥3P; relay backup supply |
| [PEA-041](#pea-041) | ขออนุญาต | ยื่นคำขอเชื่อมต่อ IPU/IPS | PEA แจ้งผลภายใน 45 วันจากเอกสารครบ หรือเวลาที่กำหนด |
| [PEA-042](#pea-042) | ขออนุญาต | ขั้นตอน VSPP / SPP | VSPP ต้องตามกระบวนการรับซื้อ/PPA; SPP ตาม PPA EGAT + เชื่อม PEA |
| [PEA-043](#pea-043) | ขออนุญาต | ค่าใช้จ่ายและขยายเขต | เจ้าของโครงการรับผิดชอบอุปกรณ์ ทดสอบ ปรับปรุงระบบ และค่าใช้จ่ายที่ PEA เรียก |
| [PEA-044](#pea-044) | ติดตั้ง | ติดตั้งตรงตามแบบอนุมัติ | อุปกรณ์/ระบบป้องกันตาม Annex 7.1 และ Grid Parameter Approved |
| [PEA-045](#pea-045) | ทดสอบรับระบบ | ทดสอบ PEA ก่อนเชื่อมต่อ | IPU/IPS: PEA ตรวจหลังแจ้งภายใน 30 วัน; ต้องผ่านก่อนเริ่มเชื่อมต่อ |
| [PEA-046](#pea-046) | ทดสอบรับระบบ | ทดสอบ relay/controls | Protection/ EXL / anti-islanding / P,Q,f,V / SCADA ตามแบบและประเภท |
| [PEA-047](#pea-047) | ปฏิบัติการ/O&M | Operation coordination | PCC ≥22 kV: ปฏิบัติตามข้อ 2.7.3-2.7.6 และประสานศูนย์ควบคุม |
| [PEA-048](#pea-048) | ปฏิบัติการ/O&M | ตรวจระบบป้องกัน/คุณภาพไฟ | IPU/IPS เชื่อม ≥22 kV: audit PQ/protection/remote ทุก 3 ปีหรือตาม PEA |
| [PEA-049](#pea-049) | แก้ไขเปลี่ยนแปลง | เพิ่มแผง / เพิ่ม inverter / เปลี่ยนพิกัด | เพิ่มเติม/เปลี่ยนอุปกรณ์หรือไฟฟ้าจ่ายออก ต้องส่งรายละเอียดก่อนดำเนินการ ≥90 วัน |
| [PEA-050](#pea-050) | งานความปลอดภัย | โครงสร้างหลังคา/ฐานราก | ไม่มีตัวเลข Structural loading ใน Grid Code ทั้ง 4 ฉบับ |
| [PEA-051](#pea-051) | งานความปลอดภัย | DC design / Lightning / Fire | ไม่มีเกณฑ์ DC cable sizing, fire access, rooftop walkway ใน Grid Code นี้ |

<a id="pre-design"></a>

## สำรวจและกำหนดประเภท (Pre-design)

<a id="pea-001"></a>

### PEA-001 · วันมีผลบังคับ

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ประกาศ 10 ก.ย. 2569; มีผล 10 ธ.ค. 2569  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจวันยื่นและวันอนุมัติโครงการ รวมถึงบทเฉพาะกาลก่อนนำไปอ้างเป็นข้อกำหนดบังคับ  
- **หลักฐาน / Deliverable:** หนังสือตรวจสอบกฎที่ใช้กับโครงการ  
- **ประเภทข้อสรุป:** เงื่อนไขก่อนใช้  
- **อ้างอิง:** `ประกาศ 10 ก.ย. 2569; C ข้อ 6; O ข้อ 6`

<a id="pea-002"></a>

### PEA-002 · จำแนก IPU / IPS / VSPP / SPP

- **ใช้กับ Solar Rooftop:** หลัก  
- **ใช้กับ Solar Farm:** หลัก  
- **เงื่อนไข / Trigger:** IPU ผลิตใช้เอง; IPS ผลิตจ่ายผู้ใช้ไฟ; VSPP/SPP ขายไฟตามเงื่อนไข  
- **สิ่งที่วิศวกรต้องทำ:** ระบุเจ้าของระบบ/ผู้ใช้/ผู้ขาย และสถานะสัญญา; ห้ามใช้เพดานขายไฟเป็นเพดาน kWp สำหรับ IPU  
- **หลักฐาน / Deliverable:** Project Basis + SLD + PPA (ถ้ามี)  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 1.3, 3.1-3.3; S ข้อ 1.3, 3.1-3.3`

<a id="pea-003"></a>

### PEA-003 · ระบุ PCC และระดับแรงดัน

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** LV 220/380 V; MV 22/33 kV; HV 115 kV  
- **สิ่งที่วิศวกรต้องทำ:** จัดทำ SLD กำหนดจุดเชื่อมต่อ, Meter, PCC, หม้อแปลง และขอบเขตผู้รับผิดชอบตาม Annex 7.1  
- **หลักฐาน / Deliverable:** SLD และแบบจุดเชื่อมต่อ กฟภ. รับรอง  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.3.1-2.3.3 และ Annex 7.1`

<a id="pea-004"></a>

### PEA-004 · แยกค่ากำลังไฟฟ้า

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** PV DC kWp / Inverter AC installed / export cap เป็นคนละค่า  
- **สิ่งที่วิศวกรต้องทำ:** จัดทำ Power Balance และ Max Export ณ PCC; ใช้ค่าที่ได้รับอนุญาตสำหรับการส่งเข้ากริด  
- **หลักฐาน / Deliverable:** Load profile, Power Balance, Export cap  
- **ประเภทข้อสรุป:** คำอธิบายเชิงวิศวกรรม  
- **อ้างอิง:** `C ข้อ 2.2, 2.2.4, 3.1.1, 3.3.1`

<a id="study"></a>

## ศึกษาผลกระทบระบบไฟฟ้า (Study)

<a id="pea-005"></a>

### PEA-005 · กระแสพิกัดสาย/โหลด

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ห้ามเกิน continuous ampacity  
- **สิ่งที่วิศวกรต้องทำ:** ศึกษา Load Flow + reverse power + conductor/transformer thermal loading  
- **หลักฐาน / Deliverable:** Load flow, Cable sizing, transformer check  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.1.1(1)`

<a id="pea-006"></a>

### PEA-006 · แรงดัน ณ PCC

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ต้องอยู่ในกรอบ PEA voltage standards  
- **สิ่งที่วิศวกรต้องทำ:** ศึกษา voltage rise/drop และ voltage regulation ที่สภาวะโหลดต่ำและ PV สูง  
- **หลักฐาน / Deliverable:** Voltage study; voltage regulation  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.1.1(2), 2.4.1`

<a id="pea-007"></a>

### PEA-007 · Short Circuit headroom

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** Isc รวม ≤ 85% ของ interrupting capacity ของอุปกรณ์ตัด/ป้องกัน  
- **สิ่งที่วิศวกรต้องทำ:** คำนวณ fault level ก่อน/หลัง PV และตรวจ CB interrupting rating  
- **หลักฐาน / Deliverable:** Short circuit study + equipment ratings  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.1.1(3)`

<a id="pea-008"></a>

### PEA-008 · Protection coordination

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ห้ามทำให้รีเลย์/CB ไม่ประสานสัมพันธ์  
- **สิ่งที่วิศวกรต้องทำ:** จัดทำ relay coordination และ Trip Matrix กับจุดเชื่อมต่อ/สถานี  
- **หลักฐาน / Deliverable:** TCC, protection study, relay settings  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.1.1(3), 2.3.7, 2.3.14`

<a id="pea-009"></a>

### PEA-009 · ทบทวนข้อจำกัด feeder & substation

- **ใช้กับ Solar Rooftop:** ถ้ามีส่งออก  
- **ใช้กับ Solar Farm:** หลัก  
- **เงื่อนไข / Trigger:** 22 kV รวม ≤8 MW/วงจร; 33 kV ≤10 MW/วงจร; รวม ≤75% rating หม้อแปลงสถานี  
- **สิ่งที่วิศวกรต้องทำ:** ใช้เป็น screening ระดับโครงข่าย (รวมผู้เชื่อมต่อทุกราย) ไม่ใช่สิทธิรายโครงการ  
- **หลักฐาน / Deliverable:** Feeder hosting capacity confirmation  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.2.2`

<a id="pea-010"></a>

### PEA-010 · ทบทวนเพดาน 115 kV

- **ใช้กับ Solar Rooftop:** ถ้าเกี่ยวข้อง  
- **ใช้กับ Solar Farm:** ถ้าเกี่ยวข้อง  
- **เงื่อนไข / Trigger:** Overhead 115 kV single 120 MW; double 230 MW/วงจร  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจกรณี underground cable/ข้อจำกัดอื่นที่ PEA อาจลดเกณฑ์  
- **หลักฐาน / Deliverable:** Grid study confirmation  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.2.3`

<a id="design"></a>

## ออกแบบและเลือกอุปกรณ์ (Design)

<a id="pea-011"></a>

### PEA-011 · LV Export cap

- **ใช้กับ Solar Rooftop:** เฉพาะขาย/ส่งออก  
- **ใช้กับ Solar Farm:** เฉพาะขาย/ส่งออก  
- **เงื่อนไข / Trigger:** LV 1 เฟส ≤5 kW/ราย; มากกว่า 1 เฟส ≤10 kW/ราย  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจเฟสและขนาดกำลังส่งออก; multi-phase ความต่างกำลังผลิตติดตั้งแต่ละเฟสสูงสุด 5 kW  
- **หลักฐาน / Deliverable:** SLD, phase balancing, export cap  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.2.1(1)-(2)`

<a id="pea-012"></a>

### PEA-012 · หม้อแปลงจำหน่าย LV

- **ใช้กับ Solar Rooftop:** เฉพาะขาย/ส่งออก  
- **ใช้กับ Solar Farm:** เฉพาะขาย/ส่งออก  
- **เงื่อนไข / Trigger:** กำลังจ่ายออกผู้ขอ+ผู้เชื่อมต่อทุกราย ≤25% kVA หม้อแปลง PEA  
- **สิ่งที่วิศวกรต้องทำ:** ขอข้อมูลกำลังรวมรายอื่น; ใช้กับปริมาณส่งออกไม่ใช่ PV DC capacity  
- **หลักฐาน / Deliverable:** PEA transformer hosting confirmation  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.2.1(3)`

<a id="pea-013"></a>

### PEA-013 · IPU/IPS Zero export

- **ใช้กับ Solar Rooftop:** สำคัญมาก  
- **ใช้กับ Solar Farm:** สำคัญมาก  
- **เงื่อนไข / Trigger:** IPU/IPS ต้องไม่จ่ายไฟเข้าสู่ระบบโครงข่าย  
- **สิ่งที่วิศวกรต้องทำ:** ออกแบบ EXL และ/หรือ Reverse Power Relay ANSI 32 ตาม Annex 7.1; ตรวจ CT polarity และ fail-safe  
- **หลักฐาน / Deliverable:** EXL logic, SLD, CT position, test record  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 3.3.1(2); Annex 7.1 รูปแบบ 2.1-2.4`

<a id="pea-014"></a>

### PEA-014 · VSPP export limiting

- **ใช้กับ Solar Rooftop:** ขาย/ส่งออก  
- **ใช้กับ Solar Farm:** ขาย/ส่งออก  
- **เงื่อนไข / Trigger:** ห้ามเกินปริมาณที่ได้รับอนุญาต; PEA อาจสั่ง EXL  
- **สิ่งที่วิศวกรต้องทำ:** ระบุ export cap และทดสอบ command, saturation, loss of CT/comms  
- **หลักฐาน / Deliverable:** EXL FAT/SAT & commissioning report  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.2.4, 3.1.1(3)`

<a id="pea-015"></a>

### PEA-015 · EXL LV trigger พิเศษ

- **ใช้กับ Solar Rooftop:** VSPP LV  
- **ใช้กับ Solar Farm:** ไม่ค่อยพบ  
- **เงื่อนไข / Trigger:** >7 kW installed เพื่อขาย ≤5 kW 1 เฟส; multi-phase เกณฑ์ >10 หรือ >15 kW ตามปริมาณขาย  
- **สิ่งที่วิศวกรต้องทำ:** ใช้รายละเอียดตามข้อ 2.2.1(4) และ Annex 7.1; อย่าเหมารวมทุกระบบเกิน 5/10 kWp ต้องติด EXL  
- **หลักฐาน / Deliverable:** Installed inverter sizing; export cap  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.2.1(4); Annex 7.1 รูปแบบ 1.1`

<a id="pea-016"></a>

### PEA-016 · Anti-islanding

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** Grid ไม่มีไฟต้องแยก; สำหรับ inverter ภายใน 1 วินาที  
- **สิ่งที่วิศวกรต้องทำ:** รับรอง function inverter + interface tripping; ไม่ให้เกิด unintentional islanding  
- **หลักฐาน / Deliverable:** Protection schematic + anti-islanding test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.3.6, 2.9.6`

<a id="pea-017"></a>

### PEA-017 · Automatic Reclosing

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** โดยหลักไม่อนุญาต auto-reclose ของผู้เชื่อมต่อ; PEA พิจารณารายกรณี  
- **สิ่งที่วิศวกรต้องทำ:** อุปกรณ์ผู้ผลิตปลดก่อน utility reclosing; ไม่ตั้ง auto reclose ของ PCC CB โดยพลการ  
- **หลักฐาน / Deliverable:** Interlocking, reclose coordination  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.3.4-2.3.5`

<a id="pea-018"></a>

### PEA-018 · Relay / CB / OCD

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ขั้นต่ำตามรูปแบบใน Annex 7.1; CT/VT protection ตาม Annex 7.2  
- **สิ่งที่วิศวกรต้องทำ:** เลือกรูปแบบ 1.1–1.6/2.1–2.9/3 ก่อนสรุป BOQ/Relay ANSI functions  
- **หลักฐาน / Deliverable:** Relay list, CB schedule, SLD, schematics  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.3.1, 3.1.1, 3.3.1, Annex 7.1-7.2`

<a id="pea-019"></a>

### PEA-019 · หม้อแปลง Winding Connection

- **ใช้กับ Solar Rooftop:** กรณีมีหม้อแปลง  
- **ใช้กับ Solar Farm:** กรณีมีหม้อแปลง  
- **เงื่อนไข / Trigger:** ต้องสอดคล้องรูปแบบและกำลังผลิต  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจ vector group และ protection/grounding ตามแบบ 7.1; แตกต่างจากแบบต้องขอ PEA เห็นชอบ  
- **หลักฐาน / Deliverable:** Transformer datasheet & SLD  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.3.3; Annex 7.1`

<a id="pea-020"></a>

### PEA-020 · Inverter tested/registered

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ทดสอบตาม Annex 7.4 หรืออยู่ในทะเบียนอุปกรณ์ PEA  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจรุ่น FW และ certificate; ตั้ง grid parameters ตามประเภทการเชื่อมต่อ  
- **หลักฐาน / Deliverable:** PEA registration/test proof; setting sheet  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9, Annex 7.4`

<a id="pea-021"></a>

### PEA-021 · Active power reduction

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ต้องลดจาก 100% ไป 0%; ลดได้อย่างน้อยครั้งละ 10% ต่อนาที  
- **สิ่งที่วิศวกรต้องทำ:** ออกแบบ PPC/inverter command point และบันทึกผล ramp-down  
- **หลักฐาน / Deliverable:** Controller functional test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.1`

<a id="pea-022"></a>

### PEA-022 · Power Factor control

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** 0.90 lagging ถึง 0.90 leading หรือดีกว่า ณ rated active power  
- **สิ่งที่วิศวกรต้องทำ:** ยืนยัน inverter kVA capability ที่ P rated; ทดสอบ constant PF  
- **หลักฐาน / Deliverable:** Capability curve, PF test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.2(1)`

<a id="pea-023"></a>

### PEA-023 · Volt-Var / Volt-Watt

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ต้องรองรับ Q(V), P(V) เริ่มทำงานที่ P≥20% rated  
- **สิ่งที่วิศวกรต้องทำ:** โหลด Q(V) และ P(V) characteristic ตามรูป 3-4 และสอบค่ากับ PEA ก่อน energize  
- **หลักฐาน / Deliverable:** Control settings & Q(V)/P(V) test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.2(2), รูป 3-4`

<a id="pea-024"></a>

### PEA-024 · Voltage Fault Ride Through

- **ใช้กับ Solar Rooftop:** เฉพาะตาม trigger  
- **ใช้กับ Solar Farm:** หลัก  
- **เงื่อนไข / Trigger:** Installed inverter >50 kW และ PCC ≥22 kV  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจ VFRT curve รูป 5; ระหว่าง V 0–90% ต้องจ่าย reactive current ทันทีตามความสามารถ  
- **หลักฐาน / Deliverable:** VFRT compliance certificate/test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.3 รูป 5`

<a id="pea-025"></a>

### PEA-025 · Under/over voltage protection

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** V<50% <0.3s; 50–90% <2s; 110–120% <0.5s; >120% <0.16s  
- **สิ่งที่วิศวกรต้องทำ:** ทำงานร่วมกับ VFRT; ยึด Grid Parameter PEA อนุมัติ ไม่ hardcode โดยไม่ตรวจสอบ  
- **หลักฐาน / Deliverable:** Voltage trip test + setting approval  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.4`

<a id="pea-026"></a>

### PEA-026 · Frequency ride-through

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** Inverter ต้องคงเชื่อมต่อในช่วง 47–52 Hz  
- **สิ่งที่วิศวกรต้องทำ:** ทดสอบ/ตรวจ certificate; นอกช่วงตามข้อกำหนดจึงพิจารณาปลด  
- **หลักฐาน / Deliverable:** FRT certificate, functional test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.5.2, 2.9.5; O ข้อ 2.8.1`

<a id="pea-027"></a>

### PEA-027 · Frequency response MV

- **ใช้กับ Solar Rooftop:** ถ้าเข้า trigger  
- **ใช้กับ Solar Farm:** หลัก  
- **เงื่อนไข / Trigger:** Installed inverter >50 kW และ PCC ≥22 kV  
- **สิ่งที่วิศวกรต้องทำ:** Connection: deadband 50±0.3 Hz และ droop 4% (หรือ 50%/Hz) ตามประเภท  
- **หลักฐาน / Deliverable:** Droop curve, freq settings test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.5, 3.1.3, 3.3.3 [ข้อ 3.3.3 ในไฟล์พิมพ์เป็น 3.1.3]`

<a id="pea-029"></a>

### PEA-029 · PQM ตาม inverter รวม

- **ใช้กับ Solar Rooftop:** ถ้า >250 kW  
- **ใช้กับ Solar Farm:** ถ้า >250 kW  
- **เงื่อนไข / Trigger:** Inverter installed รวม >250 kW ต้องจัดหา PQM  
- **สิ่งที่วิศวกรต้องทำ:** ติดตั้งวัดที่ PCC หรือจุดตามแบบ; ตรวจทุก inverter ตามรูปแบบ  
- **หลักฐาน / Deliverable:** PQM schematic + CT/VT plan  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.4.4, Annex 7.1, 7.2 ข้อ 4`

<a id="pea-030"></a>

### PEA-030 · PQM Class A / Class S

- **ใช้กับ Solar Rooftop:** เมื่อบังคับ PQM  
- **ใช้กับ Solar Farm:** เมื่อบังคับ PQM  
- **เงื่อนไข / Trigger:** >250 kW ถึง 1 MW: IEC 61000-4-30 Class A หรือ S; >1 MW: Class A + 4-7/4-15  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจ memory 30 วัน, 10-min profiles, harmonics ถึง 50th, sampling event ≥128/cycle, UPS ≥15 นาที  
- **หลักฐาน / Deliverable:** PQM technical data + FAT + Test Report  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C Annex 7.2 ข้อ 4.1-4.6`

<a id="pea-031"></a>

### PEA-031 · Monitoring quality + weather

- **ใช้กับ Solar Rooftop:** ถ้า >1 MW  
- **ใช้กับ Solar Farm:** ถ้า >1 MW  
- **เงื่อนไข / Trigger:** Installed generation >1 MW ต้อง Monitoring; weather sensor PEA อาจเรียกร้อง  
- **สิ่งที่วิศวกรต้องทำ:** เก็บ V,I,f,P,Q,PF,THDv,THDi,Pst,Plt; real-time access และ weather ตาม PEA กำหนด  
- **หลักฐาน / Deliverable:** Monitoring tag list; IT network diagram  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.4.4`

<a id="pea-032"></a>

### PEA-032 · Harmonics & Flicker

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** Harmonics อ้างอิง IEEE 1547; Flicker IEC 61000-3 ที่เกี่ยวข้อง  
- **สิ่งที่วิศวกรต้องทำ:** วิเคราะห์/วัดที่ PCC โดยใช้ค่าจำกัดฉบับที่ PEA ยอมรับ; ไม่สมมติ THDi=5% เป็นเกณฑ์ Grid Code นี้  
- **หลักฐาน / Deliverable:** Power quality study & test  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.4.2-2.4.3, 2.9.8-2.9.9`

<a id="pea-033"></a>

### PEA-033 · DC injection

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** กระแส DC injected ≤0.5% rated inverter current  
- **สิ่งที่วิศวกรต้องทำ:** ขอ test/certificate แล้วทดสอบตามที่ PEA กำหนด  
- **หลักฐาน / Deliverable:** Type test certificate  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.10`

<a id="pea-034"></a>

### PEA-034 · Inverter communication

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** อย่างน้อย Modbus RTU RS485 และ Modbus TCP Wi-Fi/4G-LTE หรือผ่าน Gateway  
- **สิ่งที่วิศวกรต้องทำ:** ทวนหมายเลข protocol/address, fail-safe, data points ก่อนสั่งของ  
- **หลักฐาน / Deliverable:** Communication schematic & data map  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.9.12`

<a id="pea-035"></a>

### PEA-035 · SCADA / RCS trigger

- **ใช้กับ Solar Rooftop:** ตามแบบ  
- **ใช้กับ Solar Farm:** ตามแบบ  
- **เงื่อนไข / Trigger:** บังคับใน VSPP แบบ 1.3, 1.6 และ SPP รูปแบบ 3; หรือ PEA กำหนด  
- **สิ่งที่วิศวกรต้องทำ:** เผื่ออุปกรณ์ FRTU/RCS, Router, Utility SCADA test, monthly comms costs  
- **หลักฐาน / Deliverable:** SCADA I/O, drawings, communications plan  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.6.1, Annex 7.1, 7.3`

<a id="pea-036"></a>

### PEA-036 · PPC / SCADA setpoints

- **ใช้กับ Solar Rooftop:** ถ้า VSPP >1 MW  
- **ใช้กับ Solar Farm:** กรณีที่ PEA สั่ง  
- **เงื่อนไข / Trigger:** VSPP >1 MW ต้องรองรับ MW/MVar/PF/Voltage setpoint ผ่าน SCADA ตามข้อ 2.6.2  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจ logic setpoint to inverter group, feedback and control response at PCC  
- **หลักฐาน / Deliverable:** PPC functional test & SCADA SAT  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.6.2, Annex 7.3`

<a id="pea-037"></a>

### PEA-037 · DNP 3.0 over IP

- **ใช้กับ Solar Rooftop:** เฉพาะมี SCADA  
- **ใช้กับ Solar Farm:** เฉพาะมี SCADA  
- **เงื่อนไข / Trigger:** Remote system: DNP 3.0 over IP with Secure Authentication; FEP อย่างน้อย 6 หรือ PEA กำหนด  
- **สิ่งที่วิศวกรต้องทำ:** ทำ I/O list, SOE ≤1ms, analog error ≤0.2%FS (รวม CT/PT ≤1%), SCBO ตามแบบ  
- **หลักฐาน / Deliverable:** Protocol implementation, point list, SCADA SAT  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C Annex 7.3 ข้อ 1.2-1.4`

<a id="pea-038"></a>

### PEA-038 · Voice communication

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** ≤1 MW อย่างน้อย 1 ช่อง; >1 MW อย่างน้อย 2 ช่อง (หนึ่งช่องวิทยุ)  
- **สิ่งที่วิศวกรต้องทำ:** ระบุผู้ประสานงานเบอร์ฉุกเฉิน วิทยุ/โทรศัพท์ตามที่ PEA กำหนด  
- **หลักฐาน / Deliverable:** Communications plan  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.7`

<a id="pea-039"></a>

### PEA-039 · Export / Import metering

- **ใช้กับ Solar Rooftop:** VSPP ขายไฟ  
- **ใช้กับ Solar Farm:** VSPP/SPP ขายไฟ  
- **เงื่อนไข / Trigger:** Export / Import-Export meter ตามประเภท; Gen-Meter สำหรับ inverter มีข้อยกเว้น  
- **สิ่งที่วิศวกรต้องทำ:** ให้ PEA อนุมัติ meter location, CT/VT circuits, ownership ก่อนสั่งอุปกรณ์  
- **หลักฐาน / Deliverable:** Metering diagram + approval  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 3.1.2, 3.2.2, 3.3.2`

<a id="pea-040"></a>

### PEA-040 · Protection CT/VT + UPS

- **ใช้กับ Solar Rooftop:** กรณีใช้รีเลย์ MV  
- **ใช้กับ Solar Farm:** กรณีใช้รีเลย์ MV  
- **เงื่อนไข / Trigger:** CT protection ≥5P20; VT protection ≥3P; relay backup supply  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจ CT burden/saturation และสำรองไฟ relay ตาม Annex 7.2  
- **หลักฐาน / Deliverable:** CT/VT datasheet, UPS schedule  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C Annex 7.2 ข้อ 2`

<a id="operation"></a>

## การปฏิบัติการและ O&M (Operation)

<a id="pea-028"></a>

### PEA-028 · ช่วง Frequency ใน Operation Code

- **ใช้กับ Solar Rooftop:** ถ้าเข้า trigger  
- **ใช้กับ Solar Farm:** หลัก  
- **เงื่อนไข / Trigger:** VSPP 49.60–50.40 Hz; IPU/IPS 49.50–50.50 Hz (ตามเงื่อนไข >50kW MV)  
- **สิ่งที่วิศวกรต้องทำ:** อย่าสับสนกับ deadband 50±0.3 ใน Connection Code; ให้ PEA อนุมัติ setting sheet ร่วม  
- **หลักฐาน / Deliverable:** PEA-approved frequency curve & control logic  
- **ประเภทข้อสรุป:** ต้องยืนยันค่าตั้ง  
- **อ้างอิง:** `O ข้อ 3.1.2.2, 3.3.2.2; C ข้อ 2.9.5`

<a id="pea-047"></a>

### PEA-047 · Operation coordination

- **ใช้กับ Solar Rooftop:** โดยเฉพาะ MV  
- **ใช้กับ Solar Farm:** หลัก  
- **เงื่อนไข / Trigger:** PCC ≥22 kV: ปฏิบัติตามข้อ 2.7.3-2.7.6 และประสานศูนย์ควบคุม  
- **สิ่งที่วิศวกรต้องทำ:** เตรียม switching program, PTW, incident reporting (บางกรณี 3 วัน)  
- **หลักฐาน / Deliverable:** Operation manual + contact list  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `O ข้อ 2.5-2.7`

<a id="pea-048"></a>

### PEA-048 · ตรวจระบบป้องกัน/คุณภาพไฟ

- **ใช้กับ Solar Rooftop:** ตามเกณฑ์  
- **ใช้กับ Solar Farm:** ตามเกณฑ์  
- **เงื่อนไข / Trigger:** IPU/IPS เชื่อม ≥22 kV: audit PQ/protection/remote ทุก 3 ปีหรือตาม PEA  
- **สิ่งที่วิศวกรต้องทำ:** แจ้ง PEA ร่วมตรวจล่วงหน้า ≥7 วัน; ส่งรายงานตามระยะที่กำหนด  
- **หลักฐาน / Deliverable:** O&M log, test reports, audit plan  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `O ข้อ 3.3.6.1-3.3.6.7`

<a id="permit"></a>

## ขออนุญาตและยื่นเอกสาร (Permit)

<a id="pea-041"></a>

### PEA-041 · ยื่นคำขอเชื่อมต่อ IPU/IPS

- **ใช้กับ Solar Rooftop:** ผลิตใช้เอง  
- **ใช้กับ Solar Farm:** ผลิตใช้เอง  
- **เงื่อนไข / Trigger:** PEA แจ้งผลภายใน 45 วันจากเอกสารครบ หรือเวลาที่กำหนด  
- **สิ่งที่วิศวกรต้องทำ:** ยื่นตามช่องทาง PEA; เผื่อ technical impact request และค่าใช้จ่าย  
- **หลักฐาน / Deliverable:** Application package & response letter  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `S ข้อ 3.3.2-3.3.3`

<a id="pea-042"></a>

### PEA-042 · ขั้นตอน VSPP / SPP

- **ใช้กับ Solar Rooftop:** เฉพาะขายไฟ  
- **ใช้กับ Solar Farm:** เฉพาะขายไฟ  
- **เงื่อนไข / Trigger:** VSPP ต้องตามกระบวนการรับซื้อ/PPA; SPP ตาม PPA EGAT + เชื่อม PEA  
- **สิ่งที่วิศวกรต้องทำ:** ห้ามถือว่า Grid Code ทำให้ขายไฟได้โดยอัตโนมัติ; เช็คสัญญาและประกาศการรับซื้อ  
- **หลักฐาน / Deliverable:** PPA / letter of award / grid approvals  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `S ข้อ 3.1-3.2`

<a id="pea-043"></a>

### PEA-043 · ค่าใช้จ่ายและขยายเขต

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** เจ้าของโครงการรับผิดชอบอุปกรณ์ ทดสอบ ปรับปรุงระบบ และค่าใช้จ่ายที่ PEA เรียก  
- **สิ่งที่วิศวกรต้องทำ:** สำรองค่า PEA review, extension, meter, communication, yearly/periodic maintenance ใน BOQ  
- **หลักฐาน / Deliverable:** Budget, PEA fee letter, BOQ  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `S ข้อ 2.1.2, 3.3.4; C ข้อ 2.1.3`

<a id="construction"></a>

## ติดตั้งและตรวจหน้างาน (Construction)

<a id="pea-044"></a>

### PEA-044 · ติดตั้งตรงตามแบบอนุมัติ

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** อุปกรณ์/ระบบป้องกันตาม Annex 7.1 และ Grid Parameter Approved  
- **สิ่งที่วิศวกรต้องทำ:** Hold point ก่อน energize: ตรวจ CT polarity, interlock, breaker trip, relay, EXL  
- **หลักฐาน / Deliverable:** As-built SLD & site inspection  
- **ประเภทข้อสรุป:** ข้อกำหนด+วิธีตรวจ  
- **อ้างอิง:** `C ข้อ 2.3.1, 2.9; S ข้อ 3.3.3`

<a id="commissioning"></a>

## ทดสอบก่อนเชื่อมต่อ (Commissioning)

<a id="pea-045"></a>

### PEA-045 · ทดสอบ PEA ก่อนเชื่อมต่อ

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** IPU/IPS: PEA ตรวจหลังแจ้งภายใน 30 วัน; ต้องผ่านก่อนเริ่มเชื่อมต่อ  
- **สิ่งที่วิศวกรต้องทำ:** ส่ง Inspection Request, test plan, as-built และเชิญ PEA witness  
- **หลักฐาน / Deliverable:** PEA inspection + grid test acceptance  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `S ข้อ 3.3.3(5)-(7)`

<a id="pea-046"></a>

### PEA-046 · ทดสอบ relay/controls

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** Protection/ EXL / anti-islanding / P,Q,f,V / SCADA ตามแบบและประเภท  
- **สิ่งที่วิศวกรต้องทำ:** ทำ point-to-point, trip logic, deadband, export limiting, remote command records  
- **หลักฐาน / Deliverable:** FAT/SAT + relay injection reports  
- **ประเภทข้อสรุป:** การนำข้อกำหนดไปทดสอบ  
- **อ้างอิง:** `C ข้อ 2.9, Annex 7.1-7.4; O ข้อ 2.3-2.4`

<a id="change-control"></a>

## การเปลี่ยนแปลงระบบ (Change control)

<a id="pea-049"></a>

### PEA-049 · เพิ่มแผง / เพิ่ม inverter / เปลี่ยนพิกัด

- **ใช้กับ Solar Rooftop:** ทุกแบบ  
- **ใช้กับ Solar Farm:** ทุกแบบ  
- **เงื่อนไข / Trigger:** เพิ่มเติม/เปลี่ยนอุปกรณ์หรือไฟฟ้าจ่ายออก ต้องส่งรายละเอียดก่อนดำเนินการ ≥90 วัน  
- **สิ่งที่วิศวกรต้องทำ:** จัดทำ Management of Change; ขอ PEA เห็นชอบ ตรวจ/ทดสอบก่อนเปลี่ยนแปลง  
- **หลักฐาน / Deliverable:** Change request, PEA written approval  
- **ประเภทข้อสรุป:** ข้อกำหนด  
- **อ้างอิง:** `C ข้อ 2.11`

<a id="site-safety"></a>

## วิศวกรรมความปลอดภัยเพิ่มเติม (Site safety)

<a id="pea-050"></a>

### PEA-050 · โครงสร้างหลังคา/ฐานราก

- **ใช้กับ Solar Rooftop:** จำเป็น  
- **ใช้กับ Solar Farm:** จำเป็น  
- **เงื่อนไข / Trigger:** ไม่มีตัวเลข Structural loading ใน Grid Code ทั้ง 4 ฉบับ  
- **สิ่งที่วิศวกรต้องทำ:** ตรวจแรงลม น้ำหนัก โครงหลังคา ฐานราก สภาพดิน และมาตรฐานวิศวกรรมอื่นก่อนติดตั้ง  
- **หลักฐาน / Deliverable:** Signed structural calculation  
- **ประเภทข้อสรุป:** แนวทางวิศวกรรมเพิ่มเติม  
- **อ้างอิง:** `ไม่อยู่ในขอบเขต Grid Code ที่แนบ`

<a id="pea-051"></a>

### PEA-051 · DC design / Lightning / Fire

- **ใช้กับ Solar Rooftop:** จำเป็น  
- **ใช้กับ Solar Farm:** จำเป็น  
- **เงื่อนไข / Trigger:** ไม่มีเกณฑ์ DC cable sizing, fire access, rooftop walkway ใน Grid Code นี้  
- **สิ่งที่วิศวกรต้องทำ:** ทำ DC string sizing, MPPT, cable voltage drop, SPD, earthing, lightning, firefighting access ตามมาตรฐานอื่น  
- **หลักฐาน / Deliverable:** DC design package + ITP  
- **ประเภทข้อสรุป:** แนวทางวิศวกรรมเพิ่มเติม  
- **อ้างอิง:** `ไม่อยู่ในขอบเขต Grid Code ที่แนบ`

---

[ดาวน์โหลด Compliance Matrix CSV](../data/compliance-matrix.csv) · [กลับหน้าหลัก](../README.md)
