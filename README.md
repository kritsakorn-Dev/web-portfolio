# Kritsakorn Payakmareong — Portfolio

A personal portfolio website designed to load fast, with strong SEO and a modern design.

---

## Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| **Astro** | ^5.7.10 | Main framework — a Static Site Generator that loads very fast by shipping pure HTML to the browser without unnecessary JavaScript |
| **TailwindCSS** | ^3.4.17 | Utility-first CSS framework that lets you style directly via classes without writing separate CSS files |
| **@astrojs/tailwind** | ^6.0.2 | Integration that connects Astro with TailwindCSS so they work together automatically |
| **Sharp** | ^0.34.5 | Library for image optimization (resize, compress) at build time |
| **TypeScript** | (built-in) | Type safety — helps catch bugs while writing code |
| **Google Fonts** | — | **Inter** font (main body text) and **Space Grotesk** (headings/display) |

---

## Prerequisites

- **Node.js** version 18 or higher — [download from nodejs.org](https://nodejs.org/)
- **npm** (comes with Node.js)

Verify your installation with:

```bash
node -v
npm -v
```

---

## How to Run the Project

### 1. Clone the project

```bash
git clone <repository-url>
cd portfolio
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run the development server

```bash
npm run dev
```

Open your browser at **http://localhost:4321** to view the website.

### 4. Build for production

```bash
npm run build
```

The built files will be located in the `dist/` folder.

### 5. Preview the production build

```bash
npm run preview
```

Use this to preview the built site before deploying it for real.

---

## Project Structure

```
portfolio/
├── public/
│   └── favicon.svg            # Website icon
├── src/
│   ├── components/
│   │   ├── Navbar.astro       # Navigation bar (turns into a floating pill on scroll)
│   │   ├── Hero.astro         # Landing hero section
│   │   ├── About.astro        # About me + statistics
│   │   ├── Skills.astro       # Skills/technologies used
│   │   ├── Projects.astro     # Works/projects
│   │   ├── Experience.astro   # Experience + education
│   │   ├── Contact.astro      # Contact channels
│   │   └── Footer.astro       # Website footer
│   ├── layouts/
│   │   └── Layout.astro       # Main layout (SEO, fonts, global styles)
│   └── pages/
│       └── index.astro        # Main page composing all components
├── tailwind.config.mjs        # TailwindCSS config (colors, fonts, animation)
├── astro.config.mjs           # Astro config
├── tsconfig.json              # TypeScript config
└── package.json               # Dependencies and scripts
```

---

## Key Features

- **Responsive Design** — supports every screen size (mobile-first)
- **Floating Pill Navbar** — the navigation bar morphs into a floating capsule on scroll
- **Scroll Reveal Animations** — animations triggered as elements enter the viewport (Intersection Observer)
- **Magnetic Cursor** — CTA buttons feature a magnetic-mouse effect
- **Glass Morphism** — frosted-glass cards with a hover lift effect
- **Comprehensive SEO** — Open Graph, Twitter Card, semantic HTML
- **Noise Texture Overlay** — subtle noise surface for a premium feel
- **Marquee Text** — auto-scrolling technology text strip
- **Dark Theme** — dark theme paired with an accent color (Lime Green)
