---
description: Treasury objectives, obligation registry, and execution intent inputs.
---

# objectives.move

## objectives.move

### Purpose

`objectives` stores what the treasury is trying to achieve and what it is required to satisfy.

It is the business-policy layer for obligations and goals.

### Objects

* objective-linked mandate state
* `ObligationRegistry`

### Entry functions

Current product evidence confirms obligation registration and objective reads.

### Events

Obligation changes appear through transaction effects and audit history.

### Invariants

* obligations must belong to the treasury context
* simulation reads current objective state
* execution outcomes must remain attributable to tracked obligations

### Security model

Objectives do not move funds alone.

They feed validation, simulation, and workflow decisions.

### Dependencies

* `financial_mandate`
* `workflow`
* `simulation`

### Related pages

* [Obligation Registration](../workflows/obligation-registration.md)
* [Programmable Money](../programmable-money/)
