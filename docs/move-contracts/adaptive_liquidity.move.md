---
description: Reserve protection, liquidity posture, and treasury preservation logic.
---

# adaptive\_liquidity.move

## adaptive\_liquidity.move

### Purpose

`adaptive_liquidity` protects treasury liquidity.

It exists to preserve reserves and constrain unsafe capital deployment.

### Objects

* reserve covenant state
* liquidity engine state

### Entry functions

Current documentation references reserve and liquidity behavior through treasury, policy, and guardian flows.

### Events

Event details are not yet broken out as a standalone inventory.

### Invariants

* reserve protection takes precedence over aggressive deployment
* treasury liquidity posture must remain inspectable
* guardian and policy layers can rely on its state

### Security model

The module acts as a capital-preservation boundary.

### Dependencies

* `vault`
* `operational_risk`
* `guardian`

### Related pages

* [Programmable Money](../programmable-money/)
* [Capital Deployment](../capital-deployment/)
