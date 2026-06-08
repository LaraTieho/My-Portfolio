# Tieho Lara — Portfolio Website

> **Geomatics & GIS Consultant** | Maseru, Lesotho  
> Turning Spatial Data Into Decisions That Save Lives

A professional portfolio website built with vanilla HTML5, CSS3, and JavaScript, featuring Three.js 3D animations, glassmorphism UI, and smooth scroll interactions.

---

## Live Demo

🔗 **[tieholara.github.io]([https://tieholara.github.io](https://my-portfolio-tlara.vercel.app/))** 

---

## Features

- **3D animated hero** — Three.js particle field with mouse-parallax effect
- **3D orbit rings** — animated torus rings around the profile photo (Three.js)
- **Glassmorphism cards** — backdrop-blur panels with subtle green-tinted borders
- **Custom animated cursor** — lerp-based outer ring tracking inner dot
- **Page loading animation** — monogram pulse with progress bar, auto-dismisses after 2 s
- **Scroll-triggered animations** — staggered viewport-entry transitions via Intersection Observer
- **Animated skill bars** — triggered on scroll, eased CSS transitions
- **Animated counters** — stat numbers count up from zero on entry
- **Project gallery** — filterable tabs (All / Health GIS / Standards & NSDI / WebGIS / Humanitarian) with clickable thumbnail strips that swap the primary project image
- **Contact form** — client-side validation with success state (wire to Formspree or Netlify Forms for production)
- **Fully responsive** — desktop (≥992 px), tablet (768–991 px), mobile (≤767 px) with hamburger nav

---

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styles | CSS3 (custom properties, Grid, Flexbox, `clamp()`) |
| Scripts | Vanilla JavaScript (ES6+) |
| 3D graphics | [Three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) via CDN |
| Fonts | [Google Fonts](https://fonts.google.com) — Space Grotesk + Inter |
| Deployment | GitHub Pages |

No build step, no bundler, no framework — a single `index.html` with no external dependencies beyond a CDN script tag.

---

## File Structure

```
/
├── index.html                      # Main website (all HTML, CSS, JS)
├── headshot.jpeg                   # Profile photo
├── Tieho Lara 2026 CV.pdf          # Downloadable CV
├── README.md                       # This file
└── Photos/
    ├── GIS Consultant/             # GDI Advisors / CHAI / MoH work
    │   ├── MoH_1.jpeg
    │   ├── MoH_2.jpeg
    │   ├── MoH_3.jpeg
    │   ├── MoH_5.jpeg
    │   ├── MoH_D1.jpeg
    │   ├── MoH_D2.jpeg
    │   ├── MoH_D3.jpeg
    │   ├── MoH_T1.jpeg
    │   ├── MoH_T2.jpeg
    │   ├── MoH_T3.jpeg
    │   ├── MoH_T4.jpeg
    │   └── MoL_3.jpeg
    ├── Geomatics Technical Consultant/   # GIZ / NSDI standards work
    │   ├── MoLC_1.jpeg
    │   ├── MoLC_2.jpeg
    │   ├── MoLC_3.jpeg
    │   ├── MoLC_4.jpeg
    │   ├── MoLC_5.jpeg
    │   └── MoLC_6.jpeg
    └── Geomatics Engineering/      # Land surveying / UAV / World Vision
        ├── GC_01.jpeg
        ├── GC_2.jpeg
        ├── GC_3.jpeg
        ├── GC_4.jpeg
        └── GC_5.jpeg
```

---

## Running Locally

No installation required. Because the site uses `loading="lazy"` and local file paths, open it via a local server rather than directly from the filesystem to avoid CORS issues with images.

**Option 1 — VS Code Live Server extension:**
1. Open the project folder in VS Code
2. Right-click `index.html` → **Open with Live Server**

**Option 2 — Python:**
```bash
cd path/to/portfolio
python -m http.server 8080
```
Then open `http://localhost:8080` in your browser.

**Option 3 — Node.js:**
```bash
npx serve .
```

---

## Deployment (GitHub Pages)

1. Create a new GitHub repository named `tieholara.github.io` (or any repo name for a project page)
2. Push the entire folder contents to the `main` branch — keep the file structure intact
3. Go to **Settings → Pages → Source** and set branch to `main`, folder to `/ (root)`
4. GitHub Pages will publish the site within a few minutes

> **Important:** Do not reorganise files into subdirectories after deployment. All image `src` paths are relative to `index.html` and must stay as-is.

---

## Sections

| # | Section | Description |
|---|---|---|
| 1 | Hero | Headline, availability badge, urgency trigger, CTA buttons, social proof, Three.js particle field |
| 2 | About | Bio, skill bars, achievement stats, CV download, Three.js orbit animation |
| 3 | Projects | 5 projects with real photos, gallery strips, filter tabs, metrics, and live links |
| 4 | Services | 6 service cards with deliverables and quote CTAs |
| 5 | Testimonials | 3 client quotes with star ratings and role attribution |
| 6 | Contact | Working form, contact details, LinkedIn and GitHub links |
| 7 | Footer | Tagline, navigation, social icons, copyright |

---

## Customisation

| What to update | Where |
|---|---|
| Availability status | Hero section — change the badge text |
| Urgency copy | Hero section — `⚡ Only 2 consulting slots…` line |
| Contact form backend | `<form>` `action` attribute — point to Formspree endpoint or Netlify Forms |
| Testimonials | Replace placeholder quotes with real client quotes |
| Project live links | `href` attributes on `View Project →` buttons in the Projects section |
| Brand colours | `:root` CSS custom properties at the top of the `<style>` block |

---

## Related Projects

- **[Lesotho GIS Health Catchments Map](https://laratieho.github.io/Lesotho-GIS-Health-Catchments-Map)** — interactive WebGIS prototype (Leaflet, GitHub Pages)

---

## Contact

- **Email:** [ernesttieo@gmail.com](mailto:ernesttieo@gmail.com)
- **LinkedIn:** [linkedin.com/in/tieholara](https://linkedin.com/in/tieholara)
- **Location:** Maseru District, Lesotho (SAST — UTC+02:00)

---

## Licence

© 2026 Tieho Lara. All rights reserved. This repository is publicly visible for portfolio purposes. Please do not reuse the content, copy, or photographs without permission.
