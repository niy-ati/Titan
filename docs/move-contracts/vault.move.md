---
description: Treasury custody, balance state, and vault-linked workflow execution.
---

# vault.move

## vault.move

### Purpose

`vault` holds treasury assets.

It is the custody layer for mandate-controlled balances.

### Objects

* `MandateVault<T>`
* vault-linked balance and reserve state

### Entry functions

Current workflow evidence confirms treasury funding and execution read or mutate vault state.

### Events

Vault changes surface through transaction effects and proof-linked object changes.

### Invariants

* vault actions require valid mandate context
* workflow execution cannot bypass custody rules
* balances must reconcile with on-chain effects

### Security model

Direct treasury execution does not treat the vault as a free wallet.

Workflow approval and authority checks gate state changes.

### Dependencies

* `financial_mandate`
* `workflow`
* `validation`
* `adaptive_liquidity`

### Related pages

* [Funding](../workflows/funding.md)
* [Portfolio](../portfolio/)
