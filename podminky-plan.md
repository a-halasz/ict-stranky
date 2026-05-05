# ICT Pro — Podmínky užívání (`podminky.html`)

## Overview

A clean, readable legal/terms-of-use page for ICT Pro (skoleni-ict.cz). Matches the visual identity of the main landing page — same nav, same footer, same colour palette and typography. Bilingual (CZ/EN toggle). No heavy interactivity needed; content is the focus.

---

## Goals

- Provide legally required terms of use in a clear, structured format
- Match the look and feel of the rest of the site (shared nav + footer)
- Be easy to scan with a sticky table of contents on desktop
- Link back to from the footer legal links on `index.html`

---

## Tech Stack

- Same as `index.html`: plain HTML5 + CSS3, vanilla JS
- No additional dependencies
- Reuse existing CSS variables and component styles from the main page

---

## Page Sections (top to bottom)

### 1. Top Bar
- Identical to `index.html` — phone, email, language switcher

### 2. Navigation Header
- Identical to `index.html` — logo, nav links, CTA button

### 3. Page Hero (minimal)
- Dark charcoal background, no image
- Headline: "Podmínky užívání" / "Terms of Use"
- Subline: "Platné od 1. ledna 2024" / "Effective from 1 January 2024"
- No CTA buttons — this is a legal page

### 4. Content Area (two-column on desktop)

**Left column — sticky Table of Contents**
- Numbered list of section anchors
- Highlights the active section on scroll (JS IntersectionObserver)
- Collapses/hides on mobile

**Right column — article body**
Sections (each with an `id` anchor):

1. **Úvodní ustanovení / Introduction**
   - Who operates the site (ICT Pro s.r.o., IČO, sídlo)
   - Scope of these terms

2. **Používání webových stránek / Use of the website**
   - Permitted use
   - Prohibited conduct (scraping, misuse, impersonation)

3. **Duševní vlastnictví / Intellectual property**
   - All content © ICT Pro s.r.o.
   - Logos, course materials, texts
   - No reproduction without written consent

4. **Ochrana osobních údajů / Personal data**
   - Reference to full Privacy Policy (GDPR page — separate)
   - Brief: data collected only for enquiry/enrolment purposes
   - Contact for data requests: skoleni@ictpro.cz

5. **Odpovědnost / Liability**
   - Site provided "as is"
   - ICT Pro not liable for third-party links or temporary unavailability

6. **Cookies**
   - Types used: necessary, analytical
   - User can manage via browser settings
   - No third-party ad cookies

7. **Změny podmínek / Changes to these terms**
   - ICT Pro reserves the right to update
   - Continued use = acceptance of updated terms
   - Changes announced on this page with updated effective date

8. **Rozhodné právo / Governing law**
   - Czech law applies
   - Disputes resolved before Czech courts (jurisdiction: Brno)

9. **Kontakt / Contact**
   - ICT Pro s.r.o.
   - Příkop 843/4, 602 00 Brno
   - skoleni@ictpro.cz
   - +420 517 546 191

### 5. Footer
- Identical to `index.html`

---

## Responsive Behaviour

| Breakpoint | Layout notes |
|---|---|
| ≥1024px | Two-column: sticky TOC left (250px), article right |
| 768–1023px | Single column, TOC collapses to a dropdown at top |
| <768px | Single column, TOC hidden, article full width |

---

## Key Content Decisions

- **Language:** Czech primary, EN toggle same as rest of site
- **Tone:** Clear and plain — avoid dense legal jargon; use short paragraphs
- **Length:** Target 800–1 200 words of body text (enough to be credible, not overwhelming)
- **Anchors:** Each section gets an `id` so the TOC links and external deep-links work
- **Last updated date:** Displayed prominently below the headline

---

## File Structure

```
podminky.html       ← this file (terms of use page)
index.html          ← links to podminky.html from footer legal strip
```

---

## Next Steps

1. Build `podminky.html` reusing nav + footer markup from `index.html`
2. Write all 9 content sections in both CZ and EN
3. Implement sticky TOC with IntersectionObserver for active-state highlighting
4. Update footer legal links in `index.html`, `kurz-aicl.html`, and `kurz-clvc.html` to point to `podminky.html`
5. Test bilingual toggle, mobile layout, and all anchor links
6. Validate HTML (W3C) and check Lighthouse accessibility score
