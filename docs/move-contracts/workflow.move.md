---
description: Session control, authorization flow, and execution sequencing.
---

# workflow.move

## workflow.move

### Purpose

`workflow` coordinates execution state.

It tracks the path from approved intent to settled action.

### Objects

* workflow session state
* execution authorization witnesses

### Entry functions

Current evidence confirms session opening and workflow-linked settlement paths.

### Events

Workflow activity is visible through proof capture and receipt issuance.

### Invariants

* settlement requires an authorized workflow path
* approval state must match execution state
* receipts must reflect the executed session

### Security model

The module prevents direct settlement without the right witness chain.

### Dependencies

* `simulation`
* `validation`
* `receipts`
* `financial_mandate`

### Related pages

* [Simulation](../workflows/simulation.md)
* [Execution](../workflows/execution.md)
