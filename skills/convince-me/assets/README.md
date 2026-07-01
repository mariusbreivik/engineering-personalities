# Conviction Meter Visuals

This directory contains GitHub-friendly SVG assets for the `convince-me` skill.

## Included Assets

- `conviction-08.svg`: early rejection state with mostly unresolved objections
- `conviction-42.svg`: middling state where some answers helped, but not enough
- `conviction-68.svg`: conditional approval territory with remaining rollout risk
- `conviction-91.svg`: high-confidence approval after strong evidence
- `conviction-progression.svg`: four-panel overview showing how the meter evolves

## Usage

Use these assets in repository docs, skills.sh screenshots, blog posts, or release notes.

Example:

```md
![Conviction meter at 42 percent](./assets/conviction-42.svg)
```

## Design Notes

- Dark terminal-style framing so the images feel like agent output rather than generic marketing cards.
- Clear block meter representation that matches the `SKILL.md` output format.
- Objection checklist included in every asset so the score is visibly tied to reasoning.
