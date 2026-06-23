---
description: Guardian policy, automated restriction, and emergency treasury controls.
---

# guardian.move

## guardian.move

### Purpose

`guardian` enforces emergency or corrective policy actions.

It exists to stop unsafe treasury behavior before or during execution.

### Objects

* `GuardianPolicy`
* guardian action state

### Entry functions

Current documentation confirms evaluate, simulate, and execute action flows.

### Events

Guardian actions appear in proof and audit records.

### Invariants

* guardian actions stay tied to a treasury mandate
* restricted state must be explicit
* corrective actions cannot skip validation

### Security model

The guardian is a policy control, not a general executor.

It blocks, restricts, or redirects behavior when treasury conditions demand it.

### Dependencies

* `operational_risk`
* `workflow`
* `simulation`
* `validation`

### Related pages

* [Security](../security/)
* [Smart Wallet Rules](../smart-wallet-rules/)
