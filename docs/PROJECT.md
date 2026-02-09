# Quentin DIDIER - Consulting Website

## Overview

A simple, elegant single-page consulting website for Quentin DIDIER, a Technical Project Manager & Transformation Lead based in Paris.

**Tagline:** "I help teams debug complex technical and organizational problems"

---

## Decisions Made

| Decision | Choice | Rationale |
|----------|--------|-----------|
| Tech stack | HTML/CSS/JS | Simple, no dependencies, future-proof |
| Hosting | GitHub Pages | Free, hassle-free, reliable |
| Language | English only | Broader reach, simpler |
| Contact | Email + LinkedIn | No backend needed |
| Style | Minimal & clean | Professional, timeless |

---

## Site Structure

### Single Page Sections

1. **Hero** - Name, title, tagline, location
2. **Services** - Two main offerings (brief, compelling)
3. **About** - Short bio establishing credibility
4. **Contact** - Email + LinkedIn links

### Content Strategy

**1. Project & Organizational Consulting**
- Improving decision-making and execution systems
- Diagnosing coordination failures and unclear ownership
- Strategy and prioritization for technical teams

**2. Internal Tools & Software Development**
- Custom internal tools (Notion, Airtable, web apps)
- Workflow automation
- Web development (Next.js, TypeScript)

---

## File Structure

```
Consulting-website/
├── docs/
│   └── PROJECT.md          # Ground truth document
├── index.html              # Main page
├── css/
│   └── style.css           # Styles
├── assets/
│   └── (optional headshot or logo)
├── CNAME                   # (optional) custom domain
└── README.md               # Repo readme
```

---

## Design Direction

**Minimal & Clean:**
- Generous whitespace
- System font stack (fast, native feel)
- Limited color palette: dark text, white background, one accent color
- No animations or fancy effects - content speaks for itself
- Mobile-first responsive design

---

## GitHub Setup Steps

```bash
# 1. Create repo on GitHub
# 2. Initialize local repo
git init
git remote add origin git@github.com:YOUR_USERNAME/consulting-website.git

# 3. After first commit
git push -u origin main

# 4. Enable GitHub Pages
# Settings → Pages → Source: main branch → / (root)
```
