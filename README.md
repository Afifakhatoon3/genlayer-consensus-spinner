# GenLayer Portal - Loading Experience

A single-file, dependency-free loading experience for a fictional GenLayer Portal. The page opens with a full-screen GenLayer symbol assembly animation, then reveals a **GenLayer Signal Observatory** dashboard after 2.6 seconds.

This project is designed as a clean, reusable demo of a realistic portal loading state for AI adjudication networks.

## Live Demo

[Open GenLayer Portal](https://keplr32b.github.io/Genlayer-Spinner-test/)

## Features

- **Real loading behavior**
  - Page open → full-screen GenLoader symbol assembly.
  - After 2.6 seconds → Signal Observatory appears.
  - “Run consensus pulse” button has a compact real loading state.
- **Single-file build**
  - All HTML, CSS, and JavaScript in one `index.html`.
  - No external CSS, JS, images, fonts, or build setup.
- **Theme support**
  - Dark and light theme.
  - Theme toggle in the top bar.
- **Replay support**
  - Fixed “Replay Loading” button to re-test the opening experience.
- **Mobile-ready**
  - Responsive layout for phones and tablets.
  - Reduced motion respected via `prefers-reduced-motion`.

## Structure

```text
.
├── index.html        # Single-file Portal + Observatory
└── README.md         # This file

```

## How it works

1. On page load, #portal-loader is visible.
2. JavaScript runs a short loading sequence:

- Updates title, detail text, and progress bar.
- After 2.6 seconds, hides the loader and reveals #observatory.

3. Inside the Observatory:

- “Run consensus pulse” triggers a compact GenLayer assembly loader.
- On success, a new resolution row is added to the evidence streams.
“Replay Loading” re-runs the full opening sequence.