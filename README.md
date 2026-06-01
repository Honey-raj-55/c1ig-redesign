# C1 Insurance Group — Website Redesign

**Live Demo → [c1ig-redesign.vercel.app](https://c1ig-redesign.vercel.app)**

A full ground-up redesign of the C1 Insurance Group website — a Dallas-based independent insurance agency serving clients across 29 states. Built with zero frameworks. Every animation, interaction, and UI component is hand-crafted in vanilla HTML, CSS, and JavaScript.

---

## What Was Built

The original site was functional but dated. This redesign turns it into a conversion-focused, premium web experience that matches the agency's 5.0★ reputation.

**The goal:** make a visitor feel confident and taken care of the moment they land — and make it easy to get a quote.

---

## Features

### 🎨 Visual Design
- Dark hero with animated **particle/network canvas** background — 70 nodes drawing live connections in real time
- Layered **radial gradient orbs** with floating animation
- **Grain texture overlay** for a premium editorial feel
- Dual-font system: *Fraunces* (serif display) + *Archivo* (clean sans-serif body)
- Custom **brass/gold** design token system across all components

### ⚡ Interactions & Animation
- **Custom cursor** with magnetic expansion on hover — blends with content via `mix-blend-mode: difference`
- **Scroll progress bar** fixed at the top of the viewport
- **Scroll-triggered reveal animations** via IntersectionObserver — elements rise into view as the user scrolls
- **3D tilt cards** — cards respond to mouse position with `perspective` transforms
- **Parallax layers** — hero orbs and visual frames move at different rates on scroll
- **Animated number counters** — stat numbers count up when they enter the viewport with an easing curve
- **Sticky conversion bar** — slides up from the bottom after scrolling past the hero

### 🧮 Interactive Premium Estimator
One of the most technically involved pieces. A fully client-side insurance quote calculator with:
- **Three product modes** — Home, Auto, Business — each with its own pricing model and breakdown
- **Live sliders** for property value, coverage level, and deductible
- **Toggle add-ons** — Umbrella, Water Backup, Cyber Risk, Valuables — each applies a percentage modifier
- **Animated number transitions** when the estimate updates
- **Breakdown bars** that fill to show premium distribution across coverage categories
- All pricing math runs in the browser — no backend calls

### 🗺️ Navigation
- Fixed header with **blur/frosted glass effect** on scroll
- **Active section highlighting** via IntersectionObserver — the active nav link underlines as you scroll
- **Mobile burger menu** with animated X transition and slide-in panel
- Smooth scroll to all sections

### 📋 Form
- Full quote request form with validation
- Success state replaces the form on submit — no page reload

### ♿ Accessibility & Performance
- `prefers-reduced-motion` respected — all animations and canvas disabled for users who opt out
- `prefers-color-scheme` awareness built into the design system
- Semantic HTML throughout with ARIA-appropriate structure
- **Schema.org structured data** (InsuranceAgency type) embedded in `<head>` for rich search results
- Full SEO meta tags, Open Graph, Twitter Card

---

## Tech Stack

| Layer | Choice |
|---|---|
| HTML | Semantic HTML5 |
| CSS | Custom properties (design tokens), no preprocessor |
| JavaScript | Vanilla ES6+ — no libraries, no build step |
| Fonts | Google Fonts — Fraunces + Archivo |
| Canvas | Native 2D Canvas API for particle network |
| Deployment | Vercel |

**No React. No Tailwind. No build pipeline.** One `index.html` file — 650 lines of intentional, hand-crafted code.

---

## Project Structure

```
c1ig-redesign/
└── index.html        # Everything — markup, styles, and scripts in one file
```

---

## Sections

| Section | What It Does |
|---|---|
| **Hero** | Dark branded landing with particle canvas, rating badge, stats, and coverage snapshot card |
| **Trust Bar** | Award strip — D Magazine, Safeco President's Club, Travelers Top 10, Progressive Platinum |
| **Premium Estimator** | Interactive quote calculator for Home / Auto / Business |
| **About** | Agency story with parallax visual frame and floating badge |
| **Solutions** | Personal and Business insurance with hover-reveal tilt cards |
| **Independent Advantage** | 4-column grid explaining the value of an independent agent |
| **Carriers & Awards** | Animated counters + carrier logo strip |
| **Reviews** | 5.0★ social proof section with 3 featured client cards |
| **Service Center** | Quick-access grid for existing clients |
| **Contact** | 3-step process + quote form + address/phone/email |
| **Footer** | Full sitemap + legal |
| **Sticky Bar** | Conversion CTA that appears after scrolling past the hero |

---

## Local Setup

No dependencies. No npm. No build step.

```bash
git clone https://github.com/Honey-raj-55/c1ig-redesign.git
cd c1ig-redesign
open index.html
```

Or serve it locally:

```bash
npx serve .
# Open http://localhost:3000
```

---

## Design Decisions

**Why vanilla?** C1 Insurance Group needed something fast to ship, easy to hand off, and zero-dependency. A single HTML file deploys anywhere in seconds and needs no maintenance pipeline.

**Why a custom estimator?** Most insurance sites bury the quote behind a phone call. Showing a live number — even a rough one — lowers the barrier for first-time visitors and drives form completions.

**Why this visual direction?** The agency's positioning is premium and trust-based. The dark hero, editorial typography, and brass/gold palette signal quality — the same language used by high-end financial and legal firms — while the warm color temperature keeps it approachable.

---

## Author

**Honey Raj Perupogu**
MS Computer Science, Southern Methodist University
[linkedin.com/in/honey-raj](https://linkedin.com/in/honey-raj) · [github.com/Honey-raj-55](https://github.com/Honey-raj-55)
