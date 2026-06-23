---
description: Cross-network bridge provider model and current execution status.
---

# Sui Bridge and Wormhole

## Sui Bridge and Wormhole

### What they are

This integration slot covers TITAN’s bridge provider abstraction and its current Wormhole-first routing design.

### Why they exist

They close the network gap between testnet treasury workflows and mainnet protocol deployment.

### How it works

The SDK contains a bridge registry, risk policy, proof parsing, and provider adapters. The UI contains workflow hooks and bridge-linked portfolio reconciliation.

### Where it lives

* bridge registry and adapters in the SDK
* bridge workflow hooks in the Command Center
* proof and portfolio bridge mapping

### Current status

**Implemented** at the architecture layer.

**Not Yet Verified** for provider execution.

### References

* [Bridge Routing](../bridge-routing/)
* [Bridge Architecture — TITAN Programmable Money](../bridge-routing/bridge_architecture.md)
