# Hudson Harvest 2026 — Field Operations Calendar

Interactive operations calendar for the Hudson Harvest 2026 outdoor cannabis cultivation season at Montgomery, NY (41.5°N, Zone 6a/6b).

**Live URL:** [hudson-harvest-ops.vercel.app](https://hudson-harvest-ops.vercel.app) *(update once deployed)*

## What's inside

A single-file static HTML application with four tabs:

- **📅 Gantt** — full-season execution timeline, May 25 through October 18. Bars, milestones, and marker lines for every workstream.
- **📋 Key Dates & Crew** — chronological action list with crew and resource assignments for every milestone.
- **🛠 Soil SOP & Notes** — soil delivery and pot-fill procedure for the week of June 8, plus four critical-path notes.
- **⚙ Legend** — full reference for every bar color, marker, and line on the Gantt.

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

This site is deployed automatically from this repo. To push a new version:

1. Replace `index.html` with the new HTML file (rename the new file to `index.html` before uploading).
2. Commit the change — Vercel auto-deploys within ~30 seconds.
3. The live URL stays the same; team bookmarks don't break.

## Format

Single self-contained HTML file. No build step, no dependencies installed at deploy time. Renders in any modern browser; works on phones (Gantt scrolls horizontally). Fonts pulled from Google Fonts at page load.

## Versioning

Current version stamped in the top-right of the nav bar (`v11 · Team Reference` as of this writing). Bump when content materially changes.

## Coverage notes

- Photoperiod flip pinned to 14-hr daylength crossover at 41.5°N — does not move regardless of plant size.
- Frost wall is the regional mid-Hudson average first fall frost. Late harvest only on clean, frost-free forecasts.
- Transplant trigger is biological, not calendar: starts when roots show through the bottom of the 4″ pots. Jun 24–26 is the planned window.

---

Operations calendar for Hudson Harvest 2026 outdoor season. Not for distribution outside the project team.
