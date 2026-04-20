# Intersect MCC — Hub page

A single-page hub for Intersect's **Membership &amp; Community Committee (MCC)**. Consolidates the 2026 budget proposal, the 2025 community-hubs post-mortem, the committee's remit, and the community FAQ into one legible entry point — without moving or duplicating any of the upstream content.

Styled to match Intersect's visual language: Cardano blue, IBM Plex, numbered sections, document-quality layout.

---

## What's on the page

1. **Announcement bar** — working-draft status for the 2026 budget
2. **Hero** — MCC mission plus four headline stats (2026 budget, 2025 hubs, events delivered, membership reach)
3. **Status card** — current MCC state with total budget plus a seven-figure cost grid across WP 01–07
4. **Paths** — five entry points (2026 proposal, 2025 post-mortem, about MCC, FAQ, join)
5. **About the MCC** — mission and five core values (inclusivity, empowerment, transparency, collaboration, sustainability)
6. **2026 budget** — all seven work packages ($300K total) plus the accountability clause
7. **2025 hubs** — the six regional hubs with contract values, periods, and milestone counts
8. **Findings** — six ROI/outcome findings from the post-mortem
9. **Participants** — MCC, hub operators, community, DReps — who does what
10. **FAQ** — nine community questions across three groups (financial accountability, ROI, governance &amp; process)
11. **Resources** — twelve deep-link cards to every authoritative source
12. **Footer** — matches intersectmbo.org structure

Every external link points to real, existing Intersect, GitHub, or Google Doc pages. Zero content migration required.

---

## Source repo

Content sourced from **[Awen-online/intersect_mcc](https://github.com/Awen-online/intersect_mcc)** — specifically `mcc_budget_2026.html` (v1.4, March 2026) and `hub_report.html` (v1.6, April 2026). This hub page summarizes and links to both; the original documents remain the authoritative sources.

---

## Design alignment

- **Primary color**: Cardano blue (`#0033AD`) — matches Intersect's ecosystem identity
- **Accent**: warm `#B85A25` (draft) for working-draft status, green for "live," amber for "upcoming"
- **Typography**: IBM Plex Sans + IBM Plex Mono + IBM Plex Serif (for numerals only)
- **Tone**: formal, structured, transparent — mirrors Intersect copy conventions
- **Layout**: sharp corners (4px), generous whitespace, grid-based, no decorative ornament
- **Sections numbered** `§ 01 · Paths` through `§ 08 · Resources` — reinforces the document-quality feel

---

## Deployment

### Quick start — GitHub Pages (zero config)
This repo ships with a GitHub Actions workflow at `.github/workflows/deploy.yml` that publishes `index.html` to GitHub Pages on every push to `main`.

1. Fork or clone this repo.
2. In the repo settings → **Pages** → set **Source** to *GitHub Actions*.
3. Push to `main`. The workflow deploys the site to `https://<user>.github.io/<repo>/`.

No build step, no dependencies.

### Alternative — any static host
This is a single HTML file with one external request (Google Fonts, preconnected). Drop `index.html` on Netlify, Vercel, Cloudflare Pages, or S3 and it works.

### Alternative — port to Next.js
If you want to integrate into a larger Intersect property, the page decomposes cleanly into components (`<Announcement>`, `<Header>`, `<Hero>`, `<StatusCard>`, `<Paths>`, `<Pillars>`, `<WorkPackages>`, `<HubsTable>`, `<Findings>`, `<Roles>`, `<FAQ>`, `<Resources>`, `<Footer>`). All CSS uses standard custom properties and can slot into any theme system.

---

## Accessibility &amp; performance

- Semantic HTML (`<section>`, `<header>`, `<nav>`, `<footer>`, `<details>` for FAQ)
- Responsive down to 320px
- No JavaScript required for core functionality (FAQ uses native `<details>`)
- Sticky header for long-scroll navigation
- Sufficient color contrast throughout (WCAG AA minimum on all text)
- Single HTML file, one external request, no framework, no build pipeline

---

## Maintenance

Copy blocks that change per cycle:

| Block | Update when | Effort |
|---|---|---|
| Announcement bar | Draft → submitted → approved | 1 line |
| Hero stats | Once per cycle | 4 values |
| Status card (version, dates) | Minor revisions | 1 block |
| Work packages | Once per cycle | 7 blocks |
| Hubs table | New hub / contract period | Add row |
| Findings grid | Once per cycle | 6 blocks |
| FAQ | As questions accumulate | Append `<details>` |
| Resources | As new documents publish | Add card |

Most cycle-over-cycle updates are copy edits, no structural changes needed.

---

## What this page deliberately does NOT do

- It does not move any upstream content. Every link points to the existing page on github.com, Intersect docs, Google Docs, or members.intersectmbo.org.
- It does not replace the full 2026 proposal or the post-mortem document — it summarizes and links to both.
- It does not make funding decisions or vote on behalf of DReps — those happen on-chain through the 2026 Cardano budget process.

---

## Credits

Community hub page drafted by Wilco van de Burgwal (W3i Software), using content from Intersect's MCC and the original `Awen-online/intersect_mcc` repository maintained by the Membership &amp; Community Committee.

Design language borrowed from the sibling `intersect-budget` hub proposal: Cardano blue, IBM Plex, numbered sections, document-quality layout.

Free to use, modify, fork, or discard as the MCC sees fit.

---

## License

Released under MIT. Do what you want with it.
