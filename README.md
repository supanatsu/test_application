# For My Dear 💕 — README

## ไฟล์ที่ต้องนำไป deploy

| ไฟล์ | คำอธิบาย |
|------|----------|
| `index.html` | แอพหลัก (ทุก feature อยู่ในนี้) |
| `service-worker.js` | ทำให้ใช้ offline ได้ + Push notifications |
| `manifest.json` | ข้อมูล PWA สำหรับการติดตั้ง |
| `icon-192.png` | ไอคอนแอพ 192×192 px |
| `icon-512.png` | ไอคอนแอพ 512×512 px |

> **หมายเหตุ:** ต้องสร้างไฟล์รูป icon-192.png และ icon-512.png เอง (รูปหัวใจสีชมพู)  
> ใช้ https://realfavicongenerator.net หรือ Canva สร้างได้เลย

---

## วิธี Deploy (ฟรี ไม่มีค่าใช้จ่าย)

### วิธีที่ 1: GitHub Pages (แนะนำ)
1. สร้าง repository ใน GitHub
2. Upload ไฟล์ทั้งหมดขึ้นไป
3. ไปที่ Settings → Pages → Source: `main` branch
4. รอสักครู่ แล้วเข้าที่ `https://username.github.io/repo-name`
5. **ต้องใช้ HTTPS** (GitHub Pages ให้ HTTPS อัตโนมัติ)

### วิธีที่ 2: Netlify (ง่ายที่สุด)
1. ไปที่ https://netlify.com
2. ลาก folder ไฟล์ทั้งหมดวางในหน้า "Deploy"
3. ได้ URL ทันที เช่น `https://dear-app.netlify.app`

### วิธีที่ 3: Vercel
1. ไปที่ https://vercel.com
2. เชื่อมกับ GitHub repo
3. Deploy อัตโนมัติทุกครั้งที่ push

---

## วิธีติดตั้งเป็นแอพบนมือถือ

### Android (Chrome)
1. เปิดเว็บใน Chrome
2. กดจุด 3 จุด → "Add to Home screen"
3. หรือรอ banner ที่แอพจะแสดงเอง

### iOS (Safari)
1. เปิดเว็บใน Safari (ต้องเป็น Safari เท่านั้น)
2. กดปุ่ม Share → "Add to Home Screen"
3. กด "Add"

---

## Features ทั้งหมด

### 💌 หน้าหลัก
- ข้อความบอกรัก 20 ข้อความ สุ่มได้เรื่อยๆ
- นับครั้งที่บอกรัก / จำนวนวันที่คบ / Streak
- Countdown ถึงวันสำคัญ (ตั้งค่าได้)
- เขียนและบันทึกจดหมายรัก + ประวัติ
- สติ๊กเกอร์ 35 แบบ แนบในจดหมาย
- Heartfall animation

### 📸 ความทรงจำ
- อัลบั้มรูปภาพ (บันทึกใน localStorage)
- Timeline บันทึก Moment สำคัญ
- Milestones (7 วัน / 1 เดือน / 100 วัน / ครบปี ...)

### ✅ ประจำวัน
- Checklist 8 ภารกิจ + เพิ่มเองได้
- Mood tracker 6 อารมณ์ + กราฟรายอาทิตย์
- Health tracker: น้ำ / ก้าว / ชั่วโมงนอน
- Period tracker
- ฝึกหายใจคลายเครียด (4-4-6-2)
- เคล็ดลับสุขภาพประจำวัน

### 🎲 สนุก
- Love Quiz 7 คำถาม + คะแนน
- วัดความเข้ากัน (ใส่ชื่อ 2 คน)
- วงล้อ Date night (8 ตัวเลือก)
- Bucket List ของเรา
- ดวงความรักประจำวัน (10 ดวง)

### ⚙️ เครื่องมือ
- Sticky Notes (ไม่จำกัด)
- Timer / Pomodoro (25/5/10 นาที)
- เครื่องคิดเลข (ครบฟังก์ชั่น)
- หารค่าใช้จ่าย + คำนวณ VAT/Service
- สุ่มไอเดีย (อาหาร/หนัง/เดท/ของขวัญ)
- ดูตำแหน่ง GPS + เปิดใน Google Maps
- ตั้งค่าชื่อแอพ / วันที่เริ่มคบ / Notifications

---

## ข้อกำหนด
- ต้องใช้ **HTTPS** (PWA บังคับ)
- เบราว์เซอร์สมัยใหม่: Chrome 80+ / Safari 14+ / Firefox 75+
- ข้อมูลทั้งหมดเก็บใน **localStorage** (ไม่มีเซิร์ฟเวอร์)
