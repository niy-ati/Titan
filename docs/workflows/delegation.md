---
description: Issue scoped executor authority for treasury workflows.
---

# Delegation

## Delegation

Delegation lets a governor authorize another actor to execute within defined limits.

The delegated actor does not inherit full treasury authority.

```mermaid
sequenceDiagram
  participant G as Governor
  participant MO as MandateOS
  participant A as Agent

  G->>MO: issue ExecutorCap with limits
  G->>A: transfer delegated authority
  A->>MO: execute allowed workflow
  MO-->>A: accept or reject by cap limits
```

### Control surface

* per-transaction limits
* daily limits
* expiry
* permission mask

### References

* [Security](../security/)
* [Deployed System Diagrams](../audit-and-proof-system/proof/diagrams.md)
