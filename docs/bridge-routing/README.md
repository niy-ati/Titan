---
description: >-
  Cross-chain architecture, provider model, route policy, and verification
  gates.
---

# Bridge Routing

## Bridge routing

Bridge routing is part of programmable capital deployment.

It is not treated as a standalone product path.

### Current architecture

The SDK contains route catalogs, provider abstractions, risk policy, proof parsing, and portfolio reconciliation support.

The Command Center contains wallet-linked bridge workflow hooks and proof recording.

### Execution boundary

Architecture exists.

Verified runtime execution does not exist yet.

```mermaid
flowchart LR
  T[Treasury] --> A[Allocation]
  A --> B[Bridge provider]
  B --> D[Destination network]
  D --> P[DeFi protocol]
  P --> R[Portfolio reconcile]
```

### Current provider posture

* Bridge registry exists.
* Wormhole-first routing is designed.
* Provider PTBs remain blocked pending configuration and verification.

### Source evidence

* [Bridge Architecture — TITAN Programmable Money](bridge_architecture.md)
* [Mainnet Readiness Report](../deployment/mainnet_readiness_report.md)
