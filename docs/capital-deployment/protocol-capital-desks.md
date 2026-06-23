---
description: Navi, Scallop, and Cetus deployment surfaces and how they differ.
---

# Protocol capital desks

## Protocol capital desks

TITAN exposes dedicated desks for each supported deployment venue.

Each desk wraps a specific protocol adapter and transaction builder path.

### Navi Capital

Navi is used for lending-style deployments.

It supports deposit, withdraw, and position reads.

Status: Implemented.

### Scallop Capital

Scallop is used for lending-style deployments with its own adapter path.

It supports deposit, withdraw, and position reads.

Status: Implemented.

### Cetus Capital

Cetus is used for concentrated liquidity deployments.

It supports LP-oriented actions and position reads.

Status: Implemented.

### Why separate desks exist

Each protocol has different state models and execution parameters.

Separate desks keep those constraints explicit.

### Read next

* [Navi](../integrations/navi.md)
* [Scallop](../integrations/scallop.md)
* [Cetus](../integrations/cetus.md)
* [Integrations](../integrations/)
