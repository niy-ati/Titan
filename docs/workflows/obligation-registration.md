---
description: Register treasury obligations before simulation and execution.
---

# Obligation Registration

## Obligation registration

Obligations express what the treasury owes.

They are the input for simulations, workflows, and downstream receipts.

```mermaid
sequenceDiagram
  participant U as User
  participant UI as Command Center
  participant SDK as MandateOSClient
  participant MO as MandateOS

  U->>UI: define obligation
  UI->>SDK: buildRegisterObligationTx
  SDK->>MO: register obligation
  MO-->>UI: updated obligation registry
```

### Current status

Chain verified on testnet.

### References

* [Treasury System](../treasury-system/)
* [Judge Flow](judge_flow.md)
