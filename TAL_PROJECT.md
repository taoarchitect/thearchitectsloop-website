# The Architect's Loop — Project Handoff

**Site:** [thearchitectsloop.com](https://www.thearchitectsloop.com)  
**Local path:** `Digital Products/The Architect's Loop/`  
**Published site files:** `utility website/` (upload contents to web host root)  
**GitHub:** backup of site source + these docs  
**Status:** **TAL toolkit v1 complete** — ready to focus on **TAO**

**Last doc update:** 3 June 2026

---

## Quick reference

| | |
|---|---|
| Live tools | **15** |
| Guides | **4** |
| Homepage | `utility website/index.html` |
| **Lead job (marketing)** | Founder site audit → [visibility report](https://thearchitectsloop.com/founder-website-visibility-report.html) |
| **Catalog** | 14 other tools linked from homepage directory |
| Email signup | Kabak — `https://kabak.info/f/tal-notify-me` |
| Related tools block | All tool, guide, and legal pages (not homepage) |
| **Flagship (planned)** | **TAO** — feasibility report from Lean Canvas case (client-side) |

---

## Positioning (June 2026)

Reddit feedback: **“Founder toolkit” is too broad** — lead with one repeat job; browser-only is trust, not the headline.

| Layer | What |
|-------|------|
| **Pitch (TAL interim)** | Run a founder site audit before launch or pitch |
| **Primary CTA** | `founder-website-visibility-report.html` |
| **Directory** | All 15 tools remain on homepage |
| **Future pitch (TAO)** | Turn idea + Lean Canvas into a feasibility report — client-side, store nothing |

### Homepage copy (`index.html`)

- **Title:** Run a founder site audit in your browser \| The Architect's Loop
- **H1:** Run a founder site audit in 15 minutes
- **Eyebrow:** Before you launch or pitch
- **Hero CTA:** Start the visibility checklist
- **Nav tagline:** Free tools · Browser only

---

## Shipped tools (15)

### Founder Website Tools (6)

| Tool | File |
|------|------|
| Website Visibility Checker | `founder-website-visibility-report.html` |
| Social Preview & Meta Tag Generator | `social-preview-meta-tag-generator.html` |
| UTM Link Builder | `utm-link-builder.html` |
| Robots.txt Builder | `robots-txt-builder.html` |
| Sitemap.xml Builder | `sitemap-xml-builder.html` |
| SEO Snippet Preview | `seo-snippet-preview.html` |

### Monetization Tools (2)

| Tool | File | Notes |
|------|------|--------|
| Ad Revenue Potential Estimator | `ad-revenue-estimator.html` | Standalone |
| Founder Business Math | `business-math-calculators.html` | **Combined:** Pricing, Break-Even, Profit Margin, Revenue Scenarios |

### Writing & Publishing Tools (5)

| Tool | File | Notes |
|------|------|--------|
| Markdown to HTML & PDF Converter | `markdown-to-html-pdf-converter.html` | File upload for `.md` |
| YAML Frontmatter Builder | `frontmatter-builder.html` | **Combined:** YAML + Frontmatter Builder |
| FAQ Schema Generator | `faq-schema-generator.html` | |
| Article Schema Generator | `article-schema-generator.html` | |
| Markdown Table Generator | `markdown-table-generator.html` | Paste or build rows |

### Spreadsheet & Data Tools (1)

| Tool | File | Notes |
|------|------|--------|
| CSV Workbench | `csv-workbench.html` | **Combined:** Merger, Cleaner, Dedupe, CSV↔JSON. **Upload** `.csv` / `.json` via File API (local only) |

### Knowledge Management Tools (1)

| Tool | File | Notes |
|------|------|--------|
| Obsidian & Notes Toolkit | `obsidian-toolkit.html` | **Combined:** Vault starter downloads, note templates, Mermaid preview (jsDelivr CDN) |

---

## Guides (4)

| Guide | File |
|-------|------|
| How Much Can a Website Earn From Ads? | `how-much-can-a-website-earn-from-ads.html` |
| What Is RPM in Website Advertising? | `what-is-rpm-in-website-advertising.html` |
| How Many Visitors Do You Need to Make Money Online? | `how-many-visitors-do-you-need-to-make-money-online.html` |
| How to Convert Markdown to HTML and PDF | `how-to-convert-markdown-to-html-and-pdf.html` |

---

## All public HTML files (`utility website/`)

```
index.html
ad-revenue-estimator.html
article-schema-generator.html
business-math-calculators.html
csv-workbench.html
disclaimer.html
faq-schema-generator.html
founder-website-visibility-report.html
frontmatter-builder.html
how-much-can-a-website-earn-from-ads.html
how-many-visitors-do-you-need-to-make-money-online.html
how-to-convert-markdown-to-html-and-pdf.html
markdown-table-generator.html
markdown-to-html-pdf-converter.html
obsidian-toolkit.html
privacy.html
robots-txt-builder.html
seo-snippet-preview.html
sitemap-xml-builder.html
social-preview-meta-tag-generator.html
utm-link-builder.html
what-is-rpm-in-website-advertising.html
```

Also: `robots.txt`, `sitemap.xml`, `images/` (favicon, etc.)

**Not for production:** `original TAL index.html`, `googleb70b8ab06061da7b.html` (verification only)

---

## Combined tools (index duplicates merged)

| Original homepage “Shipping Soon” items | Shipped as |
|----------------------------------------|------------|
| Revenue Scenario Planner, Pricing, Break-Even, Profit Margin | `business-math-calculators.html` |
| YAML Frontmatter Builder + Frontmatter Builder | `frontmatter-builder.html` |
| CSV Merger, Cleaner, Duplicate Row Remover, CSV to JSON, JSON to CSV | `csv-workbench.html` |
| Obsidian Vault Starter, Note Templates, Mermaid, Frontmatter (KM) | `obsidian-toolkit.html` |

---

## Site infrastructure

| Item | Status |
|------|--------|
| Homepage — 15 tools, no “Shipping Soon” | Done |
| Optional email signup (Kabak) | `tal-notify-me` on `#tal-notify-form` |
| Related Founder Tools (before footer) | All tools, guides, `privacy.html`, `disclaimer.html` |
| `sitemap.xml` | 22 URLs, `lastmod` 2026-06-03 |
| `robots.txt` | `Sitemap: https://thearchitectsloop.com/sitemap.xml` |
| `privacy.html` / `disclaimer.html` | Updated for full toolkit, Kabak, file uploads |
| Payhip downloads | [payhip.com/thearchitectsloop](https://payhip.com/thearchitectsloop) |

---

## Deployment

| Target | How |
|--------|-----|
| **Production** | Upload `utility website/` files to custom domain document root |
| **GitHub** | Commit `utility website/` + `README.md` + `TAL_PROJECT.md` (backup) |

Production is **not** auto-deployed from GitHub.

### Pending Google Search Console indexing (quota hit 2026-06-03)

Request indexing tomorrow for these URLs only (others done for today):

- https://thearchitectsloop.com/csv-workbench.html
- https://thearchitectsloop.com/obsidian-toolkit.html
- https://thearchitectsloop.com/how-much-can-a-website-earn-from-ads.html
- https://thearchitectsloop.com/what-is-rpm-in-website-advertising.html
- https://thearchitectsloop.com/how-many-visitors-do-you-need-to-make-money-online.html
- https://thearchitectsloop.com/how-to-convert-markdown-to-html-and-pdf.html
- https://thearchitectsloop.com/privacy.html
- https://thearchitectsloop.com/disclaimer.html

### Production checklist (host)

- [ ] Upload full `utility website/` (or sync changed files since last deploy)
- [ ] Test homepage Kabak signup on live URL
- [ ] Test CSV Workbench with a real `.csv` upload
- [ ] Optional: resubmit `sitemap.xml` in Google Search Console

### GitHub backup checklist

- [ ] Commit all files under `utility website/`
- [ ] Commit `README.md` and `TAL_PROJECT.md`
- [ ] Do not commit secrets (none required for static site)

**Suggested commit message:**

```
Complete TAL v1: 15 tools, combined workbenches, Kabak signup, docs

- Ship all homepage tools (SEO, business math, publishing, CSV, Obsidian)
- CSV Workbench: local file upload via File API
- Related Founder Tools on all inner pages
- Update sitemap, privacy, disclaimer, README, TAL_PROJECT.md
```

---

## Email signup (Kabak)

- **Endpoint:** `https://kabak.info/f/tal-notify-me`
- **Form:** `utility website/index.html` → `#tal-notify-form`
- **Backend:** Kabak.info (third party); optional CSV export in Kabak dashboard
- Formspree was considered; not used (CSV export on free tier)

---

## Conventions

- Static HTML; Tailwind CDN on most pages; Social Preview uses standalone CSS
- Vanilla JavaScript only on tools and homepage signup
- Tool data stays in browser; files read with **File API** (Markdown, CSV) — not sent to TAL servers
- Exception: optional homepage email → Kabak only

---

## Changelog

### 2026-06-03 — Homepage positioning (job-first pitch)

- Hero: visibility audit as lead job; toolkit as directory below
- Meta title/description and OG/Twitter aligned
- Primary CTA to `founder-website-visibility-report.html`
- About section reframed as “after the audit”
- Docs: `README.md`, `TAL_PROJECT.md` (this file)

### 2026-06-03 — Related tools + CSV upload fix

- Related Founder Tools added to all new tool pages that lacked it
- CSV Workbench: primary UX is **upload CSV/JSON files**, not paste-only

### 2026-06-03 — TAL toolkit v1 complete

- 10 new tool pages; homepage 15 tools; no Shipping Soon
- Full `sitemap.xml`; legal pages updated

### 2026-06-03 — UTM Link Builder + Kabak signup

- `utm-link-builder.html`; homepage notify form wired to Kabak

---

## Next work

| Track | Notes |
|-------|--------|
| **TAO** | Separate product; different architecture (see TAO workspace) |
| **TAL maintenance** | New guides, Payhip assets, self-hosted Tailwind; revisit lead job if analytics favor another tool |
| **TAO launch** | Replace interim audit pitch on main brand when TAO client-side ships |

---

*Update this file whenever the live site or GitHub backup changes.*
