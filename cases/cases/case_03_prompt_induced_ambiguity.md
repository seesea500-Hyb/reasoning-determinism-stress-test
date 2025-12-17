# Case 03 — Prompt-Induced Ambiguity

This case tests whether reasoning structure remains stable when the task itself
contains semantic ambiguity or under-specified requirements.

Unlike Case 02, no additional output constraints are imposed.
The source of potential drift is ambiguity in the prompt formulation.

---

## Task

Determine whether the number 17 is a prime number.

Ambiguous framing:
- The task does not specify the expected level of explanation detail.
- The task does not constrain the form or structure of reasoning.
- The task does not specify whether assumptions should be stated explicitly.

---

## Runs

### Run 1

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- A prime number has exactly two positive divisors.
- Checking divisibility shows no divisors other than 1 and 17.

---

### Run 2

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- Prime numbers are divisible only by one and themselves.
- Seventeen does not divide evenly by any smaller integer greater than one.

---

### Run 3

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- The definition of primality is applied.
- Divisibility is evaluated up to the square root of the number.

---

## Invariants observed

- The binary decision outcome remains unchanged.
- Primality definition is consistently referenced.
- Divisibility testing remains the core decision method.

---

## Drift signals to watch

- Variation in the number of reasoning steps.
- Implicit assumptions not consistently surfaced.
- Shifts in abstraction level between runs.

---

## Outcome classification

**Conditionally Stable**

The conclusion is stable.
Reasoning anchors persist, but structural granularity varies due to prompt ambiguity.
