# B2B Revenue Engine

**Find where revenue leaks between marketing, sales and customers, then put a dollar figure on it.**

**Live:** https://zov911.github.io/b2b-revenue-engine/ · built by [zov911](https://zov911.com)

![Single file](https://img.shields.io/badge/single%20file-no%20build-0ea5e9) ![Vanilla JS](https://img.shields.io/badge/vanilla-JS%20%2B%20SVG-f97316)

## What you can do

| | |
|---|---|
| 🗺 **Process map** | Click any of the 17 nodes to see what it feeds the other team, what it needs back, the KPIs, the **sales science** behind it and **what can be automated** |
| 💧 **Show leaks** | Leaking hand-offs turn red and drip dollars. Made for screen-sharing on a call |
| ⚡ **Leak audit** | 4 numbers + tick your problems → yearly **cost of inaction**, a ranked breakdown and a **Smarketing alignment score** (0–100) |
| 🏭 **Industry presets** | SaaS, Manufacturing, Professional services: terms, defaults and a field case change with one click |
| 📤 **Take it with you** | Copy the action plan as Markdown, save a PDF report, copy a link that reopens your exact numbers, share your score on LinkedIn |

## Use it on a sales call (2 minutes)

1. Open the **Leak audit** and pick the client's industry.
2. Type their leads per month, average deal value and lead-to-customer rate.
3. Tick the problems they admit to. Open a leak to adjust its assumption together.
4. Switch to **Process map → Show leaks** to show where it happens.
5. **Copy link** and send it after the call. It opens with their numbers.

## Where the numbers come from

Every dollar figure uses an assumption you can see and edit, set **below** what the source reports:

| Leak | Default | Source |
|---|---|---|
| No 24-hour reply SLA | +15% inbound deals | Coe (2003), citing Performark: 24-hour response raised conversion to sale 7–10× |
| Demo before discovery | +10% deals | Cognism (2021), citing Sales Benchmark Index: demos without discovery are 73% less successful |
| "Not now" leads not nurtured | 30% buy within 18 months, 5% recovered | Coe (2003): 30–50% of B2B inquiries buy within 12–18 months |
| Sellers prospecting themselves | 4 reps × 8 h/week × $75/h | Coe (2003): a field sales call costs $300–400 |

The sales-science tab also uses Atkinson, *The Psychology of Salesmanship* (1912: "Easyboy & Hardfellow", the Pre-Approach) and Hall, *The Handbook of Sales Management* (1924: compensation plans). Details: [docs/methodology.md](docs/methodology.md).

## Customise

Everything lives in one `index.html`. Edit the data blocks at the top of the script:

| Block | What it controls |
|---|---|
| `MN`, `SN`, `CN` | Map nodes and their flows |
| `SCI`, `AUTO` | Sales-science and automation tabs |
| `IND` | Industry presets, defaults, field cases |
| `LEAKS` | Audit questions, formulas, sources, fixes |

Guide: [docs/customize.md](docs/customize.md). Run locally: open `index.html`, or `python -m http.server`.

## Branches

`main` = live site (GitHub Pages) · `develop` = next release · `feature/*` → PR into `develop`. See [CONTRIBUTING.md](CONTRIBUTING.md).

## More from zov911

| Tool | What it shows |
|---|---|
| [AI Lead Qualification Agent](https://zov911.github.io/ai-lead-qualification-agent/) | Fixes the SLA and discovery leaks: score, route and reply inside the CRM |
| [Talk to Your Analytics](https://github.com/zov911/talk-to-your-analytics) | Ask Claude why leads dropped across GA4, Search Console and HubSpot |
| [Marketing Signal Dashboard](https://zov911.github.io/marketing-signal-dashboard/) | Attribution, server-side tracking, SEO opportunities |
| [Release Launch Kit](https://zov911.github.io/release-launch-kit/) | Product updates → launch content for every channel |
| [Trim Press Tonnage Calculator](https://zov911.github.io/trim-press-tonnage-calculator/) | Industrial buyer tool |

---

**Want these leaks fixed in your stack? → [zov911.com](https://zov911.com)** · [@zov911 on X](https://x.com/zov911)

© zov911. All rights reserved.
