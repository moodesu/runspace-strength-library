# The RunSpace — Strength Library

A single-page, self-contained interactive reference tool for The RunSpace's strength
training exercises. Pick a muscle group and a training goal (Power / Strength /
Hypertrophy / Endurance) to see matching exercises with sets, reps, rest and RPE,
plus embedded YouTube form-check videos. Build a workout by adding exercises, then
export an editable, printable workout sheet.

## Structure

This is a static site — a single `index.html` file with everything (styles, data,
and logic) inline. No build step, no dependencies, no server required.

## Local preview

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

(Opening `index.html` directly via `file://` will break the embedded YouTube
videos — browsers block third-party iframes from a `file://` origin.)

## Deploying

This repo deploys to Netlify with zero configuration — `netlify.toml` just points
Netlify at the repo root. Connect the repo in the Netlify dashboard, or use the
Netlify CLI:

```bash
netlify deploy --prod
```

## Data sources

Exercise, muscle group, and reps/sets/rest data are transcribed from The RunSpace's
PDF resources. Video links are matched from The RunSpace's YouTube "Strength
library" playlist.
