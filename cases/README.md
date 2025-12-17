# Test Cases

This directory contains documented reasoning determinism test cases.

Each case follows the protocol defined in `PROTOCOL.md`
and documents observable reasoning behavior across multiple runs.

---

## Case format

Each test case should include:

- a fixed task description,
- multiple independent runs,
- identified invariants,
- observed drift or stability,
- a short structural analysis.

---

## Naming convention

Cases are named sequentially:

- `case_01_basic_task.md`
- `case_02_constraint_variation.md`
- `case_03_drift_emergence.md`

---

## Note

Cases are added conservatively.
A single well-documented case is preferable
to many weak or ambiguous ones.
