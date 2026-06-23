---
description: >-
  Bridge provider registry, execution boundaries, and SDK routing
  responsibilities.
---

# Bridge registry and execution layer

## Bridge registry and execution layer

The SDK carries the routing model for bridge-aware workflows.

It separates route definition from route execution.

### Bridge registry

The bridge registry defines known providers, route metadata, supported networks, and provider-specific constraints.

This is where Sui Bridge and Wormhole fit into the system model.

### Execution layer

The execution layer turns an approved route into a signer-ready transaction plan.

It also carries cost, risk, and readiness checks.

### Current boundary

Bridge routing architecture exists.

Verified production bridge execution does not.

That distinction matters across the product and proof model.

### Why it exists

Cross-chain treasury movement needs more than a target chain.

It needs provider selection, route validation, and proof-safe execution boundaries.

### Read next

* [Bridge Routing](../bridge-routing/)
* [Sui Bridge and Wormhole](../integrations/sui-bridge-and-wormhole.md)
* [SDK](./)
