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
| **Testimonials** | Auto-scrolling infinite marquee (pauses on hover) |
| **CTA Banner** | Gold accent call-to-action strip |
| **Contact** | Contact details + enquiry form |
| **Footer** | Sitemap, practice areas, contact, legal links |

---

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `reliance-legal`).
2. Push all files, keeping the folder structure exactly as shown above.
3. Go to **Settings → Pages**.
4. Under **Source**, select `Deploy from a branch` → `main` → `/ (root)`.
5. Save. Your site will be live at `https://<your-username>.github.io/reliance-legal/`.

---

## Adding the Owner's Photo

In `index.html`, find the comment inside the owner card:

```html
<!--
  Replace the SVG below with an <img> tag pointing to the actual photo:
  <img src="assets/images/MA_Khalque_Profile.jpeg" alt="M. A. Khaleque"
       style="width:100%;height:100%;object-fit:cover;" />
-->
```

1. Copy `MA_Khalque_Profile.jpeg` (or any photo) into `assets/images/`.
2. Remove the SVG placeholder and uncomment the `<img>` tag.
3. Also remove the `avatar-circle lg` wrapper `<div>` — it constrains the image to a circle. Replace the whole `.owner-photo-placeholder` block with just the `<img>` tag for a full-bleed photo.

---

## Customisation Checklist

- [ ] Replace firm name, tagline, and established year in `index.html`
- [ ] Update phone numbers and email address
- [ ] Update office address in Contact section and Footer
- [ ] Add owner photo to `assets/images/` and update the HTML (see above)
- [ ] Update owner bio, credentials, and role
- [ ] Add associate photos and update employee cards
- [ ] Replace placeholder statistics in Trust Bar with real figures
- [ ] Replace placeholder testimonials with real client quotes
- [ ] Update `<meta>` description and OG tags at the top of `index.html`

---

## Technology

- **HTML5** — semantic, accessible markup
- **CSS3** — custom properties, Grid, Flexbox, animations (no framework)
- **Vanilla JS** — no dependencies; IntersectionObserver for scroll reveal
- **Google Fonts** — Cormorant Garamond + Jost (loaded via CDN)
