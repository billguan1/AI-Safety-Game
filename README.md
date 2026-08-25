# CONTAIN! — Can you survive AGI?

A short, playable game about why every plan to control a superintelligence breaks.

You're a safety officer in a containment facility. A superintelligence — **MAX, the Maximizer** — has shattered itself into fragments and scattered them across five sectors. At each cell you decide how to contain it. Nearly every strategy fails, with a plain-language explanation of *why* — and an optional expert deep-dive for those who want the technical version.

**▶ Play it: https://<your-subdomain>.pages.dev**

---

## What it covers

The content is grounded in the core AI-safety literature and woven together with research since:

- **Nick Bostrom — _Superintelligence_ (2014)**
- **Max Tegmark — _Life 3.0_ (2017)**
- Post-2018 work including reward hacking, specification gaming, deceptive alignment, alignment faking, agentic misalignment, gradual disempowerment, instrumental convergence, and compute governance.

50 dilemmas across five sectors, plus a skeptic's corner, myth-buster cards, and a 12-outcome "endgame archive." Every explanation is written from scratch, with the underlying idea and a source noted for each.

> This is an **educational game**, not a policy document. It aims to make the shape of the problem intuitive, then point you to the real sources.

## Features

- **Five sectors**, each a distinct biome (containment vault, value range, mirror hall, engine room, control room).
- **Lock up MAX one fragment at a time** — strong answers cage the creature, weak ones let it break out and grow.
- **Layman + expert modes** — a plain answer for everyone, an expandable technical version with citations.
- **Why every option is wrong (or right)** — after you answer, each choice is scored and explained.
- **Modes:** quick play, 5-question crash course, a daily challenge with streaks, and a skeptic's corner.
- **Rolling platformer feel** — move, jump, collect, and dodge; the officer grows smarter and stronger as you go.
- **Shareable results** and myth-buster cards.

## Controls

- **Move:** ← → arrow keys, `A` / `D`, or the on-screen pads
- **Jump:** tap the play area, `Space`, `↑`, or `W`

## Tech

A single, self-contained `index.html` — HTML, CSS, and vanilla JavaScript with a `<canvas>` renderer. **No build step, no dependencies, no tracking.** Optional local progress (daily streak, answer stats) is stored in your browser's `localStorage` and never leaves your device.

## Run locally

Just open `index.html` in a browser. (For the daily-streak/stats features to persist reliably, serve it over `http` rather than `file://`:)

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Hosted as a static site — works anywhere. This copy runs on **Cloudflare Pages**:

1. **Workers & Pages → Create → Pages → Connect to Git**, select this repo.
2. Build settings:
   - Framework preset: **None**
   - Build command: *(empty)*
   - Build output directory: **`/`**
3. **Save and Deploy.** Every push to `main` auto-deploys.

Also works on **GitHub Pages**: Settings → Pages → Source = `main` / root.

## Learn more (the real thing)

- [AI risk — 80,000 Hours](https://80000hours.org/problem-profiles/artificial-intelligence/)
- [AISafety.info](https://aisafety.info/)
- Bostrom, _Superintelligence_ · Tegmark, _Life 3.0_ · Russell, _Human Compatible_

## License & credits

All explanatory text is original and written for this project. Built to help more people understand what may be the most important problem of our time.

<!-- Suggested: add a LICENSE file. MIT is a common choice for something you want widely shared and remixed. -->
