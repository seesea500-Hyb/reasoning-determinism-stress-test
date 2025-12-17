# Reasoning Determinism Stress Test

This repository documents a reproducible protocol for testing whether
AI reasoning remains structurally stable under repetition.

The focus is not on answers, accuracy, or model internals,
but on the behavior of reasoning when the same task is executed
multiple times under fixed conditions.

---

## What this is

This is a **stress test for reasoning determinism**.

It is designed to answer one narrow question:

> If the same reasoning task is run multiple times,
> does the underlying reasoning structure remain stable?

The protocol observes:
- decision points
- invariants
- assumption sets
- drift under repetition

---

## What this is NOT

This repository does **not** claim:
- correctness of answers
- model explainability
- safety guarantees
- general AI reliability
- access to model internals

It does not inspect weights, training data, or hidden states.
Only observable behavior is analyzed.

---

## Core idea

Determinism does **not** mean:
- identical wording
- identical length
- identical style

Determinism means:
- preservation of core invariants
- consistent decision anchors
- predictable variation zones
- detectable and classifiable drift

If reasoning collapses under repetition,
this protocol makes that collapse visible.

---

## Repository structure

- `PROTOCOL.md` — step-by-step test procedure
- `CLAIMS.md` — explicit, limited claims made by this work
- `LIMITATIONS.md` — known limitations and non-goals
- `cases/` — documented test cases
- `analysis/` — invariant and drift analysis artifacts

---

## How to falsify this

If you can:
- apply the same protocol,
- run the same task multiple times,
- and demonstrate stability where this repository shows collapse,
  or collapse where this repository shows stability,

please open an issue with evidence.

This work is intended to be **falsifiable**.

---

## Status

This repository is a living evidence log.
Content is added incrementally and conservatively.
