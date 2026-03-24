# Kritsakorn Payakmareong — Portfolio

เว็บไซต์ Portfolio ส่วนตัว ออกแบบให้โหลดเร็ว, SEO ดี และดีไซน์ทันสมัย

---

## Tech Stack ที่ใช้

| เทคโนโลยี | เวอร์ชัน | หน้าที่ |
|---|---|---|
| **Astro** | ^5.7.10 | Framework หลัก — Static Site Generator ที่โหลดเร็วมาก เพราะส่ง HTML ล้วนไปยัง browser โดยไม่มี JavaScript ที่ไม่จำเป็น |
| **TailwindCSS** | ^3.4.17 | CSS Framework แบบ Utility-first ใช้เขียน style ผ่าน class โดยตรง ไม่ต้องเขียนไฟล์ CSS แยก |
| **@astrojs/tailwind** | ^6.0.2 | Integration ที่เชื่อม Astro กับ TailwindCSS ให้ทำงานร่วมกันได้อัตโนมัติ |
| **Sharp** | ^0.33.5 | Library สำหรับ optimize รูปภาพ (resize, compress) ตอน build |
| **TypeScript** | (built-in) | Type safety — ช่วยจับ bug ตั้งแต่ตอนเขียนโค้ด |
| **Google Fonts** | — | ฟอนต์ **Inter** (ตัวอักษรหลัก) และ **Space Grotesk** (หัวข้อ/display) |

---

## สิ่งที่ต้องมีก่อนรัน (Prerequisites)

- **Node.js** เวอร์ชัน 18 ขึ้นไป — [ดาวน์โหลดได้ที่ nodejs.org](https://nodejs.org/)
- **npm** (มาพร้อมกับ Node.js)

ตรวจสอบว่าติดตั้งแล้วด้วยคำสั่ง:

```bash
node -v
npm -v
```

---

## วิธีรันโปรเจค

### 1. Clone โปรเจค

```bash
git clone <repository-url>
cd portfolio
```

### 2. ติดตั้ง Dependencies

```bash
npm install
```

### 3. รัน Development Server

```bash
npm run dev
```

เปิดเบราว์เซอร์ไปที่ **http://localhost:4321** เพื่อดูเว็บไซต์

### 4. Build สำหรับ Production

```bash
npm run build
```

ไฟล์ที่ build เสร็จจะอยู่ในโฟลเดอร์ `dist/`

### 5. Preview Production Build

```bash
npm run preview
```

ใช้ดูตัวอย่างเว็บที่ build แล้วก่อน deploy จริง

---

## โครงสร้างโปรเจค

```
portfolio/
├── public/
│   └── favicon.svg            # ไอคอนของเว็บ
├── src/
│   ├── components/
│   │   ├── Navbar.astro       # แถบนำทาง (เลื่อนแล้วเปลี่ยนเป็น floating pill)
│   │   ├── Hero.astro         # หน้าแรก hero section
│   │   ├── About.astro        # เกี่ยวกับตัวเอง + สถิติ
│   │   ├── Skills.astro       # ทักษะ/เทคโนโลยีที่ใช้
│   │   ├── Projects.astro     # ผลงาน/โปรเจค
│   │   ├── Experience.astro   # ประสบการณ์ + การศึกษา
│   │   ├── Contact.astro      # ช่องทางติดต่อ
│   │   └── Footer.astro       # ส่วนท้ายเว็บ
│   ├── layouts/
│   │   └── Layout.astro       # Layout หลัก (SEO, fonts, global styles)
│   └── pages/
│       └── index.astro        # หน้าหลักที่รวมทุก component
├── astro.config.mjs           # ตั้งค่า Astro
├── tailwind.config.mjs        # ตั้งค่า TailwindCSS (สี, ฟอนต์, animation)
├── tsconfig.json              # ตั้งค่า TypeScript
└── package.json               # Dependencies และ scripts
```

---

## ฟีเจอร์หลัก

- **Responsive Design** — รองรับทุกขนาดหน้าจอ (mobile-first)
- **Floating Pill Navbar** — แถบนำทางเปลี่ยนเป็นทรงแคปซูลลอยเมื่อเลื่อนหน้า
- **Scroll Reveal Animations** — แอนิเมชันเมื่อ element เลื่อนเข้ามาในหน้าจอ (Intersection Observer)
- **Magnetic Cursor** — ปุ่ม CTA มีเอฟเฟกต์แม่เหล็กตามเมาส์
- **Glass Morphism** — การ์ดแบบกระจกขุ่นพร้อม hover lift effect
- **SEO สมบูรณ์** — Open Graph, Twitter Card, semantic HTML
- **Noise Texture Overlay** — พื้นผิว noise ละเอียดให้ความรู้สึกพรีเมียม
- **Marquee Text** — แถบตัวอักษรเทคโนโลยีเลื่อนอัตโนมัติ
- **Dark Theme** — ธีมมืดพร้อมสี accent (Indigo + Lime Green)
