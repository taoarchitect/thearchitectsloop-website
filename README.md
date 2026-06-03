# The Architect’s Loop — Founder Utilities Toolkit

The Architect’s Loop is a privacy-first collection of browser tools for founders, creators, and small website owners.

Built as static HTML pages: **no login**, **no database**, **no tracking on the tools**, **no server-side processing** for tool use, **no AI/API cost** on the public toolkit.

**Live site:** https://thearchitectsloop.com/

---

## This repository

| Purpose | Details |
|---------|---------|
| **GitHub** | Backup of site source and documentation |
| **Production** | Custom domain — upload `utility website/` to your host (not deployed from GitHub automatically) |
| **Handoff doc** | See [`TAL_PROJECT.md`](TAL_PROJECT.md) for full file list, changelog, deploy checklists, Kabak setup |

### What to commit

```
README.md                 ← this file
TAL_PROJECT.md            ← project handoff / changelog
utility website/          ← entire site (HTML, robots.txt, sitemap.xml, images/)
```

Optional: mirror `utility website/*` at repo root if that matches your hosting layout — see [Repository structure](#repository-structure).

### Suggested commit message

```
Complete TAL v1: 15 tools, combined workbenches, Kabak signup, docs

- Ship all homepage tools; CSV Workbench uses local file upload
- Related Founder Tools on all inner pages
- Update sitemap, privacy, disclaimer, README, TAL_PROJECT.md
```

---

## Core philosophy

> User input stays in the browser. Processing happens in the browser. Output stays with the user.

* Privacy-first, account-free, export-focused  
* **TAO** is a separate product and may use a different architecture later  
* **Optional homepage signup:** “Notify Me” sends email to [Kabak.info](https://kabak.info/) (`tal-notify-me`) only if the user submits — not required for any tool  

---

## Toolkit overview (15 tools)

### Founder Website Tools (6)

| # | Tool | URL |
|---|------|-----|
| 1 | Website Visibility Checker | [/founder-website-visibility-report.html](https://thearchitectsloop.com/founder-website-visibility-report.html) |
| 2 | Social Preview & Meta Tag Generator | [/social-preview-meta-tag-generator.html](https://thearchitectsloop.com/social-preview-meta-tag-generator.html) |
| 3 | UTM Link Builder | [/utm-link-builder.html](https://thearchitectsloop.com/utm-link-builder.html) |
| 4 | Robots.txt Builder | [/robots-txt-builder.html](https://thearchitectsloop.com/robots-txt-builder.html) |
| 5 | Sitemap.xml Builder | [/sitemap-xml-builder.html](https://thearchitectsloop.com/sitemap-xml-builder.html) |
| 6 | SEO Snippet Preview | [/seo-snippet-preview.html](https://thearchitectsloop.com/seo-snippet-preview.html) |

### Monetization Tools (2)

| # | Tool | URL |
|---|------|-----|
| 7 | Ad Revenue Potential Estimator | [/ad-revenue-estimator.html](https://thearchitectsloop.com/ad-revenue-estimator.html) |
| 8 | Founder Business Math | [/business-math-calculators.html](https://thearchitectsloop.com/business-math-calculators.html) |

*Business Math combines: pricing, break-even, profit margin, revenue scenarios.*

### Writing & Publishing Tools (5)

| # | Tool | URL |
|---|------|-----|
| 9 | Markdown to HTML & PDF Converter | [/markdown-to-html-pdf-converter.html](https://thearchitectsloop.com/markdown-to-html-pdf-converter.html) |
| 10 | YAML Frontmatter Builder | [/frontmatter-builder.html](https://thearchitectsloop.com/frontmatter-builder.html) |
| 11 | FAQ Schema Generator | [/faq-schema-generator.html](https://thearchitectsloop.com/faq-schema-generator.html) |
| 12 | Article Schema Generator | [/article-schema-generator.html](https://thearchitectsloop.com/article-schema-generator.html) |
| 13 | Markdown Table Generator | [/markdown-table-generator.html](https://thearchitectsloop.com/markdown-table-generator.html) |

### Spreadsheet & Data Tools (1)

| # | Tool | URL |
|---|------|-----|
| 14 | CSV Workbench | [/csv-workbench.html](https://thearchitectsloop.com/csv-workbench.html) |

*Upload `.csv` files (and `.json` for JSON→CSV) in the browser. Merge, clean, dedupe, convert — files are not uploaded to The Architect’s Loop servers.*

### Knowledge Management Tools (1)

| # | Tool | URL |
|---|------|-----|
| 15 | Obsidian & Notes Toolkit | [/obsidian-toolkit.html](https://thearchitectsloop.com/obsidian-toolkit.html) |

*Vault starter downloads, note templates, Mermaid diagram preview.*

---

## Practical guides (4)

* [How much can a website earn from ads?](https://thearchitectsloop.com/how-much-can-a-website-earn-from-ads.html)
* [What is RPM in website advertising?](https://thearchitectsloop.com/what-is-rpm-in-website-advertising.html)
* [How many visitors do you need to make money online?](https://thearchitectsloop.com/how-many-visitors-do-you-need-to-make-money-online.html)
* [How to convert Markdown to HTML and PDF](https://thearchitectsloop.com/how-to-convert-markdown-to-html-and-pdf.html)

---

## Free downloads

Payhip library: https://payhip.com/thearchitectsloop

---

## Cross-linking & homepage

* **Homepage** (`index.html`): full tool directory — **15 Tools Available**, no “Shipping Soon”
* **Inner pages:** “Related Founder Tools” section before the footer (tools, guides, privacy, disclaimer)
* **Email signup:** optional block on homepage (Kabak)

---

## Tech stack

* HTML + vanilla JavaScript  
* Tailwind CSS via CDN (most pages)  
* Social Preview: standalone CSS (same visual language)  
* Obsidian toolkit: Mermaid via jsDelivr (preview only)  
* No build step required  

---

## Privacy (summary)

* Tools process data in the browser  
* Markdown and CSV tools read files locally (File API)  
* No analytics or ad scripts on toolkit pages  
* Optional email signup uses Kabak.info (see `privacy.html` on the live site)  
* Tailwind / Mermaid CDNs may receive normal HTTP request metadata  

Full policy: https://thearchitectsloop.com/privacy.html

---

## Repository structure

**Source of truth on disk:**

```text
The Architect's Loop/
├── README.md
├── TAL_PROJECT.md
└── utility website/
    ├── index.html
    ├── *.html              (tools + guides + legal)
    ├── robots.txt
    ├── sitemap.xml
    └── images/
```

**On the web server**, files usually live at the **site root** (same names as inside `utility website/`).

---

## Local usage

1. Clone or download this repo  
2. Open `utility website/index.html` in a browser  
3. No local server required  

---

## Deployment

1. Upload `utility website/` contents to production host  
2. Keep GitHub in sync for backup (`README.md`, `TAL_PROJECT.md`, site files)  

After changes, update `sitemap.xml` and legal pages when relevant.

---

## Project status

**TAL toolkit v1 is complete** — all homepage-listed tools are live.

**Next:** TAO development; optional TAL maintenance (guides, assets, self-hosted CSS).

Details and changelog: [`TAL_PROJECT.md`](TAL_PROJECT.md)

---

## Contact

* Site: https://thearchitectsloop.com/  
* Email: [thearchitectsloop@proton.me](mailto:thearchitectsloop@proton.me)

© 2026 The Architect’s Loop. Built by Tun Bakyu.
