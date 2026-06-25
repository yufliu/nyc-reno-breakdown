# NYC Reno Cost Breakdown — Contractor vs. Self-GC

A single-file, no-backend dashboard for breaking a renovation quote into **materials + labor**, then comparing the contractor's price against doing it yourself as general contractor (subbing each trade).

**Live:** open `index.html` in any browser, or visit the GitHub Pages URL.

## What it does
- Decomposes each quoted line into materials (qty × unit price, + sales tax) and labor (hours × rate, with per-trade job minimums).
- Shows **gross savings**, **net savings** (after the real costs of self-GC'ing — permits, contingency, the value of your time), and a per-line **negotiate / DIY / let-contractor-keep** badge.
- Gives a quotable **counter-offer** per line, framed as the contractor's own cost + a fair markup.
- NYC-realistic defaults: 8.875% material sales tax, licensed plumber/electrician rates + visit minimums.

## Privacy
Everything runs in your browser. Nothing is uploaded. Your edits persist in `localStorage` only. Use **Export JSON** to save a private snapshot and **Import JSON** to reload it (e.g. on another device) — keep that file private; it never touches this site.

The numbers shipped here are **illustrative examples**, not anyone's real quote.

## Stack
Vanilla HTML/CSS/JS. No build, no dependencies. Just `index.html`.
