# The Architect's Loop — Project Handoff

**Site:** [thearchitectsloop.com](https://www.thearchitectsloop.com)  
**Local path:** `Digital Products/The Architect's Loop/`  
**Published site files:** `utility website/`  
**Homepage:** `utility website/index.html`

---

## Shipped (live on site today)

### Tools (4) — client-side, no accounts

| Tool | File | Status |
|------|------|--------|
| Website Visibility Checker | `founder-website-visibility-report.html` | **Shipped** |
| Social Preview & Meta Tag Generator | `social-preview-meta-tag-generator.html` | **Shipped** |
| Ad Revenue Potential Estimator | `ad-revenue-estimator.html` | **Shipped** |
| Markdown to HTML & PDF Converter | `markdown-to-html-pdf-converter.html` | **Shipped** |

### Practical guides (4)

| Guide | File | Status |
|-------|------|--------|
| How Much Can a Website Earn From Ads? | `how-much-can-a-website-earn-from-ads.html` | **Shipped** |
| What Is RPM in Website Advertising? | `what-is-rpm-in-website-advertising.html` | **Shipped** |
| How Many Visitors Do You Need to Make Money Online? | `how-many-visitors-do-you-need-to-make-money-online.html` | **Shipped** |
| How to Convert Markdown to HTML and PDF | `how-to-convert-markdown-to-html-and-pdf.html` | **Shipped** |

### Site infrastructure

| Item | Status |
|------|--------|
| Homepage tool directory + roadmap cards | **Shipped** |
| Free Download Library block (Payhip link) | **Shipped** |
| Privacy & Disclaimer pages | **Shipped** |
| Homepage email signup UI (“Notify Me”) | **Shipped** (UI + JS ready) |
| Email signup backend | **Kabak.info** — `https://kabak.info/f/tal-notify-me` (live in `index.html`) |
| Related Founder Tools footer block | **Shipped** on all pages except `index.html` |

### External

| Item | Status |
|------|--------|
| Payhip free downloads | **Live** — [payhip.com/thearchitectsloop](https://payhip.com/thearchitectsloop) |

---

## On the way (listed on homepage, not built yet)

### Founder Website Tools

- Robots.txt Builder
- Sitemap.xml Builder
- SEO Snippet Preview

### Monetization Tools

- Revenue Scenario Planner
- Pricing Calculator
- Break-Even Calculator
- Profit Margin Calculator

### Writing & Publishing Tools

- YAML Frontmatter Builder
- FAQ Schema Generator
- Article Schema Generator
- Markdown Table Generator

### Spreadsheet & Data Tools (whole category)

- CSV Merger
- CSV Cleaner
- Duplicate Row Remover
- CSV to JSON
- JSON to CSV

### Knowledge Management Tools (whole category)

- Obsidian Vault Starter Generator
- Note Template Generator
- Mermaid Diagram Generator
- Frontmatter Builder

---

## Recent changes

### 2026-06-03 — Kabak.info email signup

**Files changed:** `utility website/index.html`

- Form `action` → `https://kabak.info/f/tal-notify-me`
- Hidden `_honey` honeypot for spam protection
- `fetch` posts `FormData(form)` to Kabak; success UI unchanged

### 2026-06-03 — Related tools section (all non-index HTML)

**Pattern:** Matches `social-preview-meta-tag-generator.html` — eyebrow “Related Founder Tools”, heading “Continue the website setup workflow”.

| Page type | Links shown |
|-----------|-------------|
| Tool pages | 3 other tools (current tool excluded) |
| Guides, privacy, disclaimer | All 4 tools |

**Updated files:** `founder-website-visibility-report.html`, `ad-revenue-estimator.html`, `markdown-to-html-pdf-converter.html`, all 4 guide HTML files, `privacy.html`, `disclaimer.html`.  
**Unchanged:** `index.html`, `social-preview-meta-tag-generator.html` (already had section), `googleb70b8ab06061da7b.html` (Google verification only), `original TAL index.html` (archive).

### 2026-06-03 — Homepage email notification signup

- Section **Get New Tool Updates** after Practical Guides, before footer
- Formspree-ready form; `action` URL not set yet
- Vanilla JS: validate email, `fetch` POST when `action` is set

---

## Email signup backend (Notify Me) — Kabak.info

**Provider:** [Kabak.info](https://kabak.info/) — free tier, dashboard, **CSV export**, Telegram alerts optional.

**Status:** Integrated in `utility website/index.html` (vanilla `fetch` + `FormData`, no page reload). Honeypot field `_honey` included per Kabak docs.

### Endpoint

`https://kabak.info/f/tal-notify-me`

### Verify after deploy

1. Submit a test email on the homepage.
2. Confirm it appears in the [Kabak dashboard](https://kabak.info/).
3. Export CSV from dashboard when needed (Telegram alerts optional in Kabak settings).

**Rejected earlier:** Formspree (no CSV on free), Formtorch (150/mo cap).

**Still todo:** Short note in `privacy.html` that optional signups are stored/processed via Kabak.info (third party).

---

## Conventions

- **Homepage / guides:** Tailwind CDN, tokens `ink` / `paper` / `muted` / `accent`, square borders
- **Social Preview tool:** Standalone CSS (same visual language)
- **Related tools:** Before footer; tool pages = 3 links; content/legal pages = 4 links
- **Tools:** Leave tool logic unchanged unless explicitly requested

---

## Next session checklist

- [ ] Test production submit on live site (`tal-notify-me`) and confirm Kabak dashboard entry
- [ ] Update `privacy.html` — optional email signups via Kabak.info
- [ ] Deploy `utility website/` changes to production host

---

*Update this file whenever we change the TAL website or project plan.*
