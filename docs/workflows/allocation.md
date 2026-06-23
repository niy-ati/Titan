---
description: Route capital across protocol desks and record the resulting deployment state.
---

# Allocation

## Allocation

Allocation distributes capital across deployment targets.

In the current product, that routing is sequential and wallet-signed.

```mermaid
sequenceDiagram
  participant U as User
  participant AL as Allocation Engine
  participant N as Navi
  participant S as Scallop
  participant C as Cetus

  U->>AL: choose split
  AL->>N: deposit leg
  AL->>S: deposit leg
  AL->>C: deposit leg
```

### Current status

Implemented in the product.

Full chain-verified reference evidence for the whole allocation path is still pending.

### References

* [Capital Deployment](../capital-deployment/)
* [Judge Readiness Report](../audit-and-proof-system/judge_readiness_report.md)
