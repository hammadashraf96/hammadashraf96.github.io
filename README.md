<div align="center">

# Hammad Ashraf — 3D Portfolio

**Test & Validation Engineer**

[![Live Site](https://img.shields.io/badge/Live%20Site-hammadashraf96.github.io-e8ff47?style=for-the-badge&logo=github&logoColor=black)](https://hammadashraf96.github.io)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)](https://threejs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](./LICENSE)

*Personal portfolio for Hammad Ashraf — hardware test & validation engineer with experience across ATE platforms, flying probe, power electronics, and Python/SQL automation.*

</div>

---

## ✨ Features

- **3D interactive desktop** model in the hero section (Three.js + React Three Fiber)
- **3D Earth** canvas on the contact section
- **Floating tech ball** animations for the skills section
- **Framer Motion** scroll-reveal animations throughout
- **Fully responsive** — mobile, tablet, and desktop
- **EmailJS** contact form integration
- **Tailwind CSS** dark theme styling

---

## 🧰 Tech Stack

| Layer | Technology |
|---|---|
| Framework | React 18 + TypeScript |
| 3D Graphics | Three.js, @react-three/fiber, @react-three/drei |
| Animations | Framer Motion |
| Styling | Tailwind CSS |
| Build Tool | Vite 5 |
| Contact Form | EmailJS |
| Deployment | GitHub Pages |

---

## 🚀 Getting Started

**Prerequisites:** Node.js ≥ 18, npm ≥ 9

```bash
# Clone the repository
git clone https://github.com/hammadashraf96/reactjs18-3d-portfolio.git
cd reactjs18-3d-portfolio

# Install dependencies
npm install

# Start local dev server
npm run dev
```

Open **http://localhost:5173** in your browser.

---

## 📁 Project Structure

```
src/
├── assets/
│   ├── company/        # Employer logos (Advantest, EV Thermal)
│   ├── projects/       # Project screenshot SVGs
│   └── tech/           # Tech stack icons for 3D balls
├── components/
│   ├── canvas/         # Three.js canvases (Ball, Computers, Earth, Stars)
│   ├── layout/         # Navbar, Loader
│   └── sections/       # Hero, About, Experience, Tech, Works, Contact
├── constants/
│   ├── config.ts       # ⬅ Site metadata, hero text, section headings
│   └── index.ts        # ⬅ Experience, projects, tech stack, services
├── hoc/                # SectionWrapper higher-order component
└── utils/              # Framer Motion variants
```

---

## ✏️ Customization

All personal content lives in just **two files**:

| File | What it controls |
|---|---|
| `src/constants/config.ts` | Page title, hero name & subtitle, section headings, contact form |
| `src/constants/index.ts` | Service cards, tech stack balls, experience timeline, projects |

**After any edit, rebuild and redeploy:**

```bash
npm run build
cd dist
git add .
git commit -m "Update portfolio content"
git push
```

---

## 📬 Contact Form (EmailJS)

The contact form requires a free [EmailJS](https://www.emailjs.com) account.

1. Create an account and add an Email Service + Template
2. Create a `.env` file in the project root:

```env
VITE_APP_EMAILJS_SERVICE_ID=your_service_id
VITE_APP_EMAILJS_TEMPLATE_ID=your_template_id
VITE_APP_EMAILJS_PUBLIC_KEY=your_public_key
```

---

## 🌐 Deployment

Deployed to [GitHub Pages](https://pages.github.com) from the built `dist/` folder.

```bash
# Build
npm run build

# First-time deploy
cd dist
git init
git add .
git commit -m "Deploy portfolio"
git branch -M main
git remote add origin https://github.com/hammadashraf96/hammadashraf96.github.io.git
git push -f origin main

# Subsequent updates (from dist/ with remote already set)
git add .
git commit -m "Update portfolio"
git push
```

---

## 📄 License

MIT — see [LICENSE](./LICENSE)

Template by [maurodesouza](https://github.com/maurodesouza/reactjs18-3d-portfolio) · Customized by Hammad Ashraf © 2026
