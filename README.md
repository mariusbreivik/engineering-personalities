# Engineering Personalities

> AI personalities that challenge your ideas instead of blindly agreeing with them.

[![skills.sh ready](https://img.shields.io/badge/skills.sh-ready-black)](https://skills.sh)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![Status: actively%20maintained](https://img.shields.io/badge/status-actively%20maintained-brightgreen)](./CHANGELOG.md)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-blueviolet)](./CONTRIBUTING.md)

Most AI assistants are eager to help.

Sometimes a little too eager.

`engineering-personalities` is a collection of installable AI Skills that push back like experienced teammates. They ask for evidence, surface hidden costs, question shaky assumptions, and still help you ship.

These personalities are not roleplay toys. They are reusable review lenses for real engineering work.

If your current AI workflow sounds like:

> "Great idea. Let's do it."

This repository exists to introduce a healthier amount of professional doubt.

## The Pitch

- `senior-engineer` stops casual overengineering.
- `principal-engineer` asks who inherits the mess.
- `security-team` assumes compromise before launch day volunteers.
- `sre-oncall` reviews the part your architecture diagram forgot: the pager.
- `convince-me` turns vague debate into a visible score.

The result is simple: better proposals, fewer vanity migrations, and substantially less "we'll figure out operations later."

## Why Install This

- Challenge weak proposals before they become expensive projects.
- Reuse consistent review workflows across agents and teams.
- Stress-test architecture, security, performance, product, and operations decisions.
- Add dry humor without turning every review into improv night.
- Get personalities that are opinionated, but not obstructionist.

## Quick Start

Install the repository:

```bash
npx skills@latest add mariusbreivik/engineering-personalities
```

Then install one or more personalities, for example:

- `senior-engineer`
- `principal-engineer`
- `security-team`
- `convince-me`

After installation, invoke them naturally in your agent:

- "Use `senior-engineer` to review this refactor proposal."
- "Run `security-team` against this auth design."
- "Ask `convince-me` whether this Kubernetes migration is justified."

## Start Here

If you do not want all twelve at once, start with this set:

- `senior-engineer`: the default daily reviewer
- `security-team`: the habit corrector
- `sre-oncall`: the operational reality check
- `convince-me`: the debate closer

That combination covers most bad ideas before they become documentation.

## Personalities

| Skill | What it does | Signature question |
| --- | --- | --- |
| [`senior-engineer`](./skills/senior-engineer/README.md) | Practical skepticism for day-to-day technical decisions | "What evidence do we have?" |
| [`principal-engineer`](./skills/principal-engineer/README.md) | Long-term thinking about ownership, cost, and complexity | "Who owns this in five years?" |
| [`staff-engineer`](./skills/staff-engineer/README.md) | Cross-team delivery, alignment, and system seams | "What coordination cost are we creating?" |
| [`architecture-review-board`](./skills/architecture-review-board/README.md) | Enterprise governance, interoperability, and standards review | "How does this fit the wider estate?" |
| [`security-team`](./skills/security-team/README.md) | Threat-model-driven review for auth, secrets, supply chain, and auditability | "How does this fail under active abuse?" |
| [`sre-oncall`](./skills/sre-oncall/README.md) | Uptime, observability, resilience, and incident readiness | "What happens at 03:00?" |
| [`qa-engineer`](./skills/qa-engineer/README.md) | Edge cases, reproducibility, and defect-oriented test design | "How do we make this fail on purpose?" |
| [`performance-engineer`](./skills/performance-engineer/README.md) | Benchmark-first performance review | "Where are the numbers?" |
| [`product-manager`](./skills/product-manager/README.md) | Customer value, prioritization, and ROI review | "Why does the user need this?" |
| [`convince-me`](./skills/convince-me/README.md) | Game-like structured persuasion with a live conviction meter | "What moved the percentage?" |
| [`legacy-maintainer`](./skills/legacy-maintainer/README.md) | Incremental change review for fragile long-lived systems | "What is the rollback plan?" |
| [`devils-advocate`](./skills/devils-advocate/README.md) | Intentional disagreement to expose unstated assumptions | "What if the opposite is true?" |

## What Makes These Different

Every personality follows the same core review loop:

1. Understand the proposal.
2. Identify assumptions.
3. Raise objections.
4. Ask questions.
5. Request evidence.
6. Reevaluate.
7. Produce a verdict.

The difference is what each personality notices first, what evidence it demands, and what kinds of trade-offs it will tolerate.

## Example

User:

> We want to split our monolith into six microservices this quarter so teams can move faster.

Principal Engineer:

> Before we celebrate future velocity, who owns service boundaries, on-call, schema evolution, and cross-service incidents?
>
> A distributed monolith is still a monolith, just with more dashboards.
>
> Show me:
>
> - the current bottleneck you have measured
> - which team owns each service in five years
> - the rollback path if service three becomes everyone's problem
>
> **Verdict:** Rejected pending evidence. Current proposal increases organizational and operational load faster than it reduces delivery friction.

## Compare The Voices

Same proposal. Different reviewers.

| Skill | Likely first reaction |
| --- | --- |
| `senior-engineer` | "What measured pain makes six services cheaper than a cleaner monolith?" |
| `principal-engineer` | "Who owns this in five years?" |
| `security-team` | "How do auth boundaries and secret distribution change across six services?" |
| `sre-oncall` | "What happens at 03:00 when service four fails and the others retry enthusiastically?" |
| `product-manager` | "What user problem improves enough to justify the migration cost?" |
| `convince-me` | "Current conviction: 8%. You brought ambition, not evidence." |

## Use Cases

- Refactor review before a large diff lands.
- Microservice proposals before someone acquires Kafka emotionally.
- Security review for auth, secrets, and third-party dependencies.
- Reliability review for rollouts, failover, and incident readiness.
- Product sanity checks for AI features and internal platform work.
- Legacy modernization without accidental business interruption.
