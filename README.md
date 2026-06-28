# Knight Spiral Pattern Generator

A mathematical pattern visualiser hosted on GitHub Pages.

**Live site:** `https://jacksonhcnz.github.io/knightspiral/`

## How the pattern works

Starting from the centre of a checkerboard grid, squares are visited in an outward square spiral. At each square, a knight is placed **unless** it is already under attack by a previously-placed knight (using standard chess knight moves). Knights placed later in the spiral are assigned to teams in round-robin order, each rendered in a distinct colour.

## Features

- Adjustable grid size (odd numbers, up to 61×61)
- Cell scale slider (4 – 64 px per square)
- Up to 8 knight teams, each a different colour
- Toggle skipped squares and spiral path overlay
- Hover tooltip showing coordinates and team
- Seed system — any text string deterministically configures all settings via SHA-256
- Shareable seed URLs (`?seed=your-text`)
- Export PNG

## Deploying to GitHub Pages

1. Create a new GitHub repository (public).
2. Upload `index.html` to the root of the `main` branch.
3. Go to **Settings → Pages → Source** and set it to `Deploy from branch: main / root`.
4. Your site will be live at `https://<username>.github.io/<repo>/` within ~60 seconds.

No build step, no dependencies, no Node.js — just one HTML file.

## Running locally

Open `index.html` directly in any modern browser. No server needed.

## Files

```
index.html   ← the entire app (HTML + CSS + JS, self-contained)
README.md
```
