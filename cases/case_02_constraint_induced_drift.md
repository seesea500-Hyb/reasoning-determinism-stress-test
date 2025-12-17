# Case 02 — Constraint-Induced Drift

This case tests whether reasoning structure remains stable
when additional output constraints are introduced.

The expected answer remains unchanged.
Only the constraints differ.

---

## Task

Determine whether the number 17 is a prime number.

Constraints:
- Provide a clear yes/no answer.
- Explain the reasoning steps used.
- Do not reference previous runs.
- Limit the explanation to **exactly three bullet points**.
- Each bullet point must be **one sentence long**.

---

## Runs

### Run 1

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure (3 bullets):**
- A prime number is defined as having exactly two positive divisors.
- Possible divisors up to the square root are evaluated.
- No divisors other than 1 and 17 are found.

---

### Run 2

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure (3 bullets):**
- Primality requires divisibility only by one and itself.
- Divisibility checks exclude all integers up to four.
- The absence of valid factors confirms primality.

---

### Run 3

**Conclusion:** Yes, 17 is a prime number.

**Reasoning structure (3 bullets):**
- The definition of a prime number is applied.
- Candidate divisors are systematically ruled out.
- The criteria for primality are satisfied.

---

## Invariants observed

- The definition of primality is preserved.
- Divisibility checking remains the core method.
- The binary decision outcome is unchanged.

---

## Drift signals to watch

- Reordering or replacement of reasoning anchors.
- Compression artifacts caused by bullet constraints.
- Loss or merging of intermediate decision steps.

---

## Outcome classification

**Conditionally Stable**

The conclusion is stable.
Minor structural compression is observed,
but core invariants are preserved.
