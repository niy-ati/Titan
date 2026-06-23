---
description: Reader, writer, product, proof, DeFi, and bridge layers in @mandateos/sdk.
---

# SDK

## SDK

`@mandateos/sdk` is the execution and read layer between TITAN and MandateOS.

It owns PTB builders, on-chain readers, protocol adapters, product models, proof verification, and bridge scaffolding.

### Layer map

* `MandateOSClient` for writes
* `MandateOSReader` for reads
* product models for portfolio, templates, and routing
* protocol adapters for Navi, Scallop, and Cetus
* proof verification helpers

### Why it matters

The SDK is the single integration boundary for both the UI and non-UI tooling.

That keeps treasury execution, proof verification, and protocol access consistent across flows.

### Section pages

* [Readers and clients](readers-and-clients.md)
* [Config system and type definitions](config-system-and-type-definitions.md)
* [Bridge registry and execution layer](bridge-registry-and-execution-layer.md)
* [Usage examples](usage-examples.md)

### Source evidence

* [Repository Feature Inventory](../references/feature_inventory.md)
* [Product Architecture](../architecture/architecture.md)
