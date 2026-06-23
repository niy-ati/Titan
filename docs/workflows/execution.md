---
description: Settle an approved workflow and emit final receipts.
---

# Execution

## Execution

Execution consumes approved state and performs the treasury action.

This is where value moves and proof is created.

```mermaid
sequenceDiagram
  participant E as Executor
  participant MO as MandateOS
  participant R as Recipient
  participant PF as Proof Center

  E->>MO: execute approved workflow
  MO->>R: transfer or settlement action
  MO-->>E: FinancialReceipt
  E->>PF: record digest and outputs
```

### Outputs

* treasury state changes
* receipt objects
* events
* proof records

### References

* [Audit & Proof System](../audit-and-proof-system/)
* [Programmable Money Audit](../programmable-money/programmable_money_audit.md)
