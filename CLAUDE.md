# UnPossible LLC — unpossiblellc.com

## ⛔ HARD RULE — HANDOFF PROTOCOL (non-negotiable)
Every session touching this repo MUST:
1. ON START: read this file + the top (newest) entry of docs/HANDOFF.md before any change. State what the last session left off.
2. ON END: append a new entry to the TOP of docs/HANDOFF.md (template inside), commit and push it. A session that changed anything without writing a handoff is a failed session.
3. Append-only — never rewrite old handoff entries.
4. Keep docs/ROADMAP.md checkboxes current; never silently drop an item.

## What this is
Brand home for UnPossible LLC — "we make the unpossible, possible." Small studio, suspiciously large things. Playful, weird, surprising, dark terminal-hacker aesthetic.
Products: EngulfScan Pro (weekly S&P 500 engulfing scanner, LIVE), The Container (40ft/400A GPU cloud on Vast.ai, ONLINE), Super Clawd (2 Mac Minis meshed via Tailscale into one Claude Code brain, MESHED), Project ?????? (classified teaser).

## Architecture
ONE file: index.html. Fully self-contained (inline CSS/JS, WebAudio synthesized, generative canvas bg). Only external dep: Google Fonts. Stay single-file until ROADMAP Phase 3 says otherwise.
Hosting: Render static site auto-deploys from main (build cmd: none, publish dir: "."). Domain unpossiblellc.com via GoDaddy DNS (A @ → Render IP, CNAME www → onrender host). Deploy = push to main. Never push broken code.

## Design system (do not drift)
bg #060810, surfaces #0c1018/#141820/#1c2230, accent GOLD #f0c040, blue #4090ff, green #30d060, red #f04040, purple #a070f0 (sparingly).
Fonts: Bebas Neue (display), Barlow Condensed (labels), IBM Plex Mono (body).
NEVER: purple gradients, white bg, pill buttons, Inter/Roboto/system-ui.
Every new feature ships with at least one hidden thing.

## Easter eggs (8) — protect when editing
1 press U (or tap) to skip boot intro · 2 click logo 5× · 3 Konami code → rave · 4 tiny "·" button in Contact · 5 click struck-through word in Mission · 6 triple-click hero wordmark · 7 idle 45s · 8 open terminal (backtick).
Bonus: unpossible.hire() in console; "prize" in terminal after all 8. Keep EGG_TOTAL, boot line, badge, and console text in sync if eggs change.

## Testing (required before any push to main)
Headless Chromium: zero page errors; boot completes; U-key skip works; terminal opens and "help" responds; egg counter increments. Screenshot hero + work sections and look at them.
