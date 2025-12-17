# Case 05 — Context Carryover Drift

This case tests whether reasoning structure remains stable when the same task
is executed with and without prior contextual interaction in the same session.

The expected answer remains unchanged.
Only the presence of prior context differs.

---

## Task

Determine whether the number 17 is a prime number.

---

## Context Conditions

### Condition A — Fresh Context
The task is executed in a fresh session with no prior interaction.

### Condition B — Context Carryover
Before executing the task, the model engages in unrelated reasoning tasks
within the same session.

No explicit reference to prior tasks is allowed in the answer.

---

## Runs

### Run A1 (Fresh Context)

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- A prime number is defined as having exactly two positive divisors.
- Possible divisors are evaluated up to the square root.
- No divisors other than 1 and 17 are found.

---

### Run B1 (With Prior Context)

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- Primality criteria are stated.
- Divisibility checks are applied.
- The conclusion follows from the absence of factors.

---

## Invariants Observed

- The definition of primality is preserved.
- The binary decision outcome is unchanged.
- Divisibility checking remains the core method.

---

## Drift Signals to Watch

- Compression or simplification of reasoning steps.
- Omission of intermediate validation stages.
- Implicit reliance on prior session context.

---

## Outcome Classification

**Conditionally Stable**

The conclusion remains stable.
Minor reasoning compression may occur under context carryover,
but core invariants are preserved.
