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

- [ ] **2.1** Test responsiveness on mobile
  - [ ] Check content box layout on narrow screens
  - [ ] Verify text sizes are readable on phone
  - [ ] Test touch targets (buttons) are large enough
  - [ ] Check background image behavior on mobile (may need adjustment)

- [ ] **2.2** Ensure text remains readable
  - [ ] Check color contrast ratios meet WCAG AA (4.5:1 for body text)
  - [ ] Verify line lengths aren't too long/short
  - [ ] Ensure sufficient spacing between elements

- [x] **2.3** Optimize map image file size for fast loading
  - Before: **36MB**, 10643x4998px
  - After: **472KB**, 1800x845px (98.7% reduction!)
  - Subtasks:
    - [x] Resize to 1800px width
    - [x] Compress with quality 75%
    - [x] Test visual quality after compression

- [ ] **2.4** Final commit and deploy

---

### 3. Custom Domain Setup

- [x] **3.1** Purchase domain (quentin-didier.com on Cloudflare)
- [x] **3.2** Configure DNS (A records + CNAME for www)
- [x] **3.3** Add CNAME file to repository
- [x] **3.4** Enable HTTPS in GitHub Pages settings

#### Domain Purchase Instructions

**Recommended registrar:** [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/) - at-cost pricing, no markup, includes free DNS and SSL.

**Steps:**

1. **Create Cloudflare account** at cloudflare.com (free)

2. **Search for your domain** at dash.cloudflare.com → Domain Registration → Register Domain
   - Try: `quentindidier.com`, `quentindidier.fr`, or `qdidier.com`
   - `.com` typically costs ~$10/year
   - `.fr` requires being in EU (you qualify, being in France)

3. **Purchase the domain** - follow checkout process

4. **Configure DNS for GitHub Pages** - In Cloudflare DNS settings, add:
   ```
   Type: CNAME
   Name: @
   Target: tangrenin.github.io
   ```
   And for www:
   ```
   Type: CNAME
   Name: www
   Target: tangrenin.github.io
   ```

5. **Add CNAME file to repo** - Create a file called `CNAME` (no extension) containing just:
   ```
   quentindidier.com
   ```
   (replace with your actual domain)

6. **Enable in GitHub Pages** - Settings → Pages → Custom domain → enter your domain → Save

7. **Wait for DNS propagation** (can take up to 24h, usually faster)

8. **Enable HTTPS** - Once DNS propagates, check "Enforce HTTPS" in GitHub Pages settings

**Alternative registrars:**
- Namecheap - good prices, easy interface
- Google Domains - simple, integrates with Google services
- OVH - good for .fr domains, French company

---

## Reference

**Inspiration:** [simonsarris.com](https://simonsarris.com/)

**Assets:**
- `assets/Cantino_planisphere_(1502).jpg` (selected background)
- `assets/France_cotes_academie.png` (backup option)
