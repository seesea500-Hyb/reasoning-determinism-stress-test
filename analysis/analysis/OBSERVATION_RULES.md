# Observation Rules (v1)

This document defines how observations are recorded in this repository.

## Scope

Observations document **what changes** and **what remains stable** under repeated execution of a fixed task.
They do not explain causes.

## Constraints

- Observations do not speculate about hidden model state or internals.
- Observations do not claim performance, correctness, or intelligence.
- Observations must reference a concrete case file (path under `cases/`).

## Recording format

Each observation entry must include:
- **ID** (e.g., `OBS-01`)
- **Phenomenon** (what is being tracked)
- **Status** (Stable / Conditionally Stable / Degraded)
- **Evidence** (a direct link or path to the case file)
- **Notes** (short, concrete)

## Non-goals

- No interpretation of intent.
- No causal attribution.
- No benchmarking claims.
