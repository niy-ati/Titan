---
description: Scoped executor delegation and authority transfer for treasury actions.
---

# delegation.move

## delegation.move

### Purpose

`delegation` issues controlled execution authority.

It lets a governor separate ownership from operational action.

### Objects

* `DelegationCap`
* `ExecutorCap`

### Entry functions

Current evidence confirms executor-cap issuance and delegated execution paths.

### Events

Delegation appears through object creation and later workflow use.

### Invariants

* delegated execution stays inside cap limits
* delegation is treasury-scoped
* authority expiry and masks must hold at execution time

### Security model

Delegation is capability-based.

That keeps operational authority narrower than treasury ownership.

### Dependencies

* `authority`
* `workflow`
* `financial_mandate`

### Related pages

* [Delegation workflow](../workflows/delegation.md)
* [Security](../security/)
