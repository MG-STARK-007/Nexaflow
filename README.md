# Nexaflow

## 📌 Project Overview
Nexaflow is a premium SaaS landing page for a fictional AI data automation platform. Built in **Vanilla JS** and **custom CSS**, it was developed under a 4‑hour challenge with strict engineering and design requirements. The focus was on performance, semantics, and smooth motion, packaged as a single deployable `.html` file.

---

## ✨ Core Features

### 1. Pricing Engine
- Dynamic pricing table with toggles for **Monthly/Annual billing** and **INR/USD/EUR currencies**.
- Prices computed from a multi‑dimensional matrix (`PRICING_MATRIX`) factoring:
  - Base USD rate  
  - Currency conversion rate  
  - Regional tariff multiplier  
  - Billing cycle multiplier  
- Direct text node mutations (`node.firstChild.data`) ensure **no global reflows** or layout recalculations.

### 2. Bento → Accordion with Context Lock
- **Desktop:** Features displayed in a CSS bento grid.  
- **Mobile (≤768px):** Same content transforms into a touch‑friendly accordion.  
- **Context lock:** Active bento card auto‑opens as the corresponding accordion item when crossing breakpoints.  
- Implemented with a debounced `window.resize` listener + `requestAnimationFrame` for smooth transitions.

---

## 🛠️ Tech Choices
- **Vanilla JS** (zero dependencies, minimal bundle size).  
- **Custom CSS** with design tokens (`--forsythia`, `--nocturnal`, etc.).  
- **Semantic HTML5** structure (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).  
- **SEO/OG tags** for discoverability and social sharing.  
- **Performance:** Loader animation runs for 480ms, entry animations are CSS‑based with hardware acceleration.

---

## 🚀 Deployment
- Single self‑contained `.html` file.  
- Can be deployed instantly on **Netlify** or **GitHub Pages**.  

---

## ✅ Scoring Criteria Met
- **Logic & Architecture (40 pts):** Matrix pricing, state isolation, bento‑accordion context lock.  
- **SEO & Semantics (30 pts):** Semantic HTML, full meta suite, optimized load performance.  
- **UI/UX & Motion (30 pts):** Responsive breakpoints, smooth transitions, accurate motion timings.  

---

## 📖 Simple Description
Nexaflow is a responsive SaaS landing page showcasing a fictional AI data automation platform. It features a dynamic pricing engine (multi‑currency + billing cycle toggle) and a responsive bento‑to‑accordion layout with context lock. The project emphasizes performance, semantic HTML, and smooth motion, packaged as a single deployable `.html` file for Netlify or GitHub Pages.
