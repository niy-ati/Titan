---
description: Pre-settlement checks that enforce treasury and workflow correctness.
---

# validation.move

## validation.move

### Purpose

`validation` enforces correctness before settlement.

It prevents a workflow from executing against invalid or stale state.

### Objects

Validation witnesses and check outputs are consumed by settlement flows.

### Entry functions

Current documentation references validation as part of simulation, workflow, guardian, and forecast-gated execution.

### Events

Validation outcomes are mainly observable through downstream success or abort behavior.

### Invariants

* invalid state must fail closed
* workflow and forecast checks must run before settlement
* treasury protection rules cannot be bypassed

### Security model

Validation is one of TITAN’s fail-closed layers.

### Dependencies

* `simulation`
* `workflow`
* `deepbook_forecast`
* `guardian`

### Related pages

* [Execution](../workflows/execution.md)
* [Security](../security/)
