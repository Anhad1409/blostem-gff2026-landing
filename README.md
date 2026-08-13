# Blostem at Global Fintech Fest 2026 — Exhibitor Landing Page

Single-file, self-contained landing page for Blostem's presence at **Global Fintech Fest 2026**.

- **Booth:** J18 & J20, Pavilion Hall (stacked bays)
- **Dates:** 9–11 September 2026
- **Venue:** Jio World Centre, Mumbai

## Contents

| File | Notes |
| --- | --- |
| `index.html` | The entire page — markup, CSS, JS and all imagery inlined as data URIs (~9.7 MB). No build step, no asset folder. |

Google Fonts (Plus Jakarta Sans, JetBrains Mono, Playfair Display) are loaded from
`fonts.googleapis.com`, so the page needs a network connection to render with its
intended typography; everything else works offline.

## Viewing locally

Open `index.html` directly in a browser, or serve the folder:

```sh
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

The repo is already shaped for any static host — `index.html` sits at the root, so
GitHub Pages, Netlify, Cloudflare Pages or Vercel will serve it with no configuration.

## Page structure

Alternating dark ↔ light sections, per the Blostem brand rhythm:

1. Hero — co-brand, booth number, Pavilion Hall shot, countdown *(dark)*
2. GFF scale stats band, using GFF 2025 published figures *(dark)*
3. Showcase — six products, one SDK *(light)*
4. VoiceBrew.AI spotlight *(cream)*
5. Jaano spotlight *(light)*
6. About Blostem — team photo, partner and backer logo rows *(light)*
7. The stall — fabrication render, zone callouts, locator *(dark)*
8. At the booth — agenda, same across all three days *(light)*
9. GFF 2025 rewind gallery — Blostem's own booth photos *(dark)*
10. Book a meeting — form *(light)*
11. Venue and footer *(dark)*

## Known TODOs

- **Meeting form (section 10) is front-end only.** The submit handler needs wiring to
  a CRM or endpoint — see `CONTACT_EMAIL` and the submit handler in the script block
  at the bottom of `index.html`.
- **Stall render is illustrative** — final fabrication may differ.

## Sources

Event dates, theme and organiser details from globalfintechfest.com; scale figures from
GFF 2025 press releases. No competitor content used.
