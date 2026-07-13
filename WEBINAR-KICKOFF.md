# Webinar materials — Rankscale API (session kickoff)

Paste this into a fresh Claude Code session to continue. **API-only from here** (no MCP).

## Goal
Build an HTML **home page** that links the two existing reports and, next, several **API usage-example docs**. Keep everything as one visually consistent series.

## Existing artifacts to link
Published on claude.ai — **private until shared** via each page's share menu.
- **MCP vs API** — https://claude.ai/code/artifact/097fa3dd-1251-4397-a054-83899026cdd2  (favicon 📊)
- **AI Engine Consistency** — https://claude.ai/code/artifact/c57de33e-039c-41c6-b22b-95e374bc2d8e  (favicon 🎯)

## Local deliverables folder (save copies here)
`C:\Users\BojkoB\Desktop\AGY Temp\Rankscale\Public Shared\`
- `mcp-vs-api-rankscale.html`
- `ai-engine-consistency.html`
- `rankscale-skill.zip`

## Design system (reuse for series consistency)
- **Palette:** cool off-white paper / cool near-black ink; teal accent `#0f766e` (dark `#2dd4bf`); amber `#b45309` (dark `#fbbf24`). Badges: `[API]` = teal, `[GUI]` = amber.
- **Type:** serif display (Iowan Old Style / Palatino system stack), system sans body, mono for labels + data.
- **Layout:** single ~760px reading column + ~1080px wide breakout for tables/charts; findings-first; reveal-on-scroll.
- **Theme-aware** (light + dark, via `:root` tokens + `prefers-color-scheme` + `data-theme` overrides).
- **Self-contained:** Artifact CSP blocks external CDNs — inline all CSS/JS, hand-build charts as inline SVG/HTML (no Chart.js).

## State already in place
- `rankscale` skill updated: Brand Rank (by Visibility) recipe §6; quirks 15–18 (workspace-scoped keys, competitorTimeSeriesData excludes own brand, aggregate≠daily, date-filter myth debunked); file-first token-efficiency note.
- Memories saved: `reference-rankscale-brand-rank`, `mcp-vs-api-token-crossover`.

## ⚠️ API key — resolve before live calls
- Env `RANKSCALE_API_KEY` = business account (analytics@granulargroup.com) — **cannot see** the De'Longhi test brand (`1YpikjKnrLC96tSJR6Yz`).
- A private-account key (bojan.basrak@gmail.com) can see De'Longhi but was exposed in the prior chat — **rotate it**, and decide which account/brand the webinar examples should use.

## Suggested next steps
1. Draft the home-page structure (hero + cards linking the two reports + a "usage examples" section with placeholders).
2. Decide the list of usage-example docs to create (e.g. pull visibility, compute Brand Rank, citations, sentiment, credits, a bulk file-first export).
3. Build each example as its own artifact + local copy, then link from the home page.

## Note on hosting for a public webinar
claude.ai artifacts are private-by-default and shared via link — **test each shared link while logged out** to confirm external attendees can view it. Since local HTML copies exist in `Public Shared`, they can also be self-hosted (own server / static host) for guaranteed public access and control.
