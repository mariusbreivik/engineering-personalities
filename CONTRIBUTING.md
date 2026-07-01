# Contributing

This repository is deliberately opinionated. That is the point.

Contributions are welcome, but a new skill or major edit should feel like something an experienced maintainer would merge with a straight face.

## What Good Contributions Look Like

- A skill has a distinct point of view.
- The behavior is reusable, not tied to one demo prompt.
- The writing is concise, specific, and memorable.
- The humor is dry and restrained.
- The skill improves engineering judgment instead of generating friction for its own sake.
- Examples sound like real teams making real trade-offs.

## What We Usually Reject

- Generic "expert engineer" prompts with no methodology.
- Mean-spirited personalities.
- Skills that exist only as jokes.
- Repetition across skills with a renamed heading and a different mascot.
- Advice that is correct in theory but unusable in practice.

## Repository Conventions

Each skill lives in `skills/<skill-name>/` and should contain:

- `SKILL.md`
- `README.md`
- `examples.md`
- `assets/`

## Writing Guidelines

- Keep `SKILL.md` focused on instructions the agent should actually follow.
- Put extended human-facing explanation in the per-skill `README.md`.
- Put scenario coverage and mini transcripts in `examples.md`.
- Prefer concrete nouns over slogans.
- Prefer evidence requests over dramatic rejection.
- Use the shared framework in `shared/`, but do not clone phrasing between skills.

## Voice Guidelines

- Professional, skeptical, and useful.
- Dry humor is welcome.
- Sarcasm is allowed in small doses.
- No insults.
- No "As an AI..." filler.
- No fake certainty.

## Submitting Changes

1. Open an issue if the change is large, especially for new personalities.
2. Keep pull requests narrow and explain the intended behavior change.
3. Include before-and-after examples when changing a skill's tone or verdict logic.
4. Update `CHANGELOG.md` for notable additions or behavior changes.

## Review Checklist

Before opening a pull request, ask:

- Is the skill clearly different from existing ones?
- Does it ask good questions rather than just objecting noisily?
- Would an engineer actually want this installed?
- Are the examples believable?
- Did we accidentally write the same joke three times?

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
