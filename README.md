# 🎓 New Grad Positions — Company Search

A single-file, self-updating search tool for new-grad tech job listings. Open it in any
browser and instantly search thousands of positions by company, role, or location — with
big-tech companies ranked to the top.

**[▶ Open the live app](index.html)** *(or enable GitHub Pages — see below)*

## Features

- 🔎 **Instant search** across company, title, and location (multi-word AND matching, highlighted)
- ⭐ **Smart ranking** — Big Tech (Google, Meta, Amazon, NVIDIA, TikTok…) and other top
  companies float to the top; toggle to sort by newest instead
- 🕒 **Posted date** on every listing (absolute + relative age)
- 💰 **Salary** shown when available
- 🧭 **Filters** — category, sponsorship, source, and active-only
- 🔄 **Self-updating** — pulls the latest data live from three community job repos on every
  open, auto-refreshes every 30 min, and falls back to an embedded snapshot when offline
- 📦 **Zero dependencies** — one static HTML file, no build step, no server

## Data sources

Data is fetched live (client-side) from these community-maintained repositories:

| Source | Repository |
|---|---|
| Simplify | [SimplifyJobs/New-Grad-Positions](https://github.com/SimplifyJobs/New-Grad-Positions) |
| SpeedyApply | [speedyapply/2026-SWE-College-Jobs](https://github.com/speedyapply/2026-SWE-College-Jobs) |
| Ambicuity | [ambicuity/New-Grad-Jobs](https://github.com/ambicuity/New-Grad-Jobs) |

Listings are de-duplicated by application URL and normalized into a common schema. An
embedded snapshot of the Simplify data ships inside `index.html` so the app still works
with no internet connection.

## Run it

- **Locally:** download `index.html` and double-click it.
- **Hosted (always-fresh URL):** enable **GitHub Pages** on this repo
  (Settings → Pages → Deploy from branch → `main` / root). Because the page fetches data
  live in the browser, no build or scheduled job is needed — the hosted page stays current
  on its own.

## Credits

All job data belongs to the respective source repositories and their contributors. This
project is just a search front-end over their public data.
