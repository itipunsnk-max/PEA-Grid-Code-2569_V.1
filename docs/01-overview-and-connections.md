# 01 — ภาพรวมและรูปแบบการเชื่อมต่อ Solar PV

[← กลับหน้าหลัก](../README.md) · [ต่อไป: ค่าพิกัดสำคัญ →](02-key-thresholds.md)

> **หมายเหตุด้านการใช้งาน:** เนื้อหานี้เรียบเรียงจาก HTML และภาพสรุปที่แนบมา ไม่ใช่ประกาศหรือหนังสืออนุมัติอย่างเป็นทางการของ กฟภ. ก่อนนำตัวเลข/ข้อกำหนดไปใช้ใน TOR, BOQ, งานออกแบบ หรือยื่นเชื่อมต่อ ให้ตรวจเอกสาร กฟภ. ฉบับเต็มและหนังสืออนุมัติเฉพาะโครงการอีกครั้ง

## 1. เอกสารหลักที่ต้องรู้จัก

| เอกสาร | คำย่อ | เนื้อหาหลัก |
|---|---|---|
| ประกาศเรื่อง Grid Code พ.ศ. 2569 | Notice | วันบังคับใช้และบทเฉพาะกาลตามประกาศ |
| ข้อกำหนดเกี่ยวกับการเชื่อมต่อระบบโครงข่ายไฟฟ้า | C — Connection Code | ข้อกำหนดทางเทคนิค, การเชื่อมต่อ, Inverter, Protection, Annex 7.1–7.4 |
| ข้อกำหนดเกี่ยวกับการใช้บริการระบบโครงข่ายไฟฟ้า | S — Service Code | การยื่นขอเชื่อมต่อ การพิจารณา การทดสอบ และค่าใช้จ่าย |
| ข้อกำหนดเกี่ยวกับการปฏิบัติการระบบโครงข่ายไฟฟ้า | O — Operation Code | การควบคุม การประสานงาน ความปลอดภัย การทดสอบ และ O&M |

เอกสาร HTML ที่ให้มาระบุวันประกาศ **10 ก.ย. 2569** และวันใช้บังคับ **10 ธ.ค. 2569** พร้อมข้อควรตรวจสอบบทเฉพาะกาลก่อนนำไปใช้กับโครงการเดิม

## 2. แยกกำลังไฟฟ้าให้ถูกต้อง

- **PV DC (kWp):** กำลังพิกัดแผงแสงอาทิตย์ฝั่ง DC
- **Inverter installed AC (kW):** กำลัง AC ของ Inverter ที่ติดตั้งรวมกัน ใช้พิจารณาเงื่อนไขบางรายการ เช่น PQM
- **Export Cap (kW):** กำลังสูงสุดที่ได้รับอนุญาตให้ส่งเข้าสู่โครงข่ายไฟฟ้า ณ จุดเชื่อมต่อ
- **PCC (Point of Common Coupling):** จุดเชื่อมต่ออ้างอิงสำหรับพิจารณาการป้องกัน คุณภาพไฟฟ้า การวัด และการควบคุม

**สำคัญ:** เพดานการส่งไฟใน Grid Code ไม่เท่ากับเพดานกำลังติดตั้งแผง PV และไม่ควรใช้ตัวเลขทั้งสามแทนกัน

## 3. เลือกรูปแบบการเชื่อมต่อเบื้องต้น

ตารางต่อไปนี้ถอดจาก `scenarios` ใน HTML ต้นฉบับ **เป็นตัวอย่างประเภทงาน** ไม่ใช่การรับรองว่าจะเลือกแบบใดได้โดยอัตโนมัติ

| ประเภท | ลักษณะการใช้งาน | PCC / แรงดัน | ขนาด / เงื่อนไข | Annex 7.1 | หัวข้อที่ต้องตรวจ | อ้างอิง |
| --- | --- | --- | --- | --- | --- | --- |
| IPU/IPS | Rooftop self-use | LV 220/380 V | ทุกขนาดตามอนุญาต | 2.1 | ห้าม Export; EXL/32; OCD protection | C 3.3.1; Annex 7.1 แบบ 2.1 |
| IPU/IPS | Rooftop/Farm self-use | 22/33 kV | ≤2 MW | 2.2 | EXL/32; protection; PQM >250kW; VFRT ถ้า >50kW | C 3.3.1; Annex 7.1 แบบ 2.2 |
| IPU/IPS | Rooftop/Farm self-use | 22/33 kV | >2 MW | 2.3 | EXL/32; protection เพิ่มตามแบบ; monitoring | C 3.3.1; Annex 7.1 แบบ 2.3 |
| IPU/IPS | Large self-use | 115 kV | ตามแบบอนุมัติ | 2.4 | EXL/32; PQM, protection and monitoring | C 3.3.1; Annex 7.1 แบบ 2.4 |
| VSPP | Rooftop export | LV 220/380 V | ตาม PEA export cap | 1.1 | Export cap LV 5kW/10kW, EXL ตาม 2.2.1(4) | C 3.1.1; Annex 7.1 แบบ 1.1 |
| VSPP | Farm/Rooftop export | 22/33 kV | ≤1 MW | 1.2 | Protection + PQM ตามเกณฑ์; export cap | C 3.1.1; Annex 7.1 แบบ 1.2 |
| VSPP | Farm/Rooftop export | 22/33 kV | >1 MW | 1.3 | RCS/SCADA + setpoints + PQM + monitoring | C 2.6; 3.1.1; Annex 7.1 แบบ 1.3 |
| SPP | Power producer to EGAT | 115 kV | ตาม PPA/PEA | 3 | SCADA/remote + protection + metering | C 3.2.1; Annex 7.1 แบบ 3 |

### แนวทางเลือกแบบตามลักษณะโครงการ

**A. Solar Rooftop ผลิตใช้เอง (Self-consumption):** แยก IPU/IPS ให้ชัด ระบุ No Export/Zero Export, จุดวัดและ CT ของ EXL, การตัดต่อวงจร และอุปกรณ์ตามระดับแรงดัน

**B. Solar Rooftop ส่ง/ขายไฟ:** ตรวจประเภท VSPP, เงื่อนไขสัญญารับซื้อ, เพดานส่งออก, Meter, Protection และ EXL เมื่อเข้าเงื่อนไข

**C. Solar Farm ผลิตใช้เอง:** ตรวจ PCC/แรงดัน, หม้อแปลง, Protection, Load Flow, Short Circuit, Export Limit และการสื่อสารตามขนาดจริง

**D. Solar Farm ขายไฟ:** ตรวจประเภท VSPP/SPP, ข้อจำกัดโครงข่าย, PQM, Protection, SCADA และข้อกำหนดการสื่อสาร/ควบคุมที่เกี่ยวข้อง

## 4. ลำดับงานตั้งแต่แบบจนจ่ายไฟ

| ขั้น | งานหลัก | Deliverable ที่ควรมี |
|---|---|---|
| 1. Project Basis | ระบุ IPU/IPS/VSPP/SPP, PCC, แรงดัน, กำลัง DC/AC และ Export Cap | Design Basis, Concept SLD |
| 2. Grid Study & Design | Load Flow, Voltage, Short Circuit, Coordination, Inverter, PQM, EXL/SCADA | Study Reports, Design SLD, Protection Settings |
| 3. Application | ส่งแบบและเอกสารขอเชื่อมต่อให้ กฟภ. | Application, PEA Correspondence |
| 4. Installation | ติดตั้งตามแบบอนุมัติ ตรวจ CT/VT, Inverter, Relay, Breaker และ Communication | Inspection Report, As-built, ITP |
| 5. Commissioning | ทดสอบ Protection, Anti-Islanding, EXL/PQM/SCADA ตามเงื่อนไข | Test Reports, SAT, PEA Acceptance |
| 6. Operation | ส่งมอบ O&M, ดูแลค่าตั้งและการเปลี่ยนแปลง | O&M Manual, Change Log |

## 5. คำถามที่ควรตอบก่อนสั่งอุปกรณ์

- [ ] PCC อยู่ที่ LV 400/230 V, MV 22/33 kV หรือ HV 115 kV?
- [ ] โครงการผลิตใช้เองหรือส่ง/ขายไฟ? มีเงื่อนไขห้ามส่งออกหรือไม่?
- [ ] กำลัง Inverter รวมเกิน 250 kW หรือไม่ (ตรวจ PQM)?
- [ ] กำลังรวมเกิน 1 MW หรือไม่ (ตรวจ Monitoring และ PQM Class ตามเงื่อนไข)?
- [ ] Annex 7.1 รูปแบบที่ยื่นและแบบที่ กฟภ. อนุมัติคืออะไร?
- [ ] EXL / Reverse Power Relay ANSI 32 ใช้งานในกรณีใด?
- [ ] Remote Control / SCADA ต้องมีตามรูปแบบโครงการหรือหนังสือ กฟภ. หรือไม่?
- [ ] มี Drawing, Protection Setting, Test Plan และเอกสารยืนยันก่อน Energize ครบหรือยัง?

**อ่านต่อ:** [ค่าพิกัดสำคัญ](02-key-thresholds.md) · [Compliance Matrix](03-compliance-matrix.md) · [รูปภาพหน้าหลัก](../README.md)
