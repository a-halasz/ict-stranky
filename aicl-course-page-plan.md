# AICL Course Page Plan — `kurz-aicl.html`

## Overview

A dedicated course detail page for **"Claude – jak používat AI jako užitečný pracovní nástroj (AICL)"**, sitting within the ICT Pro site. The page must convert a visitor who already has intent (they clicked through from the category or a campaign) into a course enquiry or private booking request. It should inherit the full visual identity from `index.html` (same top bar, sticky nav, footer) and feel like a natural extension of the site.

**Source course URL:** `https://www.skoleni-ict.cz/kurz/Claude-jak-pouzivat-AI-jako-uzitecny-pracovni-nastroj-AICL.aspx`

> ⚠️ **Key difference from CLVC:** This course is offered **only as private/customised training** — there are no guaranteed public dates. The booking flow therefore leads to a custom-training enquiry form, not a direct date-selection checkout.

---

## Goals

- Drive enquiries via the "Školení na míru" / custom-training request form
- Communicate that **no technical or programming knowledge is required** — remove the single biggest objection for non-technical audiences
- Clearly explain the practical, day-to-day work focus (emails, summaries, analysis, text preparation) so visitors self-qualify quickly
- Build trust through outcomes and the practical structure of the curriculum
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
- Breadcrumb added below nav: `Domů → Kategorie kurzů → Umělá Inteligence → Claude → AICL`

### 2. Course Hero / Header
- Two-column layout: left content, right booking card (sticky on desktop scroll)
- **Left:**
  - Category breadcrumb trail (with yellow `>` separators)
  - Course code badge: `AICL` (dark charcoal background, yellow text — monospace)
  - H1: **"Claude – jak používat AI jako užitečný pracovní nástroj"**
  - Short intro paragraph (from the source page):
    > "AI dnes dokáže výrazně urychlit běžnou práci — od psaní textů a zpracování podkladů až po shrnování informací a přípravu návrhů. Aby ale AI skutečně pomáhala, nestačí ji jen „zkusit". Je potřeba vědět, jak jí zadávat úkoly, jak vyhodnotit výstup a jak ji používat bezpečně."
  - Trust badges row: `2 dny` · `Pouze privátní výuka` · `Žádné tech. znalosti` · `Certifikát`
- **Right (sticky booking card):**
  - Prominent label: **"Kurz pouze na míru"** (charcoal background, yellow accent)
  - Sub-text: "Termíny a cenu přizpůsobíme vašim potřebám — pro firmy i jednotlivce."
  - Primary CTA: **"Nezávazně poptat →"** (yellow button) — links to `https://www.skoleni-ict.cz/Objednavka_kurzu_na_miru.aspx?K=AICL`
  - Secondary: **"Napsat dotaz"** (outline button) — mailto: `skoleni@ictpro.cz`
  - Small note: "Dostupné prezenčně v učebně i online (hybridní formát)"

### 3. "Co se naučíte" — Learning Outcomes
- Section title: **"Co se naučíte"** / "What you'll learn"
- 2-column grid of outcome cards (icon + bold headline + 1-line description)
- 7 items drawn from the source page:
  1. 🧠 Praktická práce s Claude — Osvojíte si postupy, které fungují v reálných situacích
  2. ✍️ Lepší výstupy z AI — Naučíte se zadávat úkoly tak, aby dávaly použitelné výsledky
  3. ⚡ Rychlejší příprava textů — E-maily, zápisky, podklady a návrhy za zlomek času
  4. 📄 Shrnutí a přehled informací — Zpracování delších textů, rešerší a strukturování dat
  5. ✅ Kontrola kvality výstupů — Získáte návyky pro ověřování a finální kontrolu AI odpovědí
  6. 🛡️ Bezpečné používání AI — Pochopíte, jaká data nevkládat a jak postupovat zodpovědně
  7. ⚖️ Právní a etický přehled — Základní orientace v AI Actu, autorském právu a odpovědnosti

### 4. Pro koho je kurz určen — Target Audience
- Section title: **"Pro koho je kurz určen"** / "Who should attend"
- 6 persona tiles in a horizontal row (icon + role title + one-liner)
  1. 🖥️ Běžní uživatelé — Chtějí AI používat systematicky, ne jen náhodně
  2. 🗂️ Administrativa a HR — Zpracování dokumentů, korespondence a podkladů
  3. 📣 Marketing a obchod — Tvorba textů, konceptů a komunikačních materiálů
  4. 📋 Projektoví manažeři — Příprava zápisů, shrnutí a podkladů pro rozhodnutí
  5. 👔 Vedoucí pracovníci — Efektivnější využití AI pro sebe i tým
  6. 💡 Podnikatelé a freelanceři — Zrychlení každodenní agendy pomocí AI
- Below: bold callout box — **"Žádné technické ani programátorské znalosti nejsou potřeba."** (charcoal bg, yellow accent left border)

### 5. Obsah kurzu — Course Curriculum
- Section title: **"Obsah kurzu"** / "Course programme"
- 7 accordion modules (closed by default, click to expand), ordered as on the source page:
  1. Kde AI v praxi opravdu pomáhá
  2. Zadávání úkolů v Claude: jak získat lepší výstupy
  3. Texty a dokumenty s využitím Claude
  4. Práce s informacemi: shrnutí, struktura, přehled
  5. Kreativní podpora a návrhová práce s AI
  6. Bezpečnost, pravidla a odpovědnost při používání AI
  7. Jak AI zapojit do vlastní práce dlouhodobě
- Each module: module number badge (yellow on charcoal) + title + sub-bullet list revealed on expand
- Module count strip above accordion: **7 modulů · 2 dny · 16 hodin výuky**

**Sub-topics per module (for the accordion expand):**

1. **Kde AI v praxi opravdu pomáhá**
   - Co je generativní AI z pohledu běžného uživatele
   - Jaké úkoly AI zvládá dobře a kde je potřeba opatrnost
   - Typické příklady využití v pracovním prostředí
   - Jak poznat, kdy AI dává smysl a kdy ne
   - Role nástroje Claude v každodenní práci s textem a informacemi

2. **Zadávání úkolů v Claude: jak získat lepší výstupy**
   - Jak formulovat zadání podle cíle a kontextu
   - Co má obsahovat dobré zadání (účel, vstup, výstup, forma)
   - Jak si řídit styl, délku a strukturu odpovědi
   - Jak Claude vést krok po kroku k lepšímu výsledku
   - Jak pracovat s upřesněním, opravou a iterací
   - Praktické cvičení na přepis nejasných zadání do kvalitních promptů

3. **Texty a dokumenty s využitím Claude**
   - Psaní e-mailů, zpráv, zápisů, shrnutí a návrhů textů
   - Tvorba osnovy, argumentace a variant výstupu
   - Úprava stylu textu podle cílové skupiny (formální, stručný, obchodní, srozumitelný)
   - Jak si pomocí AI připravit podklady pro prezentaci nebo meeting
   - Revize a finální kontrola výstupu před použitím
   - Praktický trénink na běžných pracovních situacích

4. **Práce s informacemi: shrnutí, struktura, přehled**
   - Jak využít Claude pro rychlé pochopení tématu
   - Shrnutí delších textů a vytěžení podstatných bodů
   - Třídění a strukturování informací do přehledné podoby
   - Porovnání variant a příprava podkladů pro rozhodnutí
   - Jak rozpoznat slabá místa AI odpovědi a co ověřovat
   - Cvičení zaměřená na praktickou analýzu vstupů

5. **Kreativní podpora a návrhová práce s AI**
   - Jak využít Claude při brainstormingu a generování nápadů
   - Tvorba konceptů, variant a návrhů řešení
   - Příprava textových podkladů pro marketing a komunikaci
   - Jak kombinovat AI s vlastním know-how, aby výsledek nebyl generický
   - Kde jsou limity AI při kreativní práci
   - Praktické ukázky využití v různých typech rolí

6. **Bezpečnost, pravidla a odpovědnost při používání AI**
   - Jaká data do AI nevkládat a proč
   - Práce s interními, osobními a citlivými informacemi
   - Odpovědnost za obsah výstupu a finální rozhodnutí
   - Zásady bezpečného používání AI ve firemním prostředí
   - Základní orientace: autorské právo, licence, AI Act
   - Praktická doporučení pro každodenní bezpečné používání

7. **Jak AI zapojit do vlastní práce dlouhodobě**
   - Výběr prvních use-caseů s rychlým přínosem
   - Jak si nastavit jednoduché workflow s Claude
   - Šablony zadání pro opakující se činnosti
   - Jak měřit přínos (čas, kvalita, konzistence výstupu)
   - Závěrečné procvičení na vlastních scénářích účastníků
   - Doporučení pro další samostatný rozvoj

### 6. Co si z kurzu odnesete — Takeaways
- Section title: **"Co si z kurzu odnesete"** / "Your takeaways"
- 5-item icon grid (ideally 3 + 2 or 2 × 3):
  1. ✅ Použitelné postupy pro každodenní práci s Claude
  2. ✍️ Šablony zadání pro opakující se úkoly (e-maily, zápisy, shrnutí)
  3. ⚙️ Jednoduchý workflow: jak Claude zapojit do vlastní práce
  4. 🛡️ Pravidla bezpečného používání AI ve firmě
  5. 🎓 Certifikát o absolvování

### 7. Forma výuky a termíny — Format & Booking
- Section title: **"Forma výuky"** / "Format & booking"
- **No fixed public dates** — clearly communicate this so the visitor isn't left confused
- Two format cards side by side:
  - 🏫 **Prezenčně v učebně** — V ICT Pro učebně nebo u vás ve firmě
  - 💻 **Online (virtuálně)** — Hybridní formát, odkaz na [více informací](https://www.skoleni-ict.cz/slu_virtualpro.aspx)
- Wide CTA card (charcoal bg, yellow button):
  - Heading: **"Nezávazná poptávka školení na míru"**
  - Body: "Kurz přizpůsobíme termínu, rozsahu i počtu účastníků. Kontaktujte nás a připravíme nabídku."
  - Primary CTA: **"Poptat školení →"** — `https://www.skoleni-ict.cz/Objednavka_kurzu_na_miru.aspx?K=AICL`
  - Contact strip: 📧 `skoleni@ictpro.cz` · 📞 `+420 517 546 191`

### 8. Předpoklady a logistika — Prerequisites & Logistics
- Two-column info strip:
  - **Předpokládané znalosti:** Základní práce s počítačem a internetem. Žádné technické ani programátorské znalosti nejsou potřeba.
  - **Časový rozvrh:** 2 dny, 9:00 – 17:00 hod.
  - **Forma výuky:** Prezenčně nebo online (hybridní — upřesněte při poptávce)
  - **Cena:** Na základě poptávky — přizpůsobena počtu účastníků a rozsahu
  - **Kód kurzu:** AICL
  - **Certifikát:** Ano — vydán po absolvování

### 9. Sociální důkaz / Reference — Social Proof
- Section title: **"Co říkají účastníci"** / "What attendees say"
- Placeholder for 3 testimonial cards (styled as quote cards matching `index.html`)
  - Note: No testimonials available from the source page — use placeholders and fill with real quotes
- Below: small partner logo strip (same as `index.html` section 11)

### 10. Mohlo by vás zajímat — Related Courses
- Section title: **"Mohlo by vás zajímat"** / "You might also like"
- 3-card row of related courses (category: Umělá Inteligence / Claude):
  - Claude AI – vibe coding a tvorba aplikací bez programování (CLVC)
  - ChatGPT – efektivní využití pro praxi
  - AI pro firmy – strategie a implementace
- Each card: course code badge · name · 1-line description · "Více informací →" link

### 11. Shared Footer
- Identical to `index.html` — copy verbatim
- Active link in the footer quick-links column: "ICT Kurzy" → highlighted with yellow underline

---

## Sticky Booking Card (desktop behaviour)

The right-column booking card (introduced in Section 2) sticks to the top of the viewport as the user scrolls, until the footer is reached. Because there are no public dates, the card remains static (no date selector). On mobile it collapses to a fixed bottom bar showing:
- "Školení na míru" + "Poptat →" button (full width)

---

## Responsive Behaviour

| Breakpoint | Hero layout | Booking card | Curriculum |
|---|---|---|---|
| ≥ 1100px | 2-column (content + sticky card) | Sticky right column | Accordion |
| 768–1099px | 1-column, card below hero content | Static, full-width | Accordion |
| < 768px | 1-column | Fixed bottom bar | Accordion (full width) |

---

## Key Content Decisions

- **No technical knowledge assumption:** repeated in hero, audience section, and prerequisites — same conversion lever as CLVC, but even more prominent here given the non-technical target audience
- **Private-only clarity:** the page must never imply public dates exist; replace every "Objednat" CTA with "Poptat" or "Nezávazně poptat" to reflect the enquiry-first booking flow
- **Practical focus:** all copy emphasises real work tasks (emails, summaries, decisions) rather than technical AI concepts — this differentiates AICL from the more technical CLVC course
- **Hybrid note:** both in-person and online options mentioned on the booking card and format section
- **Price:** listed as "na základě poptávky" — do not show a fixed price since the source page doesn't publish one; instead emphasise flexibility
- **Language toggle:** inherits CZ/EN from `index.html`; all section titles and CTAs have both language variants via `data-lang` / `inline-cs` / `inline-en` pattern
- **No external dependencies added:** pure HTML/CSS/JS, consistent with `index.html`

---

## Differences from `kurz-clvc.html`

| Feature | CLVC | AICL |
|---|---|---|
| Course code | CLVC | AICL |
| Public dates | Yes (4 scheduled dates) | No — private only |
| Primary CTA | "Objednat kurz →" | "Nezávazně poptat →" |
| Price shown | 9 800 Kč bez DPH | "Na základě poptávky" |
| Sticky card content | Nearest date + price | "Kurz na míru" + enquiry CTA |
| Mobile bottom bar | Date + price + Objednat | "Školení na míru" + Poptat |
| Dates & booking table | Yes (card per date) | No — replaced by Format section |
| Tool/licence callout | Yes (Claude Code access) | Not applicable |
| Curriculum modules | 9 | 7 |
| Target audience | Mixed (incl. developers) | Non-technical / office workers |

---

## File Structure

```
index.html                  ← existing landing page
kurz-clvc.html              ← CLVC course detail page
kurz-aicl.html              ← this new course detail page (AICL)
css/
  style.css                 ← (future) shared tokens extracted from all pages
js/
  main.js                   ← (future) shared JS (language toggle, hamburger)
img/
  logo.svg
  icons/
```

---

## Next Steps

1. Build `kurz-aicl.html` skeleton — shared top bar, nav, footer from `index.html`
2. Implement 2-column hero with sticky "Kurz na míru" booking card
3. Build learning outcomes grid (Section 3)
4. Build target audience persona tiles (Section 4)
5. Build accordion curriculum (Section 5) with JS expand/collapse — 7 modules
6. Build format & booking section (Section 7) — no date table, enquiry CTA instead
7. Wire up sticky card mobile → fixed bottom bar behaviour
8. Add bilingual toggle support throughout (CZ/EN)
9. Cross-browser test (Chrome, Firefox, Safari) at all three breakpoints
10. Validate HTML (W3C) · Lighthouse audit (Performance ≥ 90, Accessibility ≥ 95)
