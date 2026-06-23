---
description: Simulation approval objects and dry-run authorization logic.
---

# simulation.move

## simulation.move

### Purpose

`simulation` turns a candidate workflow into an approval object.

It is the pre-settlement control layer.

### Objects

* `SimulationApproval`

### Entry functions

Current evidence confirms simulate-and-approve behavior through the shim and treasury workflows.

### Events

Approval creation is visible through object changes and proof output.

### Invariants

* execution depends on a valid approval
* approval must match the intended workflow
* approval transfer remains explicit

### Security model

Simulation prevents direct execution without policy review.

### Dependencies

* `workflow`
* `validation`
* PTB shim client flow

### Related pages

* [Simulation workflow](../workflows/simulation.md)
* [Deployed System Diagrams](../audit-and-proof-system/proof/diagrams.md)
