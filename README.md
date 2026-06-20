# Real Estate AI Lead Nurturing Agent

**Lumen** — an AI-assisted lead-nurturing CRM for real estate agents. Leads are
captured from multiple sources (Zillow, WhatsApp, website forms, Facebook ads),
auto-qualified and scored by an AI assistant ("Aria"), and surfaced to the agent
with a morning briefing, suggested replies, and a hand-off flow when a lead turns hot.

This repo contains a self-contained front-end prototype implemented from the
[Claude Design](https://claude.ai/design) source `Lumen Lead Nurturing.dc.html`.

## Features

- **Lead Inbox** — segment/source filters, lead scoring, stat tiles, and an Aria insights panel.
- **Lead Detail** — profile, score gauge, qualification facts, AI intent summary, activity timeline, and a live conversation thread.
- **AI ↔ Human handoff** — toggle between "Aria handling" and "You handle", click an AI-suggested reply to take over, and review a full hand-off briefing before stepping in.

## Running locally

No build step required. The app is a single static `index.html` that loads React
and Babel from a CDN.

```bash
# Option 1 — just open the file
start index.html      # Windows

# Option 2 — serve the folder
npx serve .
```

## Deployment

The app is a static site. On [Vercel](https://vercel.com) it deploys with zero
configuration — `index.html` is served at the root.

## Tech

- React 18 (UMD via CDN)
- Babel Standalone (in-browser JSX)
- No bundler / no dependencies to install
