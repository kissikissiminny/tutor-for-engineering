# Session: การหาแรงต้านทานเฉลี่ยในการเบรกรถยนต์

## โจทย์
รถยนต์มวล $m = 1000\text{ kg}$ วิ่งด้วยความเร็ว $u = 20\text{ m/s}$ เหยียบเบรกจนหยุดนิ่งในระยะทาง $s = 50\text{ m}$ จงหาแรงต้านทานเฉลี่ย

## ตัวแปรที่ระบุได้ (Identify)
- $m = 1000\text{ kg}$
- $u = 20\text{ m/s}$
- $v = 0\text{ m/s}$
- $s = 50\text{ m}$
- Find: $\bar{F}_{\text{res}}$ (แรงต้านทานเฉลี่ย)

## แนวทางการคำนวณที่เลือก
- กฎการเคลื่อนที่ของนิวตัน: $\Sigma F = ma$
- สมการจลนศาสตร์: $v^2 = u^2 + 2as$

## การคำนวณ (Calculation)
- จาก $0^2 = 20^2 + 2(a)(50) \implies 100a = -400 \implies a = -4\text{ m/s}^2$
- แรงลัพธ์: $\Sigma F = ma = (1000\text{ kg})(-4\text{ m/s}^2) = -4000\text{ N}$
- **คำตอบ:** แรงต้านทานเฉลี่ยมีขนาด $4000\text{ N}$ (หรือ $4\text{ kN}$) มีทิศตรงข้ามกับการเคลื่อนที่

## Sanity Check
1. **Unit & Dimension Analysis:** $[\text{kg}] \cdot [\text{m/s}^2] = [\text{kg}\cdot\text{m/s}^2] = [\text{N}]$ (สอดคล้องกับมิติของแรง $[M L T^{-2}]$)
2. **Physical Plausibility:** $4000\text{ N} \approx 0.4g$ ของน้ำหนักรถ ($W \approx 10000\text{ N}$) ซึ่งสมเหตุสมผลกับแรงเบรกปกติของยางรถยนต์บนพื้นถนนแห้ง ($\mu \approx 0.4$)

## สถานะความคืบหน้า
- [x] 1. Identify (Givens & Find)
- [x] 2. Physical Modeling & Governing Equation
- [x] 3. Calculation & Sanity Check (เสร็จสมบูรณ์)
