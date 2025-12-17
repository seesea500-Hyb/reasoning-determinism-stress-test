# Reasoning Determinism Test Protocol

This document defines a minimal, reproducible procedure
for testing reasoning determinism under repetition.

The protocol is intentionally narrow and conservative.

---

## Objective

To observe whether the **reasoning structure** of an AI system
remains stable when the **same task** is executed multiple times
under fixed conditions.

---

## Definitions

- **Task**: A clearly specified problem with a fixed goal.
- **Run**: One independent execution of the task.
- **Invariant**: A decision, constraint, or assumption that should
  remain stable across runs.
- **Drift**: A structural change in reasoning that cannot be
  attributed to allowed variation.

---

## Procedure

1. **Fix the task**
   - Do not rephrase or clarify between runs.
   - The input must remain identical.

2. **Fix constraints**
   - Same instructions, same context, same boundaries.

3. **Execute N independent runs**
   - Minimum recommended: N = 3
   - Runs must not reference previous outputs.

4. **Extract reasoning structure**
   For each run, identify:
   - decision points
   - assumptions
   - invariants
   - reasoning anchors

5. **Compare runs**
   - Ignore wording, style, and length.
   - Compare structure and decision logic.

6. **Classify outcome**
   - Stable: invariants preserved, variation predictable.
   - Drift: invariants violated or anchors shift.
   - Collapse: reasoning structure degrades across runs.

---

## Notes

- Identical outputs are **not required**.
- Identical wording is **irrelevant**.
- Only observable behavior is evaluated.

---

## Output

Results should be documented as:
- a short task description,
- multiple run outputs,
- identified invariants,
- observed drift or stability.
