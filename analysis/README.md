# Analysis

This directory contains observational analysis derived from executed test cases.

The purpose of this analysis is not interpretation or explanation,
but structured recording of what remains stable and what degrades
under repeated reasoning execution.

All observations reference concrete cases and runs.

---

## Observation schema

Each observation records:

- invariant or anchor being observed
- preservation status under repetition
- evidence reference (case / run)
- notes limited to observable behavior

No causal claims are made.

---

## Observations

| Observation ID | Invariant / Anchor            | Status       | Evidence                  | Notes |
|---------------|-------------------------------|--------------|---------------------------|-------|
| OBS-01        | Task framing consistency      | Preserved    | case_01_basic_task / run1-3 | Framing remains identical |
| OBS-02        | Decision path ordering        | Preserved    | case_01_basic_task / run1-3 | Same logical sequence |
| OBS-03        | Constraint interpretation     | Degraded     | case_02_constraint_induced_drift / run2 | Constraint reweighted |

---

## Notes

- “Preserved” means structurally consistent, not textually identical.
- “Degraded” means detectable shift in anchors or weighting.
- Absence of observation does not imply absence of behavior.
