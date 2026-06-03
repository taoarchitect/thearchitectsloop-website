# The Architect’s Loop — Founder Utilities Toolkit

The Architect’s Loop is a small collection of privacy-first browser tools for founders, creators, and small website owners.

The tools are built as simple client-side web pages.

No login.  
No database.  
No tracking on the tools.  
No backend required for tool processing.  
No AI/API cost.

The goal is to create practical utilities that help users think clearly, estimate possibilities, review website readiness, prepare metadata, and convert useful working files.

## Core Philosophy

All public tools under The Architect’s Loop follow this rule:

> User input stays in the browser. Processing happens in the browser. Output stays with the user.

The tools are designed to be:

* privacy-first
* browser-only
* account-free
* database-free
* tracking-free
* lightweight
* export-focused
* practical for real founder work

**TAO** is the only exception and may use a different architecture in the future.

**Optional homepage email signup:** The homepage offers an optional “Notify Me” form. If used, the email address is sent to [Kabak.info](https://kabak.info/) (`tal-notify-me`) for notifications and CSV export. This is separate from the tools — no account is required to use any tool.

## Live Website

https://thearchitectsloop.com/

## This Repository

This GitHub repo is a **backup** of the site source. The live site is hosted on a **custom domain**, not deployed automatically from GitHub.

To update production: upload the site files to your web host (see [Repository structure](#repository-structure)).

For changelog, roadmap, and deployment notes, see `TAL_PROJECT.md`.

## Current Tools

### 1. Ad Revenue Potential Estimator

A browser-based calculator for estimating possible website ad revenue based on:

* monthly traffic
* audience geography
* device mix
* ad placement density
* direct revenue add-ons
* low / realistic / high scenarios

Live tool: https://thearchitectsloop.com/ad-revenue-estimator.html

### 2. Founder Website Visibility Report

A manual website readiness checklist for founders and small website owners.

It helps review:

* search positioning
* title and meta description
* website clarity
* technical readiness
* trust signals
* competitor awareness
* priority next actions

Live tool: https://thearchitectsloop.com/founder-website-visibility-report.html

### 3. Markdown to HTML & PDF Converter

A client-side Markdown converter that allows users to:

* paste Markdown
* upload Markdown files
* preview Markdown
* export HTML
* copy HTML
* download TXT
* copy clean text
* print or save as PDF
* generate a simple local graph view from linked Markdown notes

The graph view detects:

* `[[wikilinks]]`
* `.md` links
* `#tags`

Live tool: https://thearchitectsloop.com/markdown-to-html-pdf-converter.html

### 4. Social Preview & Meta Tag Generator

A client-side tool for creating and previewing social sharing metadata.

It allows users to:

* enter a page title
* enter a meta description
* enter a website URL
* enter an image URL
* preview social link cards
* generate basic HTML meta tags
* generate Open Graph tags
* generate Twitter/X card tags
* copy the generated code

This tool is a manual builder and previewer. It does not scan websites, fetch pages, or collect user data.

Live tool: https://thearchitectsloop.com/social-preview-meta-tag-generator.html

## Practical Guides

The website also includes simple guide pages connected to the tools.

Current guides include:

* How much can a website earn from ads?
* What is RPM in website advertising?
* How many visitors do you need to make money online?
* How to convert Markdown to HTML and PDF

## Free Downloads

Downloadable files (dashboards, spreadsheets, templates) are hosted on Payhip:

https://payhip.com/thearchitectsloop

## Homepage Structure

The homepage is organized as a lean tool directory.

Current categories include:

### Founder Website Tools

* Website Visibility Checker
* Social Preview & Meta Tag Generator
* Robots.txt Builder — Shipping Soon
* Sitemap.xml Builder — Shipping Soon
* SEO Snippet Preview — Shipping Soon

### Monetization Tools

* Ad Revenue Estimator
* Revenue Scenario Planner — Shipping Soon
* Pricing Calculator — Shipping Soon
* Break-Even Calculator — Shipping Soon
* Profit Margin Calculator — Shipping Soon

### Writing & Publishing Tools

* Markdown to HTML/PDF Converter
* YAML Frontmatter Builder — Shipping Soon
* FAQ Schema Generator — Shipping Soon
* Article Schema Generator — Shipping Soon
* Markdown Table Generator — Shipping Soon

### Spreadsheet & Data Tools

* CSV Merger — Shipping Soon
* CSV Cleaner — Shipping Soon
* Duplicate Row Remover — Shipping Soon
* CSV to JSON — Shipping Soon
* JSON to CSV — Shipping Soon

### Knowledge Management Tools

* Obsidian Vault Starter Generator — Shipping Soon
* Note Template Generator — Shipping Soon
* Mermaid Diagram Generator — Shipping Soon
* Frontmatter Builder — Shipping Soon

### Optional updates (homepage)

* **Get New Tool Updates** — optional email signup (Kabak.info), no account required

## Cross-linking

Tool, guide, privacy, and disclaimer pages include a **Related Founder Tools** section before the footer (homepage uses the full directory instead).

## Design Direction

The design is intentionally simple:

* square borders
* minimal colors
* readable layout
* no heavy animation
* no account system
* export-focused tools
* privacy-first messaging
* clear tool categories

The visual style uses:

* paper background
* black ink text
* muted gray secondary text
* blue accent color
* simple utility card layouts

## Tech Stack

This project is intentionally lightweight.

Current stack:

* HTML
* Tailwind CSS via CDN (most pages)
* Vanilla JavaScript
* Static hosting

No build process is required.

For stricter self-contained deployment, Tailwind CSS can be compiled or self-hosted instead of loaded from a CDN.

The Social Preview tool uses standalone CSS with the same visual language.

## Privacy Approach

The tools are designed to run inside the browser.

Current public tools do not require:

* user accounts
* database storage
* server-side file upload
* analytics scripts
* tracking pixels
* programmatic advertising scripts
* AI/API requests

Some pages may load styling assets such as Tailwind CSS from a CDN. User inputs are not submitted to a database or backend by the tools.

The optional homepage email signup sends only an email address to Kabak.info when the user chooses to submit it. Update `privacy.html` when describing this on the live site.

## Repository Structure

Working copy on disk may use a `utility website/` folder. On the web server (and often in this GitHub backup), files typically sit at the **site root**:

```text
/
├── index.html
├── ad-revenue-estimator.html
├── founder-website-visibility-report.html
├── markdown-to-html-pdf-converter.html
├── social-preview-meta-tag-generator.html
├── how-much-can-a-website-earn-from-ads.html
├── what-is-rpm-in-website-advertising.html
├── how-many-visitors-do-you-need-to-make-money-online.html
├── how-to-convert-markdown-to-html-and-pdf.html
├── privacy.html
├── disclaimer.html
├── robots.txt
├── sitemap.xml
├── images/
├── README.md
└── TAL_PROJECT.md
```

## Local Usage

To run locally:

1. Download or clone the repository.
2. Open `index.html` in a browser.
3. Open any tool page directly if needed.

Because this is a static website, no server is required for basic use.

## Deployment

Upload the site files to your static host (custom domain).

The public site is at:

https://thearchitectsloop.com/

After adding new pages, update:

* `index.html`
* `sitemap.xml`
* internal links
* `privacy.html` / `disclaimer.html` if needed
* `README.md` and `TAL_PROJECT.md` in this backup repo

## Project Status

This project is still in early development.

Current focus:

* building small useful tools
* keeping tool logic client-side
* keeping the tools privacy-first
* improving practical guide pages
* improving homepage directory structure
* testing which tools are actually useful for users

## Future Ideas

Future tools must follow the same philosophy:

* privacy-first
* browser-only
* no accounts
* no database
* no tracking
* no AI/API costs

Possible future tools:

* Robots.txt Builder
* Sitemap.xml Builder
* SEO Snippet Preview
* Revenue Scenario Planner
* Pricing Calculator
* Break-Even Calculator
* YAML Frontmatter Builder
* FAQ Schema Generator
* Article Schema Generator
* CSV Merger
* CSV Cleaner
* Obsidian Vault Starter Generator
* Note Template Generator
* Mermaid Diagram Generator

## Contact

The Architect’s Loop  
https://thearchitectsloop.com/

Contact email: [thearchitectsloop@proton.me](mailto:thearchitectsloop@proton.me)

## License

All rights reserved unless otherwise stated.

© 2026 The Architect’s Loop. Built by Tun Bakyu.
