# Limitations

This document lists the known limitations and non-goals
of the reasoning determinism protocol documented in this repository.

These limitations are intentional.

---

## Methodological limitations

- The protocol does not provide access to model internals.
- It does not explain *why* a model reasons in a certain way.
- It cannot distinguish between coincidental stability and causal stability.
- It relies entirely on observable outputs.

---

## Scope limitations

- Results apply only to the specific tasks tested.
- Results do not generalize across models, versions, or configurations.
- Results do not imply future stability.

---

## What this protocol cannot do

This protocol cannot:

- guarantee correctness of reasoning,
- guarantee safety or alignment,
- certify models or systems,
- prevent hallucinations,
- enforce determinism.

It can only **observe and document behavior**.

---

## Interpretation warning

Stability under this protocol does not imply:
- correctness,
- truth,
- intelligence,
- reliability outside tested conditions.

Instability under this protocol does not imply:
- uselessness,
- failure in all contexts,
- lack of capability.

---

## Rationale

The purpose of this protocol is **visibility**, not control.
