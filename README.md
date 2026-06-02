# Reliance Legal Services — Website

A modern, responsive one-page website for Reliance Legal Services, built for deployment on GitHub Pages.

---

## Project Structure

```
reliance-legal/
│
├── index.html              # Main entry point — HTML only, no inline styles or scripts
│
├── assets/
│   ├── css/
│   │   └── style.css       # All styles (design tokens, layout, components, animations)
│   ├── js/
│   │   └── script.js       # All JavaScript (nav, scroll reveal, form handling)
│   ├── images/             # Place photos and logos here
│   │   └── (e.g. MA_Khalque_Profile.jpeg)
│   ├── fonts/              # Custom web fonts if self-hosted (.woff2 files)
│   └── media/              # Video or audio files if needed
│
└── README.md               # This file
```

---

## Sections

| Section | Description |
|---|---|
| **Nav** | Fixed top nav with scroll effect; mobile hamburger drawer |
| **Hero** | Full-viewport headline with rotating badge and animated entry |
| **Trust Bar** | Four key statistics (years, cases, satisfaction, recovered) |
| **About** | Firm history and core values grid |
| **Practice Areas** | Six practice area cards with hover effects |
| **Our Team** | Featured owner/partner card + associate grid |
| **File List** | List of available files to download |
| **Buy Documents** | Full Stack Bkash Supported Buying Functionality |
| **Download File** | After Purchase is confirmed, Downlaod the file |
| **Testimonials** | Auto-scrolling infinite marquee (pauses on hover) |
| **CTA Banner** | Gold accent call-to-action strip |
| **Contact** | Contact details + enquiry form |
| **Footer** | Sitemap, practice areas, contact, legal links |

---


## Technology

- **HTML5** — semantic, accessible markup
- **CSS3** — custom properties, Grid, Flexbox, animations (no framework)
- **Vanilla JS** — no dependencies; IntersectionObserver for scroll reveal
- **Google Fonts** — Cormorant Garamond + Jost (loaded via CDN)
