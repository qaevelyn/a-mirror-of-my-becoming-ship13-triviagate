# A Mirror of My Becoming™ Tools — Ship 13 · TriviaGate™

The canon build: a six-mode AWS CLF-C02 training arcade, statically exported from the fleet's
Next.js engine. No server, no accounts, no network at play time — every claim verified,
nothing leaves the browser.

**Play it live:** https://qaevelyn.github.io/a-mirror-of-my-becoming-ship13-triviagate/

## Why this exists

Built during Per Scholas AWS re/Start (cohort 2026-RTT-41): certification prep that plays
like a game instead of a wall of flashcards — a jeopardy board for recall, a rush mode for
pressure, a real exam engine for rehearsal, a forge for fresh questions, a flashback deck
for study group, and a teacher console for anyone's own deck. It is Ship 13 of the fleet:
the payload that goes through the gate once the record of the journey is complete.

## The six modes

1. **JEOPARDY** — 4 CLF-C02 domains × 5 values, hidden Daily Double, wrong answers pay the house.
2. **RUSH** — 15 questions, 20 seconds each, speed bonus + streak multipliers, kahoot tiles.
3. **EXAM** — 20 questions / 25-minute clock, flag-for-review, domain breakdown, 70% pass line.
4. **FORGE** — offline pattern drills from the verified 61-fact pool, or bring-your-own-key AI generation (your key never leaves the browser).
5. **FLASHBACK** — self-paced flashcards through all 61 verified facts. Flip, self-grade, no clock.
6. **TEACHER CONSOLE** — author, import (JSON · CSV · flashcards), export and manage custom decks; one switch mixes them into every game.

## Shipped in the canon build — Nov 6, 2026

- Canonical name: **A Mirror of My Becoming™ Tools — TriviaGate™**.
- Home page tiles render **three per row** (single column on phones).
- Answer choices render **three per line** in every mode (two per line on narrow phones).
- **MISSION LOG — results vault**: every finished run lands in the on-machine vault on the
  boot screen (last 30 kept), with the full log downloadable as one .txt.
- **.txt transcripts**: every result screen has a **Save report (.txt)** button, and any
  MISSION LOG row saves its own transcript. The report includes the result headline, stats,
  XP earned, domain breakdown, and a per-question review — your answer vs. the correct one
  and the "why". Opens in any text editor: offline review with no account and no network.
- XP, 11 ranks up to Commander, badges, best-streak memory — all localStorage, nothing sent anywhere.

## What's inside

| Path | What it is |
| --- | --- |
| `index.html` + `_next/` | The canon arcade, statically exported — every asset self-hosted in this repo |
| `404.html`, `robots.txt`, `logo.svg` | Static-site housekeeping |

## Controls

`1`–`4` answer · `Enter` confirm/next · `F` flag (exam) · `Esc` abort to menu — mouse/touch works everywhere too.

## Run it locally

The build is a static site: serve the folder with any static server, e.g.
`python3 -m http.server 8080` in this directory, then open
`http://localhost:8080/a-mirror-of-my-becoming-ship13-triviagate/` (the `/_next/` assets
need a server; double-clicking `index.html` won't resolve them).

## Updating later

Replace `index.html` + `_next/` with a fresh export, commit, push — Pages redeploys automatically.
