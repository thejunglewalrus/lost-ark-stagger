# Lost Ark Stagger Tool

A browser-based reference for Lost Ark stagger (paralyzation) values across
every class, skill, and tripod combination.

[**→ Open the tool**](https://thejunglewalrus.github.io/stagger-tool/)  <!-- update this URL -->

## What it shows

- **Per-class skill lists** with stagger values pulled from the game DB and
  verified against combat-log encounter data
- **Tripod-modified stagger** — each tier's popular pick is pre-applied, and
  custom selections update live
- **Chain/Hold/Summon callouts** for complex skills (Perfect Zone totals,
  multi-press combos, auto-attack dps, ground effects)
- **Boss paralyzation thresholds** for the current Kazeros Raid acts
- **Ark Grid stagger modifiers** reference

## Data sources

Stagger values use a three-layer priority:

1. **Verified** — manually tested in-game against the training dummy
2. **Encounter calibration** — mode per-cast stagger from combat logs
3. **Dedup formula** — DB sum of unique AiPointMin effects (fallback)

Skill icons are merged from lostark.bible (popularity + tripods),
lostarkcodex.com, and lostark.fandom.com.

## Found something wrong?

Use the **"Report it"** link at the bottom of the tool to submit corrections.
Every submission is reviewed before going live.

## How it's built

This repository contains the static site only. The Python build pipeline that
generates the data files lives in a separate local project — the JSON under
`data/` is the baked output of that build.

## License & attribution

Skill data extracted from the Lost Ark client. Skill icons courtesy of
lostark.bible, lostarkcodex.com, and the Lost Ark Fandom wiki.

This project is not affiliated with Smilegate or Amazon Games.
