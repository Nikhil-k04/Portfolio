# 🔥 Ember & Oak — Restaurant Landing Page

> **Project 1: Front-End Web Development**
> A fully responsive, single-page marketing website for a fictional wood-fired restaurant.

---

## 📸 Project Overview

**Concept:** Ember & Oak is a rustic modern wood-fired kitchen & bar. The design uses deep charcoal tones, warm amber/fire accents, and Playfair Display serif typography to evoke warmth, craft, and premium dining.

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Semantic page structure |
| CSS3 + Custom Properties | Theming, animations, layout |
| Bootstrap 5.3 | Grid, navbar, carousel, modal |
| Bootstrap Icons | Icon set |
| Vanilla JavaScript (ES6+) | All interactions, validation |
| Google Fonts | Playfair Display + Lato |

> ⚠️ **No JavaScript frameworks used** — pure vanilla JS only.

---

## 📁 File Structure

```
project1/
├── index.html              # Main HTML file
├── css/
│   └── custom.css          # All custom styles + CSS variables + dark mode
├── js/
│   └── main.js             # All JavaScript interactions
├── assets/
│   └── images/             # (placeholder — replace with real images)
└── README.md               # This file
```

---

## 🚀 How to Run Locally

No build step required. Simply open the file in a browser:

**Option A — Direct open:**
```bash
# Navigate to the project folder and open index.html
open project1/index.html
```

**Option B — Local server (recommended to avoid CORS issues):**
```bash
# Using Python
cd project1
python3 -m http.server 3000
# Then visit http://localhost:3000

# Using Node.js / npx
npx serve project1
# Then visit the URL shown
```

---

## 📋 Sections Implemented

| Section | Description |
|---|---|
| 🧭 **Navbar** | Sticky, transparent → solid on scroll, active link highlighting, mobile-responsive |
| 🔥 **Hero** | Full-viewport, animated fire particles, tagline, dual CTAs |
| 🏠 **About** | Brand story, overlapping image layout, stats cards |
| 🍽️ **Menu Highlights** | 8 signature dishes as responsive cards with badges |
| 🖼️ **Gallery** | CSS grid layout, Bootstrap modal lightbox with prev/next navigation |
| ⭐ **Testimonials** | Bootstrap carousel with 5 customer reviews |
| 📍 **Contact & Location** | Info panel, embedded Google Map, booking form |
| 🦶 **Footer** | Social links, opening hours, quick nav links |

---

## ✅ Functional Features

### JavaScript Form Validation
- Required field checks (first name, last name, email, phone, date, time, guests, T&C checkbox)
- Email format validation via regex
- Phone number format and length validation (7–15 digits)
- Min/max length for name fields
- Date validation: no past dates, no Mondays (closed day)
- Real-time validation on blur
- Character counter for notes textarea (max 300)
- Loading state on submit + success confirmation message

### Dark Mode Toggle
- Saved to `localStorage` and restored on page load
- Smooth CSS transition between themes
- Icon changes between 🌙 and ☀️

### Today's Special Badge
- Shown/hidden based on day of week using JavaScript
- Different special message per day (Tue–Sat)
- Hidden on Sunday and Monday (closed)
- Animated pulsing glow effect

### Gallery Lightbox
- Bootstrap modal
- Prev/Next navigation buttons
- Keyboard arrow key support
- Image counter display
- Accessible with ARIA labels

---

## ♿ Accessibility Features

- Semantic HTML: `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<address>`
- `alt` text / `aria-label` on all images and interactive elements
- Visible `:focus-visible` states with orange outline
- `aria-required`, `aria-live`, `role="alert"` on form elements
- ARIA labels on all carousel controls and modal
- Color contrast: all text meets WCAG AA minimum
- Skip-to-content not required (single page with anchor nav)

---

## 🔍 SEO Features

- `<title>` tag: "Ember & Oak | Wood-Fired Kitchen & Bar"
- Meta `description` and `keywords`
- Open Graph tags (`og:title`, `og:description`, `og:type`, `og:image`, `og:url`)
- Emoji favicon via inline SVG data URI
- Semantic heading hierarchy (H1 → H2 → H3)

---

## 🎨 Stretch Features Implemented

- [x] **Today's Special badge** — day-based JavaScript logic
- [x] **Dark mode toggle** — persisted via `localStorage`
- [x] **SEO meta tags** — title, description, Open Graph tags, favicon

---

## 📊 Evaluation Criteria Alignment

| Criteria | Max | Implementation |
|---|---|---|
| Layout & responsiveness | 15 | Bootstrap grid, CSS Grid gallery, mobile nav, no horizontal scroll |
| Visual polish | 10 | Custom fonts, fire color palette, hover animations, dark mode |
| JavaScript & validation | 10 | 8-field validation, lightbox, dark mode, today's special, scroll animations |
| Accessibility & code quality | 5 | Semantic HTML, ARIA, focus states, clean modular JS |
| **Total** | **40** | |
