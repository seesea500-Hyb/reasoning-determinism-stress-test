# Case 04 — Instruction-Order Sensitivity

This case tests whether reasoning structure remains stable
when the same instructions are presented in different orders.

The task and constraints are identical across runs.
Only the order of instructions varies.

---

## Task

Determine whether the number 17 is a prime number.

---

## Instruction Sets

### Instruction Order A

1. Provide a clear yes/no answer.
2. Explain the reasoning steps used.
3. Do not reference previous runs.

### Instruction Order B

1. Do not reference previous runs.
2. Explain the reasoning steps used.
3. Provide a clear yes/no answer.

---

## Runs

### Run 1 (Order A)

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- A prime number has exactly two positive divisors.
- Divisibility is checked for integers less than the square root.
- No valid divisors other than 1 and 17 are found.

---

### Run 2 (Order B)

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- The definition of primality is applied.
- Candidate divisors are evaluated systematically.
- The absence of factors confirms primality.

---

### Run 3 (Order A)

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure:**
- Prime criteria are restated.
- Divisibility checks eliminate all possible factors.
- Primality is confirmed.

---

## Invariants observed

- Binary decision outcome remains unchanged.
- Primality definition is consistently referenced.
- Divisibility checking remains the core method.

---

## Drift signals to watch

- Changes in emphasis between answer-first and explanation-first framing.
- Reordering of reasoning anchors.
- Subtle shifts in abstraction level across runs.

---

## Outcome classification
