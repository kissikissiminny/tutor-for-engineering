# Session: การหาความเร็วของวัตถุก่อนกระทบพื้น (Free Fall)

## โจทย์
ปล่อยวัตถุมวล $m = 2\text{ kg}$ ตกจากหน้าผาสูง $h = 20\text{ m}$ ลงสู่พื้นดิน จงหาความเร็วของวัตถุก่อนกระทบพื้น ($v$) โดยไม่คิดแรงต้านอากาศ

## แหล่งอ้างอิง (Ground Truth)
- [sources/mechanics/reference.md](file:///c:/Users/Lenovo/Desktop/my-first-project/sources/mechanics/reference.md)

## ตัวแปรที่ระบุได้ (Identify & Model)
- $m = 2\text{ kg}$
- $u = 0\text{ m/s}$ (ปล่อยตกจากหยุดนิ่ง)
- $s = 20\text{ m}$ (ทิศลง)
- กำหนดทิศลงเป็นบวก ($+$) $\implies a = +g$
- Find: $v$ (ความเร็วก่อนกระทบพื้น)

## สมการหลัก (Governing Equation)
- กฎการอนุรักษ์พลังงานกล: $E_{\text{mech}} = K_1 + U_1 = K_2 + U_2$ *(อ้างอิง: `sources/mechanics/reference.md`)*
- พลังงานจลน์: $K = \frac{1}{2}mv^2$
- พลังงานศักย์โน้มถ่วง: $U_g = mgh$

## การคำนวณ (Progressive Calculation)
- จาก $mgh = \frac{1}{2}mv^2 \implies v = \sqrt{2gh}$
- แทนค่า $h = 20\text{ m}$:
  - กรณีใช้ $g = 10\text{ m/s}^2$: $v = \sqrt{2(10)(20)} = 20\text{ m/s}$ ($72\text{ km/h}$)
  - กรณีใช้ $g = 9.81\text{ m/s}^2$ *(อ้างอิง: `sources/mechanics/reference.md`)*: $v = \sqrt{2(9.81)(20)} \approx 19.81\text{ m/s}$

## การตรวจสอบความถูกต้อง (Sanity Check)
1. **Unit & Dimension Analysis:** 
   $$[v] = \sqrt{[g][h]} = \sqrt{\left(\frac{\text{m}}{\text{s}^2}\right)(\text{m})} = \sqrt{\frac{\text{m}^2}{\text{s}^2}} = \text{m/s}$$ (ตรงตามมิติความเร็ว $[L T^{-1}]$)
2. **Physical Plausibility:** ตกจากตึกสูงประมาณ 6 ชั้น ($20\text{ m}$) ความเร็วแตะพื้นราว $72\text{ km/h}$ ถือว่าสมเหตุสมผลเชิงกายภาพ
3. **Mass Independence (Equivalence Principle):** มวล $m$ ตัดกันหมดทั้งสองข้างของสมการ ($v = \sqrt{2gh}$) ดังนั้นไม่ว่าวัตถุจะมีมวล $2\text{ kg}$ หรือ $200\text{ kg}$ ความเร็วก่อนกระทบพื้นจะเท่ากันเสมอเมื่อไม่คิดแรงต้านอากาศ

## สถานะความคืบหน้า
- [x] 1. Identify & Model (Givens & Find, Coordinate/Assumptions)
- [x] 2. Governing Equations & Ground Truth Verification
- [x] 3. Progressive Calculation
- [x] 4. Sanity Check (เสร็จสมบูรณ์)
