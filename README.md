# Hudson Harvest 2026 — Operations Hub

Operations hub for the Hudson Harvest 2026 outdoor cannabis cultivation season at Montgomery, NY (41.5°N, Zone 6a/6b). A small, durable static site: a landing page (`index.html`) that links out to self-contained HTML documents, one per project/topic. New documents drop in as siblings over time.

**Live URL:** [opstimeline.vercel.app](https://opstimeline.vercel.app) (also serves husdonharvest.space). Auto-deploys from `main`.

## What's inside

Flat static site — one self-contained HTML file per page, all at the repo root:

- **`index.html`** — the hub landing page (cards + timeline linking to every document below).
- **`gantt.html`** — 📅 Field Operations Calendar: the full-season execution Gantt, with Key Dates & Crew, Soil SOP & Notes, and Legend tabs. This is the original calendar, formerly served as `index.html`.
- **`field-build-plan.html`** — 🛠 2026 Field Build Plan: the ~30-day build to get 1,000 plants in the field (warehouse & tents, prop house, irrigation, the 45-gal pot matrix, budget).

## Season anchors

| Gate | Date | Notes |
|---|---|---|
| Clone cut at TC nursery | Mon Jun 1 | ~14-day root cycle |
| Clones arrive at farm | Mon Jun 15 | Indoor prop, hold 2 days |
| Up-pot to 4″ container | ~Jun 17 | Settle 2 days under lights |
| Move to prop greenhouse | Sun Jun 21 | Solstice — begin hardening |
| Field transplant | Jun 24–26 | 3-day operation, triggered by root visibility |
| Photoperiod flip | ~Aug 6–8 | Daylength crosses 14 hr at 41.5°N |
| First frost wall | ~Oct 14 | Regional avg — hard stop |

## Three parallel build streams (May 28 – Jun 22)

1. **Prop infrastructure** (▲) — indoor prop space prep → prop greenhouse build
2. **Field infrastructure** (◆) — irrigation rework → soil + pot fill
3. **Perimeter / security** (▼) — deer fence build (target Jul 4, hotwire backup required by transplant)

All three must converge by Jun 22 — two days before transplant begins.

## How to update

This site is deployed automatically from this repo (Vercel auto-deploys from `main` in ~30 seconds; live URLs stay stable so team bookmarks don't break).

**To add a page:** drop its `.html` file at the repo root and add a matching card + timeline entry to `index.html`. Keep the link relative — `href="my-page.html"`.

**To retire a page:** remove its card from `index.html` (and optionally delete the file).

**To update an existing page** (e.g. a new Gantt version): replace that page's `.html` file in place, keeping the same filename so the hub link still resolves. Commit — Vercel redeploys automatically.

Keep it flat: no build step, no framework, no bundler, no `/public` or `/dist`, no subfolders. Every document is a single self-contained HTML file, and all internal links are relative — never absolute paths or hardcoded full domains.

## Format

Self-contained HTML files, one per page, served flat from the repo root. No build step, no dependencies installed at deploy time. Renders in any modern browser; works on phones (the Gantt scrolls horizontally). Fonts pulled from Google Fonts at page load.

## Versioning

Current version stamped in the top-right of the nav bar (`v11 · Team Reference` as of this writing). Bump when content materially changes.

## Coverage notes

- Photoperiod flip pinned to 14-hr daylength crossover at 41.5°N — does not move regardless of plant size.
- Frost wall is the regional mid-Hudson average first fall frost. Late harvest only on clean, frost-free forecasts.
- Transplant trigger is biological, not calendar: starts when roots show through the bottom of the 4″ pots. Jun 24–26 is the planned window.

---

Operations calendar for Hudson Harvest 2026 outdoor season. Not for distribution outside the project team.
