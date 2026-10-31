# 02 — ตารางค่าพิกัดและเงื่อนไขสำคัญ (34 รายการ)

[← กลับหน้าหลัก](../README.md) · [← ภาพรวม](01-overview-and-connections.md) · [ต่อไป: Compliance Matrix →](03-compliance-matrix.md)

> **หมายเหตุด้านการใช้งาน:** เนื้อหานี้เรียบเรียงจาก HTML และภาพสรุปที่แนบมา ไม่ใช่ประกาศหรือหนังสืออนุมัติอย่างเป็นทางการของ กฟภ. ก่อนนำตัวเลข/ข้อกำหนดไปใช้ใน TOR, BOQ, งานออกแบบ หรือยื่นเชื่อมต่อ ให้ตรวจเอกสาร กฟภ. ฉบับเต็มและหนังสืออนุมัติเฉพาะโครงการอีกครั้ง

**หลักการอ่าน:** ค่าในคอลัมน์ “เกณฑ์” ใช้ได้ภายใต้เงื่อนไข “ใช้เมื่อ” เท่านั้น; ตัวเลขกำลังส่งออกไม่ใช่ขนาด PV DC ที่ติดตั้ง และไม่ได้แทนเงื่อนไขเฉพาะจุดเชื่อมต่อที่ กฟภ. อนุมัติ

## วันใช้บังคับ

| หัวข้อ | ค่าตามไฟล์สรุป | ใช้เมื่อ / Scope | หมายเหตุ | อ้างอิง |
| --- | --- | --- | --- | --- |
| ประกาศใหม่ | 10 ธ.ค. 2569 | ทุกโครงการ | Official effective date | ประกาศ PEA 10 ก.ย. 2569 |

## ขนาดกำลังส่งออกและขีดจำกัดโครงข่าย

| หัวข้อ | ค่าตามไฟล์สรุป | ใช้เมื่อ / Scope | หมายเหตุ | อ้างอิง |
| --- | --- | --- | --- | --- |
| Export LV 1-phase | ≤ 5 kW/ราย | เฉพาะจ่าย/ขายเข้า PEA | ไม่ใช่ขนาดติดตั้ง DC | C 2.2.1(1) |
| Export LV multi-phase | ≤ 10 kW/ราย | เฉพาะจ่าย/ขายเข้า PEA | ความต่างกำลังผลิตแต่ละเฟส ≤5kW | C 2.2.1(2) |
| LV transformer export hosting | ≤ 25% transformer kVA | รวมผู้ขอ+ผู้เชื่อมต่อทุกราย | เทียบกำลังส่งออก kW กับ rating kVA ตามถ้อยคำข้อกำหนด | C 2.2.1(3) |
| Feeder 22 kV export | ≤ 8 MW/feeder | รวมผู้เชื่อมต่อทุกราย | ต้องตรวจ feeder hosting กับ PEA | C 2.2.2(1) |
| Feeder 33 kV export | ≤ 10 MW/feeder | รวมผู้เชื่อมต่อทุกราย | ต้องตรวจ feeder hosting กับ PEA | C 2.2.2(2) |
| Substation transformer export | ≤ 75% rated kVA | รวมทุก feeder 22/33 kV | คำนวณตาม transformer max rating แต่ละลูก | C 2.2.2 |
| 115 kV single overhead export | ≤ 120 MW/feeder | ผู้เชื่อมต่อทุกรายรวม | Cable/constraints may change limit | C 2.2.3 |
| 115 kV double overhead export | ≤ 230 MW/feeder | ผู้เชื่อมต่อทุกรายรวม | Cable/constraints may change limit | C 2.2.3 |

## Protection, Inverter และการควบคุมความถี่

| หัวข้อ | ค่าตามไฟล์สรุป | ใช้เมื่อ / Scope | หมายเหตุ | อ้างอิง |
| --- | --- | --- | --- | --- |
| Short circuit total | ≤ 85% breaker interrupting capacity | ทุกโครงการ | ประสาน protection | C 2.1.1(3) |
| Inverter anti-islanding | ≤ 1 second | ทุก inverter | ตัดเมื่อต้นทาง PEA ไม่มีไฟ | C 2.9.6 |
| Inverter frequency FRT | 47–52 Hz | ทุก inverter | ride through; นอกช่วงสามารถตัด | C 2.5.2; 2.9.5 |
| Frequency control deadband | 50 ± 0.3 Hz | PCC ≥22kV + Inverter installed >50kW | Connection Code; ดู Operation Code เพิ่ม | C 2.9.5 |
| Frequency droop | 4% หรือ 50% ต่อ 1Hz | PCC ≥22kV + inverter installed >50kW | PEA สามารถเปลี่ยนค่า | C 2.9.5 |
| Operation VSPP band | 49.60–50.40 Hz | ตาม O 3.1.2 เงื่อนไข MV | ไม่เท่ากับ Connection deadband | O 3.1.2.2 |
| Operation IPU/IPS band | 49.50–50.50 Hz | ตาม O 3.3.2 เงื่อนไข MV | ไม่เท่ากับ Connection deadband | O 3.3.2.2 |
| Inverter PF | 0.90 lag – 0.90 lead | ทุก inverter | ที่ rated P | C 2.9.2(1) |
| Volt-var, Volt-watt active threshold | ≥20% rated active power | ทุก inverter | ดู characteristic curves รูป 3–4 | C 2.9.2(2) |

## PQM และ Power Quality

| หัวข้อ | ค่าตามไฟล์สรุป | ใช้เมื่อ / Scope | หมายเหตุ | อ้างอิง |
| --- | --- | --- | --- | --- |
| PQM applicability | Inverter total >250 kW | ทุกโครงการ inverter | ต้องไม่สมมติว่าที่ต่ำกว่านี้ PEA ไม่เรียกเพิ่ม | C 2.4.4 |
| PQM accuracy class S | >250kW ถึง ≤1MW | ทุก inverter | Class S หรือ A, IEC 61000-4-30 | C Annex 7.2 ข้อ 4.4.2 |
| PQM accuracy class A | >1MW | ทุก generator | IEC 61000-4-30 A, 4-7, 4-15 | C Annex 7.2 ข้อ 4.4.1 |
| PQM memory | ≥ 30 days | PQM installed | บันทึกไม่สูญหาย | C Annex 7.2 ข้อ 4.5 |
| PQM UPS | ≥ 15 minutes | PQM installed | และ auto restart | C Annex 7.2 ข้อ 4.6 |
| Power quality monitoring | Total installed >1MW | ทุกประเภท | weather may be required for Solar | C 2.4.4 |
| DC injection | ≤0.5% inverter rated current | ทุก inverter | type-test recommended | C 2.9.10 |

## Reconnection และ CT/VT

| หัวข้อ | ค่าตามไฟล์สรุป | ใช้เมื่อ / Scope | หมายเหตุ | อ้างอิง |
| --- | --- | --- | --- | --- |
| Grid reconnection | ≤5 minutes once grid normal | ทุก inverter | หรือ Ramp Rate ที่ PEA กำหนด | C 2.9.7 |
| Relay CT accuracy | 5P20 หรือดีกว่า | ใช้ Protection Relay | ดู CT burden/saturation | C Annex 7.2 ข้อ 2 |
| Relay VT accuracy | 3P หรือดีกว่า | ใช้ Protection Relay | Relay ต้องมี backup supply | C Annex 7.2 ข้อ 2 |

## งานอนุมัติ ตรวจสอบ และ O&M

| หัวข้อ | ค่าตามไฟล์สรุป | ใช้เมื่อ / Scope | หมายเหตุ | อ้างอิง |
| --- | --- | --- | --- | --- |
| IPU/IPS application review | 45 วันหลังเอกสารครบ | IPU/IPS | หรือที่ PEA กำหนด | S 3.3.3(2) |
| PEA inspection after completion notice | 30 วัน | IPU/IPS | ก่อนทดสอบเชื่อมต่อ | S 3.3.3(5) |
| Modification advance notice | ≥90 วันก่อนเริ่มแก้ไข | เพิ่มเติม inverter/PCC/export | ขอเห็นชอบก่อนเปลี่ยน | C 2.11 |
| IPU/IPS MV audit | ทุก 3 ปี | IPU/IPS PCC ≥22kV | PQ, relay, SCADA (if any) | O 3.3.6.2 |
| Inspection PEA witness notice | ≥7 วันก่อน audit | IPU/IPS PCC ≥22kV | กำหนด PEA ร่วมตรวจ | O 3.3.6.4 |
| Incident report | 3 วันหลังเหตุ | PCC ≥22kV / incident scope | เหตุฉุกเฉินตาม O 2.7.6.5 | O 2.7.6.5 |

## ข้อควรระวังสำหรับ TOR และการตรวจแบบ

1. **PQM:** จากข้อมูลต้นฉบับ ใช้เกณฑ์กำลัง Inverter รวม **มากกว่า 250 kW** ไม่ใช่กำลัง DC ของแผง; ขนาด **250 kW พอดี** ไม่เท่ากับ **>250 kW**
2. **Frequency:** ระวังสับสนระหว่าง *Frequency Ride Through*, *Connection Code Deadband* และ *Operation Code Band* เพราะเป็นข้อกำหนดคนละลักษณะ
3. **Grid reconnection:** ค่าเวลา `≤5 minutes once grid normal` เป็นข้อความที่ถอดตาม HTML แนบ **ควรตรวจถ้อยคำ/ทิศทางเครื่องหมายใน C ข้อ 2.9.7 โดยตรง** ก่อนระบุใน Setting Sheet หรือ TOR
4. **SCADA/Remote:** ให้ยึดรูปแบบการเชื่อมต่อ Annex 7.1, Annex 7.3 และหนังสืออนุมัติรายโครงการ ไม่ใช้เกณฑ์กำลังเพียงตัวเดียว
5. **Grid capacity:** ค่า 22/33/115 kV เป็น screening ระดับโครงข่ายที่ต้องให้ กฟภ. ตรวจยืนยัน ไม่ใช่สิทธิการติดตั้งรายโครงการ

[ดาวน์โหลดตาราง CSV สำหรับ Excel](../data/thresholds.csv) · [ดู Matrix 51 รายการ](03-compliance-matrix.md)
