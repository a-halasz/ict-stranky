# CLVC Course Page Plan — `kurz-clvc.html`

## Overview

A dedicated course detail page for **"Claude AI – vibe coding a tvorba aplikací bez programování (CLVC)"**, sitting within the ICT Pro site. The page must convert a visitor who already has intent (they clicked through from the category or a campaign) into a course registration. It should inherit the full visual identity from `index.html` (same top bar, sticky nav, footer) and feel like a natural extension of the site.

**Source course URL:** `https://www.skoleni-ict.cz/kurz/Claude-AI-vibe-coding-a-tvorba-aplikaci-bez-programovani-CLVC.aspx`

---

## Goals

- Drive registrations via the "Objednat" booking flow
- Communicate that **no programming knowledge is required** — remove the single biggest objection
- Surface all available dates and locations clearly so the visitor can commit immediately
- Build trust through outcomes, outputs, and social proof
- Support the bilingual CZ/EN toggle inherited from `index.html`

---

## Tech Stack

Identical to `index.html`:
- Plain HTML5 + CSS3, no framework
- Vanilla JS (shared language toggle, hamburger, accordion)
- Google Fonts: Inter (body) + Poppins (headings)
- Colour palette: `#1A1A1A` charcoal · `#F5C400` yellow · `#FFFFFF` white · `#F4F6F9` light grey
- Copy `<style>` design tokens and shared components from `index.html` to keep the files in sync; extract to `css/style.css` when the site grows beyond 3 pages

---

## Page Sections (top to bottom)

### 1. Shared Top Bar & Nav
- Identical to `index.html` — copy verbatim
- Breadcrumb added below nav: `Domů → Kategorie kurzů → Umělá Inteligence → Claude → CLVC`

### 2. Course Hero / Header
- Two-column layout: left content, right booking card (sticky on desktop scroll)
- **Left:**
  - Category breadcrumb trail (with yellow `>` separators)
  - Course code badge: `CLVC` (dark charcoal background, yellow text — monospace)
  - H1: **"Claude AI – vibe coding a tvorba aplikací bez programování"**
  - Short intro paragraph (2–3 sentences from the source page — the "Představujeme Claude..." text)
  - Trust badges row: `2 dny` · `9 800 Kč bez DPH` · `Žádné programování` · `Certifikát`
- **Right (sticky booking card):**
  - Nearest available date highlighted: Praha · 4. 5. – 5. 5. 2026
  - Price: `9 800 Kč` (bez DPH) / `11 858 Kč` (s DPH)
  - Primary CTA: **"Objednat kurz →"** (yellow button)
  - Secondary: **"Školení na míru"** (outline button)
  - Small note: "Nebo se připojte online — uveďte do poznámky"

### 3. "Toto školení vám pomůže" — Learning Outcomes
- Section title: **"Co se naučíte"** / "What you'll learn"
- 2-column grid of outcome cards (icon + bold headline + 1-line description)
- 8 items drawn from the bullet list on the source page:
  1. 🧠 Možnosti a limity AI — Pochopíte, kdy AI pomůže a kdy selže
  2. ⚙️ Personalizace Claude — Memory, Skills, Projects nastavené pro vás
  3. 🌐 Vlastní webová stránka — Bez jediného řádku kódu, publikovaná online
  4. 🚀 Publikace na GitHub Pages — Web dostupný na internetu zdarma
  5. 🤖 Automatizace s GitHub Actions — Skripty, které pracují za vás
  6. 💬 Techniky promptování — Chain of thought, few-shot, role prompting
  7. 🛡️ Etika a bezpečnost AI — Co Claude vidí, ukládá, a jak odpovídat za výstupy
  8. ✅ Kdy AI použít a kdy NE — Praktická rozhodovací kritéria

### 4. For Whom — Target Audience
- Section title: **"Pro koho je kurz určen"** / "Who should attend"
- 5 persona tiles in a horizontal row (icon + role title + one-liner)
  1. 📊 Analytici a datoví pracovníci
  2. 📣 Marketingoví pracovníci
  3. 📋 Projektoví manažeři
  4. 🗂️ HR a administrativa
  5. 💡 Kdokoli, kdo chce tvořit
- Below: bold callout box — **"Žádné programátorské znalosti nejsou potřeba."** (charcoal bg, yellow accent left border)

### 5. Course Curriculum / Programme
- Section title: **"Obsah kurzu"** / "Course programme"
- 9 accordion modules (closed by default, click to expand), ordered as on the source page:
  1. Úvod do AI a Claude
  2. Efektivní promptování
  3. Personalizace Claude
  4. Claude Chat vs Claude Code
  5. GitHub a verzování
  6. Praktický projekt: Vlastní web
  7. Interaktivní aplikace
  8. Automatizace s GitHub Actions
  9. Etika a bezpečnost AI
- Each module: module number badge (yellow on charcoal) + title + sub-bullet list revealed on expand
- Module count strip above accordion: **9 modulů · 2 dny · 16 hodin výuky**

### 6. Course Outputs — What You Take Away
- Section title: **"Co si z kurzu odnesete"** / "Your takeaways"
- 6-item icon grid (3 × 2):
  1. ✅ Nastavený Claude účet (Memory, Skills, Projects)
  2. 🌐 Vlastní web na GitHub Pages
  3. 🖥️ Interaktivní nástroj (kalkulačka / formulář)
  4. ⚙️ Automatizační skript (GitHub Actions + Python)
  5. 💬 Prompt šablony pro běžné situace
  6. 🎓 Certifikát o absolvování

### 7. Dates & Locations — Booking Table
- Section title: **"Termíny a místa konání"** / "Dates & locations"
- Card-based layout (one card per date block), sorted chronologically:

  | Datum | Lokalita | Cena | CTA |
  |---|---|---|---|
  | 4. 5. – 5. 5. 2026 | Praha + online | 9 800 Kč | Objednat |
  | 2. 6. – 3. 6. 2026 | Brno + online | 9 800 Kč | Objednat |
  | 15. 6. – 16. 6. 2026 | Praha + online | 9 800 Kč | Objednat |
  | 21. 9. – 22. 9. 2026 | Praha + online | 9 800 Kč | Objednat |

- Each card: date (bold) · location badge (Praha blue / Brno green / Online purple) · price · "Objednat →" yellow button
- "Školení na míru" wide card below the grid — charcoal bg, yellow outline button

### 8. Tool Access Callout
- Narrow full-width banner (light yellow background `#FFFBEB`, yellow left border)
- Icon: 🔑
- Text (from source): "V průběhu školení budeme využívat **naše placené licence** — každý účastník získá přístup ke Claude Code na dobu výuky + 1 týden po skončení kurzu."
- Sub-note: "Pokud již účet máte, předem si jej aktivujte a ušetříme čas."

### 9. Prerequisites & Logistics
- Two-column info strip:
  - **Předpokládané znalosti:** Základní práce s počítačem a internetem. Žádné programátorské znalosti nejsou potřeba.
  - **Časový rozvrh:** 2 dny, 9:00 – 17:00 hod.
  - **Forma výuky:** Prezenčně nebo online (hybridní — uveďte do poznámky)
  - **Cena:** 9 800 Kč bez DPH / 11 858 Kč s DPH
  - **Kód kurzu:** CLVC
  - **Certifikát:** ano — vydán po absolvování

### 10. Social Proof / Reference
- Section title: **"Co říkají účastníci"** / "What attendees say"
- Displayed reference: Ministerstvo pro místní rozvoj, Karel H. — styled as a quote card (matching the style from `index.html` testimonials section)
- Placeholder for 2 further testimonial cards (to be filled with real quotes)
- Below: small partner logo strip (same as `index.html` section 11)

### 11. Related Courses
- Section title: **"Mohlo by vás zajímat"** / "You might also like"
- 3-card row of related courses (category: Umělá Inteligence / Claude):
  - AI v Excelu a Microsoft 365 Copilot
  - ChatGPT – efektivní využití pro praxi
  - VIBE Coding s pomocí AI nástrojů (generic)
- Each card: course code badge · name · 1-line description · "Více informací →" link

### 12. Shared Footer
- Identical to `index.html` — copy verbatim
- Active link in the footer quick-links column: "ICT Kurzy" → highlighted with yellow underline

---

## Sticky Booking Card (desktop behaviour)

The right-column booking card (introduced in Section 2) sticks to the top of the viewport as the user scrolls, until the footer is reached. On mobile it collapses to a fixed bottom bar showing:
- "Praha · 4. 5." + price + "Objednat →" button (full width)

---

## Responsive Behaviour

| Breakpoint | Hero layout | Booking card | Curriculum |
|---|---|---|---|
| ≥ 1100px | 2-column (content + sticky card) | Sticky right column | Accordion |
| 768–1099px | 1-column, card below hero content | Static, full-width | Accordion |
| < 768px | 1-column | Fixed bottom bar | Accordion (full width) |

---

## Key Content Decisions

- **No programming assumption:** repeated in hero, audience section, and prerequisites — this is the single biggest conversion lever
- **Hybrid note:** "Připojte se online" mentioned in the booking card and every date card — mirrors the original site UX
- **Price clarity:** always show both ex-VAT and inc-VAT figures next to each other
- **Language toggle:** inherits CZ/EN from `index.html`; all section titles and CTAs have both language variants via `data-lang` / `inline-cs` / `inline-en` pattern
- **No external dependencies added:** pure HTML/CSS/JS, consistent with `index.html`

---

## File Structure

```
index.html                  ← existing landing page
kurz-clvc.html              ← this new course detail page
css/
  style.css                 ← (future) shared tokens extracted from both pages
js/
  main.js                   ← (future) shared JS (language toggle, hamburger)
img/
  logo.svg
  icons/
```

---

## Next Steps

1. Build `kurz-clvc.html` skeleton — shared top bar, nav, footer from `index.html`
2. Implement 2-column hero with sticky booking card
3. Build learning outcomes grid (Section 3)
4. Build accordion curriculum (Section 5) with JS expand/collapse
5. Build dates & booking cards (Section 7)
6. Wire up sticky card mobile → fixed bottom bar behaviour
7. Add bilingual toggle support throughout (CZ/EN)
8. Cross-browser test (Chrome, Firefox, Safari) at all three breakpoints
9. Validate HTML (W3C) · Lighthouse audit (Performance ≥ 90, Accessibility ≥ 95)
