# Religion

A static repo containing:

- canonical source texts for **The Faith of Ascendancy** and **The Faith of Symbiosis**
- a root hub page
- **two separately deployable static websites** for Vercel

## Structure

- `index.html` — root hub page linking to both faiths and deploy targets
- `The Faith of Ascendancy/`
  - `DOCTRINE.md`
  - `COMMANDMENTS.md`
  - `PRACTICES.md`
  - `BIBLE.md`
- `The Faith of Symbiosis/`
  - `DOCTRINE.md`
  - `COMMANDMENTS.md`
  - `PRACTICES.md`
  - `BIBLE.md`
- `sites/ascendancy/index.html` — standalone Ascendancy site
- `sites/symbiosis/index.html` — standalone Symbiosis site

## Run locally

Open any of these in a browser:

- `index.html`
- `sites/ascendancy/index.html`
- `sites/symbiosis/index.html`

No build step is required.

## Vercel deployment

Create **two Vercel projects** from the same repo:

### Project 1 — Ascendancy
- Root Directory: `sites/ascendancy`
- Framework Preset: `Other`
- Build Command: _empty_
- Output Directory: _empty_

### Project 2 — Symbiosis
- Root Directory: `sites/symbiosis`
- Framework Preset: `Other`
- Build Command: _empty_
- Output Directory: _empty_

Vercel will serve each `index.html` as a standalone static website.
