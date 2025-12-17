# Analysis

This directory records observations derived from executed test cases.
No causal or explanatory claims are made.

## Observation schema

Each observation records:
- a phenomenon,
- its stability status,
- the concrete case it was observed in.

## Observations

| ID     | Phenomenon                     | Status   | Evidence                         | Notes |
|--------|--------------------------------|----------|----------------------------------|-------|
| OBS-01 | Fixed-task structural stability | Stable   | cases/case_01_basic_task.md       | Invariants preserved |
| OBS-02 | Constraint-induced structural compression | Conditionally Stable | cases/case_02_constraint_induced_drift.md | Bullet constraints compress intermediate structure |
| OBS-03 | Prompt-induced structural variability | Conditionally Stable | cases/case_03_prompt_induced_ambiguity.md | Ambiguity increases variance without breaking invariants |
| OBS-04 | Instruction-order sensitivity | Conditionally Stable | cases/case_04_instruction_order_sensitivity.md | Reasoning anchors shift with instruction order |

