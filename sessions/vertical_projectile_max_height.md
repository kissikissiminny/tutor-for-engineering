# Session: การหาความสูงสูงสุดของการขว้างวัตถุในแนวดิ่ง

## โจทย์
ขว้างก้อนหินมวล $m = 2\text{ kg}$ ขึ้นไปในแนวดิ่งด้วยความเร็วต้น $u = 30\text{ m/s}$ จงหาความสูงสูงสุด ($h_{\text{max}}$) ที่ก้อนหินขึ้นไปได้ (กำหนดความเร่งโน้มถ่วง $g \approx 9.8\text{ m/s}^2$ หรือ $10\text{ m/s}^2$)

## ตัวแปรที่ระบุได้ (Identify)
- $m = 2\text{ kg}$
- $u = 30\text{ m/s}$ (ทิศขึ้น)
- $v = 0\text{ m/s}$ (ที่จุดสูงสุด)
- Find: $h_{\text{max}}$

## การสร้างแบบจำลอง (Physical Modeling)
- กำหนดแกนพิกัด: ทิศขึ้นเป็นบวก ($+$)
- แรงโน้มถ่วงกระทำในทิศลง: $a = -g$ (ความหน่วงเนื่องจากแรงโน้มถ่วง)
- สมมติฐาน: ละเว้นแรงต้านอากาศ (Free Fall)

## สมการหลัก (Governing Equation)
- $v^2 = u^2 + 2as$ โดยที่ $a = -g$ และ $s = h_{\text{max}}$
- จัดรูปได้: $0 = u^2 - 2g h_{\text{max}} \implies h_{\text{max}} = \frac{u^2}{2g}$

## การคำนวณ (Progressive Calculation)
- จาก $h_{\text{max}} = \frac{u^2}{2g}$
- แทนค่า $u = 30\text{ m/s}$ และ $g = 10\text{ m/s}^2$:
  $$h_{\text{max}} = \frac{30^2}{2(10)} = \frac{900}{20} = 45\text{ m}$$
  *(หากใช้ $g = 9.8\text{ m/s}^2$ จะได้ $h_{\text{max}} \approx 45.92\text{ m}$)*
- **ข้อสังเกต:** มวล $m = 2\text{ kg}$ ไม่ส่งผลต่อความสูงสูงสุด (Mass independence)

## การตรวจสอบความถูกต้อง (Sanity Check)
1. **Unit & Dimension Analysis:** 
   $$[h_{\text{max}}] = \frac{[u]^2}{[g]} = \frac{(\text{m/s})^2}{\text{m/s}^2} = \frac{\text{m}^2/\text{s}^2}{\text{m/s}^2} = \text{m}$$ (ได้มิติความยาว $[L]$ ตรงกับระยะความสูง)
2. **Physical Plausibility:** ความเร็ว $30\text{ m/s}$ (ประมาณ $108\text{ km/h}$) ใช้เวลาขึ้นจนหยุดนิ่ง $t = \frac{u}{g} = 3\text{ s}$ ความเร็วเฉลี่ย $\bar{v} = 15\text{ m/s}$ ระยะทาง $s = \bar{v}t = 15 \times 3 = 45\text{ m}$ สมเหตุสมผล
3. **Extreme Case Analysis:** เมื่อ $g \to \infty \implies h_{\text{max}} \to 0$ เพราะ $h_{\text{max}} \propto \frac{1}{g}$ สอดคล้องกับฟิสิกส์จริงที่แรงดึงดูดมหาศาลจะกดไม่ให้วัตถุลอยขึ้นได้สูง

## สถานะความคืบหน้า
- [x] 1. Identify (Givens & Find)
- [x] 2. Physical Modeling & Governing Equation
- [x] 3. Progressive Calculation
- [x] 4. Sanity Check (เสร็จสมบูรณ์)
