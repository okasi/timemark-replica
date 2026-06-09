# 📸 Timemark Replica - Watermark Studio ⚡

A high-fidelity, resolution-independent camera timestamp watermark tool designed to look identical to the **Timemark** app watermarks. 

This is a **replica** watermark utility built entirely with HTML5 Canvas, Javascript, and Vanilla CSS. It runs 100% locally in your browser and lets you batch/single-watermark photos with precise design control.

---

## ✨ Features

- **🎯 Exact Timemark Replica**: Tall, condensed clock lettering, a vertical yellow/gold line, and stacked date details with drop shadows.
- **🌐 Dynamic Multi-Language Locales**: Formats the date and day-of-week dynamically based on the chosen language (e.g. Indonesian `id-ID` yields `28 Mei 2026` & `Kamis`).
- **📏 Resolution-Independent Canvas Drawing**: Scales the font sizes and margins relative to the uploaded image's short edge so that the watermark looks identical on a 400px profile pic or a 5000px DSLR photo!
- **⚡ Interactive Controls**:
  - Live clock toggles vs manual overrides (type whatever you want).
  - Sliders for scale, margins (X & Y), divider height/thickness, and drop-shadow intensity.
  - **🔄 Reset Fidelity** button to instantly restore dividers and shadows back to the reference design settings.
- **🎨 Design Customizations**: Adjust font color, divider color, and pick from Google Fonts like `Barlow Condensed`, `Roboto Condensed`, `Oswald`, and `Share Tech Mono`.
- **💻 Drag & Drop**: Drop any image anywhere onto the preview area to import it instantly.
- **🔒 Private & Secure**: Zero server uploads! Your images are processed entirely in your browser.

---

## 🚀 Getting Started

### 1. Installation
First, open your terminal, navigate to the folder, and install dependencies:
```bash
cd /Users/okasi/Developer/timemark-replica
npm install
```

### 2. Start the Local Dev Server
Run the Vite development server:
```bash
npm run dev
```

### 3. Open the App
Open the local URL in your browser:
👉 **[http://localhost:5173/](http://localhost:5173/)**

---

## 🛠️ Tech Stack
- **Core**: HTML5, Canvas API, JavaScript (ES6)
- **Styling**: Vanilla CSS (CSS Grid, Variables, Glassmorphism backdrop-filters)
- **Tooling**: Vite (for dev server)
