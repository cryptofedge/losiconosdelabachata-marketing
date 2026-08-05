# Los Iconos Marketing Hub

> **Built by Marino Santos. Powered by Marino 007.**
> The campaign desk for Los Iconos de la Bachata — strategy, calendars, and platform-ready copy in one place.

Los Iconos de la Bachata is the official merch and cultural platform for Aventura and the legends of bachata. This repository is where the marketing behind it lives: brand strategy, monthly content calendars, campaign briefs, and finished post copy for all six platforms — versioned, reviewable, and ready to hand to whoever is posting that day.

It is a content repository, not an application. There is no build step and nothing to install.

---

## The System

| Section | What's There |
|---|---|
| `strategy/` | Brand strategy — who we are, voice, platforms, core hashtags |
| `campaigns/` | Campaign briefs with objectives, timelines, and per-platform copy |
| `calendar/` | Monthly content calendars |
| `content/` | Finished post copy, one folder per platform |
| `assets/copy-templates/` | Reusable content brief template and the Marino 007 WhatsApp command sheet |
| `assets/images/`, `assets/videos/` | Creative assets |
| `analytics/` | Performance tracking |
| `index.html` | Marketing hub landing page, served via GitHub Pages |

---

## Architecture

Flat, browsable Markdown. Strategy sets the voice, campaigns apply it, calendars schedule it, and `content/` holds the copy that actually ships.

```
strategy/brand-strategy.md      voice, platforms, hashtags — the source of truth
   |
campaigns/                      objective + timeline + UTM links per drop
   |-- summer-drop-001-la-cultura-no-para
   |-- august-de-vuelta-al-barrio
   |-- fan-feature-series-los-iconos-de-la-comunidad
   |
calendar/                       june-2026, july-2026
   |
content/                        ready-to-post copy
   |-- instagram/  tiktok/  facebook/  twitter-x/  youtube/  threads/
   |
assets/copy-templates/          brief template + Marino 007 bot commands
```

`.nojekyll` is present so GitHub Pages serves `index.html` as-is rather than running it through Jekyll.

---

## Core Files

| File | Purpose |
|---|---|
| `strategy/brand-strategy.md` | Brand voice, platform list, and core hashtags |
| `assets/copy-templates/content-brief-template.md` | Starting point for a new campaign brief |
| `assets/copy-templates/whatsapp-bot-commands.md` | Marino 007 WhatsApp commands for generating posts |
| `campaigns/*.md` | One brief per campaign — objective, timeline, platforms, copy |
| `calendar/*.md` | Month-by-month posting schedule |
| `index.html` | Public marketing hub page |

---

## Marino 007 Commands

Post copy can be generated from WhatsApp through the Marino 007 agent. Full list in [`assets/copy-templates/whatsapp-bot-commands.md`](assets/copy-templates/whatsapp-bot-commands.md).

```
!iconos [topic]           Generate posts for Instagram, TikTok, Facebook, Twitter/X
!iconos-spanish [topic]   Same, in Spanish
```

---

## Brand

- **Voice:** Direct. Proud. Cultural. Spanish and English, sometimes in the same sentence. Emotion over hype.
- **Audience:** People who grew up with this music — quinceañeras, weddings, and "Obsesión" on repeat at 2am.
- **Platforms:** Instagram · TikTok · Facebook · Twitter/X · YouTube · Threads
- **Site:** [losiconosdelabachata.com](https://losiconosdelabachata.com)
- **Core tags:** `#LosIconosDeLaBachata` `#Bachata` `#Aventura` `#BachataLife` `#OrgulloLatino`
- **Credit:** Built by **Marino Santos**

---

## Quick Start

Nothing to install — clone and read.

```bash
git clone https://github.com/losiconosdelabachata-star/losiconosdelabachata-marketing.git
cd losiconosdelabachata-marketing
```

**Starting a campaign:** copy `assets/copy-templates/content-brief-template.md` into `campaigns/`, fill in objective, timeline, and platforms, then write the per-platform copy into `content/`.

**Previewing the hub page:**

```bash
python -m http.server 8000
```

---

## Roadmap

- [x] Brand strategy documented
- [x] June and July 2026 content calendars
- [x] Three campaigns briefed with per-platform copy
- [x] Post copy for all six platforms
- [x] Marino 007 WhatsApp command sheet
- [x] Marketing hub page on GitHub Pages
- [ ] Analytics populated with real performance data
- [ ] Image and video assets committed
- [ ] Calendars beyond July 2026

---

## License & Brand

<img src="marino-007-avatar.png" alt="Marino 007" width="120" height="120">

### Los Iconos de la Bachata | Built by Marino Santos

**© 2026 Marino Santos. All rights reserved.**

This project is proprietary and protected under copyright law. Unauthorized use, reproduction, or distribution is strictly prohibited.

### License Details

- **Type:** Proprietary — All Rights Reserved
- **Owner:** Marino Santos
- **Brand:** Los Iconos de la Bachata
- **Status:** Protected and Confidential

### Key Rights

- **All intellectual property retained**
- **Reproduction prohibited without permission**
- **Distribution rights reserved**
- **Derivative works not permitted**
- **Commercial use requires authorization**

### Attribution

When referencing this work, please include:
- Los Iconos de la Bachata
- Marino Santos
- Marino 007

### Inquiries

For licensing, partnerships, or usage permissions:
Email: **007@marinosantos.com**

---

**Learn more:** [Full License](LICENSE) · [Brand Strategy](strategy/brand-strategy.md)

**Los Iconos de la Bachata** — *Timeless Music, Timeless Stories*
