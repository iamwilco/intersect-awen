# Intersect Community Hubs · 2025 Post-Mortem

A single-page summary of the **2025 Community Hubs programme** — the six regional hubs (AWEN, LATAM, Japan, Sri Lanka, WADA, Clay Nation) that ran from May 2024 to June 2025 under Intersect's Membership &amp; Community Committee.

This page consolidates the full post-mortem into a legible entry point with every cost figure disclosed, every milestone accounted for, and every community concern answered directly — while linking back to the full document and primary sources.

Styled to match Intersect's visual language: Cardano blue, IBM Plex, numbered sections, document-quality layout.

---

## What's on the page

1. **Announcement bar** — report status
2. **Hero** — headline narrative plus four stats (6 hubs, 173 events, 49/49 milestones, 2,395 members)
3. **Status card** — version plus six-figure cost grid ($176K USD · 264,616 ADA · $128.90 per member · $982 per event · 70% in-region · 15,436 ADA returned)
4. **§ 01 Paths** — five ways to read the report
5. **§ 02 Funding** — complete program funding table (Phase 1 · AMM · Phase 2 bridge) across all six hubs with sourced citations
6. **§ 03 ROI** — cost efficiency by hub, six program-wide stat cards, detailed Japan benchmark with category breakdown
7. **§ 04 The six hubs** — per-hub cards (region, manager where public, contract, events, members, three highlights each, deep-link to the full hub section)
8. **§ 05 Caveats** — how to read the numbers (duration, local cost structure, sub-hub structure, snapshot lag, no single winner)
9. **§ 06 Deliverables** — contract delivery table (6 requirements, all delivered) plus six beyond-scope outcome cards
10. **§ 07 FAQ** — eight community concerns across three groups (financial accountability, ROI, governance &amp; process)
11. **§ 08 Resources** — twelve deep-link cards to every source (archived contracts, Japan spreadsheet, Cardanoscan, Dev Updates, KB pages)
12. **Footer** — matches intersectmbo.org structure

Every external link points to real, existing public records. Zero content migration required.

---

## Source content

Derived from **[Awen-online/intersect_mcc](https://github.com/Awen-online/intersect_mcc)** — specifically `hub_report.html` v1.6 (April 2026). The original document remains the authoritative source; this page is a navigable summary with receipts.

---

## Design alignment

- **Primary color**: Cardano blue (`#0033AD`) — ecosystem convention
- **Accent semantics**: green for *delivered/ok*, blue for *info*, orange for *highest* — used consistently in tables and stat cards
- **Typography**: IBM Plex Sans + IBM Plex Mono (for numbers) + IBM Plex Serif (caveat numerals only)
- **Tone**: formal, transparent, specific — no hedging, no PR
- **Layout**: sharp corners (4px), generous whitespace, grid-based, no decorative ornament
- **Sections numbered** `§ 01 · Paths` through `§ 08 · Resources` — reinforces document-quality feel

---

## Deployment

### GitHub Pages (zero config)
This repo ships with a GitHub Actions workflow at `.github/workflows/deploy.yml` that publishes `index.html` on every push to `main`.

1. Fork or clone.
2. Repo **Settings → Pages → Source: GitHub Actions**.
3. Push to `main` — the workflow deploys to `https://<user>.github.io/<repo>/` within about a minute.

No build step, no dependencies, one external request (Google Fonts).

### Any other static host
Single HTML file. Drop on Netlify, Vercel, Cloudflare Pages, or S3 and it works as-is.

---

## Accessibility &amp; performance

- Semantic HTML (`<section>`, `<header>`, `<nav>`, `<footer>`, `<details>` for the FAQ)
- Responsive down to 320px
- No JavaScript required for core functionality
- Sticky header for long-scroll navigation
- WCAG AA color contrast on text
- Single HTML file, one external request, no framework, no build pipeline

---

## What this page deliberately does NOT do

- It is **not a 2026 budget proposal** — that lives separately in `mcc_budget_2026.html` in the source repo.
- It does not replace the full post-mortem document — it summarizes and links to it.
- It does not reinterpret or re-score any figure — every number is sourced exactly as published by the underlying records.

---

## Credits

Community summary page drafted by Wilco van de Burgwal (W3i Software), using content from `Awen-online/intersect_mcc` maintained by Intersect's Membership &amp; Community Committee.

Design language shared with the sibling `intersect-budget` hub proposal: Cardano blue, IBM Plex, numbered sections.

Free to use, modify, fork, or discard as the MCC sees fit.

---

## License

Released under MIT.
