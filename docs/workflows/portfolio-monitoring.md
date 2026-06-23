---
description: Observe treasury, protocol, and proof-backed portfolio state after execution.
---

# Portfolio Monitoring

## Portfolio monitoring

Portfolio monitoring closes the workflow loop.

It shows whether treasury actions changed balances, positions, and exposure the way the workflow intended.

```mermaid
sequenceDiagram
  participant UI as Portfolio UI
  participant RPC as Sui RPC
  participant AD as DeFi Adapters
  participant PF as Proof Center

  UI->>RPC: fetch wallet and vault state
  UI->>AD: fetch protocol positions
  UI->>PF: load proof-linked activity
  RPC-->>UI: treasury balances
  AD-->>UI: positions
  PF-->>UI: verified activity context
```

### References

* [Portfolio](../portfolio/)
* [Production Reality Audit](../references/reports/production_reality_audit.md)
