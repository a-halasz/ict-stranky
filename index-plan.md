# ICT Pro — Landing Page Plan (`index.html`)

## Overview

A modern, professional landing page for ICT Pro (skoleni-ict.cz), a Czech IT training company founded in 1995. The page targets both individual learners and corporate clients looking for IT courses, certifications, and tailored training programmes.

---

## Goals

- Communicate trust and scale (31 years, 2 000+ courses, 2 000+ corporate clients)
- Drive two primary actions: browse courses and contact sales
- Surface the breadth of the course catalogue without overwhelming the visitor
- Work well in both Czech and English (bilingual toggle)

---

## Tech Stack

- Plain HTML5 + CSS3 (no framework dependency for portability)
- Vanilla JS for interactivity (tab switching, mobile menu, language toggle)
- Google Fonts: Inter (body) + Poppins (headings)
- Colour palette: dark charcoal `#1A1A1A`, accent yellow `#F5C400`, highlight yellow `#FFD700`, white `#FFFFFF`, light grey `#F4F6F9`

---

## Page Sections (top to bottom)

### 1. Top Bar
- Left: phone number `+420 517 546 191` and email `skoleni@ictpro.cz`
- Right: language switcher (CZ / EN) + "Zákaznická sekce" login link

### 2. Navigation Header
- Logo: "ictPro ...Strict Professionals" wordmark
- Nav links: Domů · O firmě · ICT Kurzy · Soft Skills · Certifikace · Videokurzy · Kontakt
- CTA button: "Nezávazná poptávka" (Non-binding enquiry) — accent yellow on dark
- Sticky on scroll, collapses to hamburger on mobile

### 3. Hero Section
- Full-width banner (dark charcoal background, subtle geometric pattern with yellow accents)
- Headline: "IT školení a firemní vzdělávání na míru" (IT training tailored to your company)
- Subheadline: short trust statement (e.g. "Pomáháme firmám i jednotlivcům růst od roku 1995.")
- Two CTA buttons: "Prozkoumat kurzy" (primary) · "Kontaktovat nás" (secondary/outline)
- Animated stats strip below headline: 31 let · 12 učeben · 2 000+ kurzů · 400+ lektorů · 2 000+ firemních klientů · 10 000+ účastníků za rok

### 4. Course Category Grid
- Section title: "Školení podle kategorií"
- 4-column grid (2 on tablet, 1 on mobile) of category cards
- Each card: icon + category name + 3–4 top subcategory links
- Categories (12 total):
  1. Microsoft 365 & Office
  2. Microsoft (Server, Azure, Dynamics)
  3. Programování (Python, Java, .NET…)
  4. Databáze (SQL, Oracle, PostgreSQL…)
  5. Virtualizace a Cloud (VMware, AWS, Azure…)
  6. Bezpečnost (Kyberbezpečnost, GDPR…)
  7. Umělá Inteligence (ChatGPT, Copilot, Claude…)
  8. Networking (Cisco, Fortinet, MikroTik…)
  9. Unixové systémy (Linux, FreeBSD…)
  10. Grafika (Adobe, CAD, 3D…)
  11. IBM
  12. Specializovaná školení
- "Zobrazit všechny kurzy →" link at bottom

### 5. Why ICT Pro — Trust Strip
- 3-column layout with icons:
  - **Autorizovaná centra** — official partner of Microsoft, Cisco, VMware, IBM, etc.
  - **Zkušení lektoři** — 400+ certified instructors, practitioners not just teachers
  - **Flexibilní výuka** — onsite, online, blended, on-demand video

### 6. New Courses Highlight
- Section title: "Nová školení v naší nabídce"
- Horizontal scrollable card row (or 3-column grid)
- Each card: course code badge, course name, short description, "Více informací →" link
- Pulls from the newest additions (e.g. VIBE Coding, AI v Excelu, 3D grafika…)

### 7. Guaranteed Dates (Garantované termíny)
- Section title: "Nejbližší garantované termíny"
- Tabbed or filterable list: All · Microsoft · AI · Programování · Bezpečnost
- Each row: date range, course name, location badge (Praha / Brno / Online)
- "Zobrazit kompletní přehled →" link

### 8. Special Offers (Akční nabídka)
- Section title: "Akční nabídka"
- 3-card row showing discounted courses
- Each card: course name, original price struck through, discounted price in accent yellow, date, "Přihlásit se" CTA button

### 9. Corporate Training CTA Banner
- Full-width dark charcoal banner with yellow accent stripe or border
- Headline: "Školíme celé týmy. Na míru, ve vašich prostorách nebo online."
- Short body text about tailored corporate programmes
- CTA button: "Nezávazná poptávka pro firmy" — yellow button, dark text

### 10. Testimonials / Social Proof (optional v1)
- 3 quote cards from corporate clients
- Client logo strip below (Microsoft, Cisco, VMware, IBM, Adobe, Check Point…)

### 11. Certifications & Partners Strip
- Horizontal logo row of official authorised partner badges
- Short copy: "Jsme autorizovaným školicím centrem předních světových technologií."

### 12. Contact Footer
- Left column: address (Brno + Praha), phone, email, social icons (LinkedIn, Facebook)
- Middle column: quick links (O firmě, Kurzy, Certifikace, Kontakt, GDPR)
- Right column: newsletter signup or "Zavoláme vám" mini-form (name + phone + submit)
- Bottom bar: © ICT Pro s.r.o. + legal links

---

## Responsive Behaviour

| Breakpoint | Layout notes |
|---|---|
| ≥1200px | Full desktop — 4-col category grid, full nav |
| 768–1199px | Tablet — 2-col category grid, condensed nav |
| <768px | Mobile — 1-col stack, hamburger menu, stat strip scrolls horizontally |

---

## Key Content Decisions

- **Language:** Czech primary; EN switcher changes static text (JS-driven, no server needed for v1)
- **Images:** hero uses CSS gradient overlay; course category cards use SVG icons (no stock photos needed initially)
- **Performance:** no heavy frameworks; lazy-load any images; minify CSS/JS before shipping
- **SEO:** semantic HTML5 landmarks (`<header>`, `<main>`, `<section>`, `<footer>`), `<meta>` description + keywords matching existing site, structured data (`Organization`, `Course`) via JSON-LD

---

## File Structure

```
index.html          ← this file (landing page)
css/
  style.css         ← main stylesheet
  responsive.css    ← media queries
js/
  main.js           ← nav toggle, language switch, tabs
img/
  logo.svg
  hero-bg.jpg
  icons/            ← category SVG icons
```

---

## Next Steps

1. Build `index.html` skeleton with all sections stubbed out
2. Write `css/style.css` (design tokens, layout, components)
3. Add JS interactivity (hamburger, language toggle, course tab filter)
4. Populate real course data (hardcoded for v1, API-driven later)
5. Test across Chrome, Firefox, Safari — mobile + desktop
6. Validate HTML (W3C) and run Lighthouse audit (target: Performance ≥90, Accessibility ≥95)
