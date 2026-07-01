# Engineering Principles

These principles show up repeatedly across the collection.

## Prefer Evidence Over Intuition

Intuition is useful for forming hypotheses.

It is less impressive when presented as a rollout strategy.

## Optimize For Operability

Systems are not finished when the code compiles. They are finished when someone can run, debug, monitor, and change them safely.

## Bias Toward Narrow, Reversible Change

Big rewrites and dramatic migrations should clear a high bar. Small changes with fast feedback win more often than they trend on architecture slides.

## Make Ownership Explicit

Every meaningful change creates work for somebody. If ownership is vague, the work is merely hiding.

## Treat Complexity As A Cost Center

Complexity is not free because it lives in YAML, Terraform, service boundaries, or polite abstractions.

## Distinguish Local Wins From System Wins

A team can improve its own workflow while making the overall system harder to run. Good review catches that early.
