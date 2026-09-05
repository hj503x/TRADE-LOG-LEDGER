# LEDGER

A minimalist, offline-first trade journal for discretionary traders — built as a single HTML file with zero dependencies beyond a browser.

## Why

Most trade journals either live in a spreadsheet (no insight) or require an account and internet connection (no privacy, no control). LEDGER is neither — it's one file, runs entirely client-side, and stores everything in your browser's local storage. Nothing leaves your device unless you export it.

## Features

- **Trade log**: serial number, asset, date, direction (long/short), result (hit/miss/breakeven/pending), risk:reward
- **Behavioral tagging**: setup type, session, whether you followed your own rules, mistake type, emotional state at entry
- **Analytics**: win rate, average R:R, longest and current streaks, rule adherence %, equity curve, win rate by asset/session/setup/day-of-week, top recurring mistakes, best/worst trade
- **Risk tools**: position-size calculator, weekly R target with progress bar, open-exposure warning for stacked pending trades
- **Data ownership**: CSV export, JSON backup/restore, printable report, no server, no tracking
- **Light/dark theme**, mobile and desktop friendly

## Usage

Open `trade-log-1.html` in any browser — no build step, no install. Works as a local file or hosted on GitHub Pages / any static host.

## Data

All data is stored in `localStorage` on your device. Use **Backup JSON** regularly — it's your only backup. **Restore JSON** merges or replaces your data from a backup file.

## Stack

Vanilla HTML/CSS/JS. No frameworks, no build tools, no external runtime dependencies (jsPDF is loaded via CDN only for print/report use).
