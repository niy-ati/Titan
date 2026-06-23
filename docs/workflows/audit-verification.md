---
description: Export, inspect, and independently verify workflow proof artifacts.
---

# Audit Verification

## Audit verification

Audit verification turns product activity into third-party evidence.

It is the final step for judges, auditors, and operators who need independent confirmation.

```mermaid
sequenceDiagram
  participant U as User
  participant PF as Proof Center
  participant RPC as Sui RPC
  participant R as Report

  U->>PF: export proof document
  PF->>RPC: verify digests and effects
  RPC-->>PF: transaction data
  PF-->>R: verified or invalid report
```

### References

* [Audit & Proof System](../audit-and-proof-system/)
* [Judge Verification Pack](../audit-and-proof-system/proof/)
