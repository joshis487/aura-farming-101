# Aura Farming 101

Turn your daily life into a progression game.

Complete routines → earn XP → build streaks → level up → collect achievements → grow your Aura.

A premium, game-inspired daily habit and routine tracker. The interface stays clean and minimal — the game mechanics live in the language and the moments (XP gains, streaks, level-ups), not in cartoon characters or clutter.

## Live app

Open `index.html` in any browser — no install, no account, no build step. If this repo has GitHub Pages enabled, the live link is in the **About** section on the right side of this repo's homepage.

## Features

- **Today** — your Aura Level, XP progress toward the next level, Daily Score, Aura Streak, and today's Daily Quests in one view. Checking something off awards XP immediately with a small animation.
- **Daily Quests** — recurring habits, either every day or on specific weekdays, optionally grouped into Morning / Afternoon / Evening.
- **One-time tasks** — quick, ad-hoc to-dos that also earn XP but don't repeat.
- **Perfect Day** — clearing every quest for the day triggers a celebration and bonus XP.
- **Aura Streak** — an overall daily streak, plus a separate streak tracked per routine.
- **Auto-progressing routines** — a routine can carry a set of exercises (name + reps). After a configurable streak milestone (e.g. every 15 days), the reps automatically increase and the routine levels up — a built-in progressive-overload mechanic for workouts or similar habits.
- **Achievements** — a fixed set of badges for milestones: first Perfect Day, streak lengths, tasks completed, total Aura earned, and Aura Level thresholds.
- **Journey** — XP over time, a consistency heatmap, performance by category, Aura Level history, and the full achievement shelf.
- **Routine management** — add, edit, pause, delete, and drag-reorder routines; create custom categories with their own color.
- **Light / dark / system theme.**

## How your data is stored

- Opened inside a Claude artifact: progress is saved to that artifact's built-in database.
- Opened as a plain file or hosted elsewhere (e.g. GitHub Pages): progress is saved to that browser's local storage instead.

Either way, each browser/device keeps its own independent, private progress — nothing is shared between people unless they're opening the exact same artifact link.

## Tech

Single self-contained HTML file. React 18 and Babel Standalone loaded from a CDN, no build step or package manager required. All styling is hand-written CSS with light/dark theme tokens.

## Customizing

Everything — categories, XP values, difficulty presets, the achievement list, colors — is defined near the top of the `<script>` block in `index.html` and is safe to edit directly.
