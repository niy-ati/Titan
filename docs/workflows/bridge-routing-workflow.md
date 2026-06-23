---
description: Route capital across networks under bridge risk and proof constraints.
---

# Bridge Routing Workflow

## Bridge routing workflow

Bridge routing sits between allocation and destination deployment.

It is designed into the stack, but it is not yet a verified runtime path.

```mermaid
sequenceDiagram
  participant T as Treasury Context
  participant BR as Bridge Router
  participant BP as Bridge Provider
  participant DN as Destination Network

  T->>BR: request route
  BR->>BR: validate route and policy
  BR->>BP: build provider tx
  BP->>DN: relay asset
```

### Current status

Architecture exists.

Provider execution remains blocked pending dependency verification.

### References

* [Bridge Routing](../bridge-routing/)
* [Bridge Architecture — TITAN Programmable Money](../bridge-routing/bridge_architecture.md)
