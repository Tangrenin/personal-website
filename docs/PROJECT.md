# Quentin Didier - Personal Website

## Overview

A minimal personal website for Quentin Didier at quentin-didier.com. Three pages: home, writing, and projects.

---

## Decisions

| Decision | Choice | Rationale |
|----------|--------|-----------|
| Tech stack | HTML/CSS | Simple, no dependencies, future-proof |
| Hosting | GitHub Pages | Free, reliable |
| Language | English | Broader reach |
| Style | Antique map background, warm paper content box, serif headings | Distinctive, timeless |

---

## Pages

1. **Home** (`/`) — Name, nav, brief intro
2. **Writing** (`/writing/`) — List of written pieces (currently placeholder)
3. **Projects** (`/projects/`) — List of projects (currently placeholder)

All pages share the same layout: hero with name link, nav bar, page content, footer with email and copyright.

---

## File Structure

```
personal-website/
├── index.html              # Home page
├── writing/
│   └── index.html          # Writing listing page
├── projects/
│   └── index.html          # Projects listing page
├── css/
│   └── style.css           # Styles
├── assets/
│   ├── Cantino_planisphere_(1502).jpg  # Background image
│   └── Q_icon.png          # Favicon
├── docs/
│   └── PROJECT.md          # This file
├── CNAME                   # Custom domain config
└── README.md               # Repo readme
```

---

## Design

- Antique map background image (fixed, covers viewport)
- Centered paper-colored content box with subtle border and shadow
- Sorts Mill Goudy serif for headings, Source Sans 3 for body
- Warm color palette: paper (#f5f0e8), dark text (#2c2416), saddle-brown accent (#8b4513)
- Responsive: content box fills width on mobile, map scrolls naturally on iOS
