# Website Improvements Plan

## Overview
Redesign the consulting website with a warmer, more personal aesthetic inspired by [simonsarris.com](https://simonsarris.com/), featuring an antique map background and a centered paper-like content box.

---

## Decisions Made

| Question | Decision |
|----------|----------|
| Background map | Cantino planisphere (warm colors, aged parchment) |
| Typography | Serif for headings |
| Domain | quentin-didier.com (Cloudflare) |

---

## Tasks

### 1. Redesign Implementation

- [x] **1.1** Set Cantino planisphere as fixed full-page background
- [x] **1.2** Create centered content container with paper/cream background
  - Scrolls independently from fixed background
  - Max-width constraint for readability
  - Subtle shadow for depth
- [x] **1.3** Unify all section backgrounds to same cream/paper color
- [x] **1.4** Switch to serif font for headings (Libre Baskerville)
- [x] **1.5** Reduce name size (less prominent h1)
- [x] **1.6** Change "DIDIER" to "Didier" (remove all-caps)
- [x] **1.7** Adjust text and button colors to complement warm palette

---

### 2. Final Polish

- [x] **2.1** Test responsiveness on mobile
  - [x] Check content box layout on narrow screens
  - [x] Verify text sizes are readable on phone
  - [x] Test touch targets (buttons) - increased to 44px min height
  - [x] Fix background image on iOS (disabled `background-attachment: fixed` on mobile)

- [x] **2.2** Ensure text remains readable
  - [x] Improve color contrast - darkened muted text (#5c5347 → #4a453c)
  - [x] Line lengths constrained by max-width
  - [x] Increased button font size and padding

- [x] **2.3** Optimize map image file size for fast loading
  - Before: **36MB**, 10643x4998px
  - After: **472KB**, 1800x845px (98.7% reduction!)
  - Subtasks:
    - [x] Resize to 1800px width
    - [x] Compress with quality 75%
    - [x] Test visual quality after compression

- [x] **2.4** Final commit and deploy

---

### 3. Custom Domain Setup

- [x] **3.1** Purchase domain (quentin-didier.com on Cloudflare)
- [x] **3.2** Configure DNS (A records + CNAME for www)
- [x] **3.3** Add CNAME file to repository
- [x] **3.4** Enable HTTPS in GitHub Pages settings

## Reference

**Inspiration:** 
- [simonsarris.com](https://simonsarris.com/)
- [https://ulyssepence.com/](https://ulyssepence.com/)

**Assets:**
- `assets/Cantino_planisphere_(1502).jpg` (selected background)
- `assets/France_cotes_academie.png` (backup option)
