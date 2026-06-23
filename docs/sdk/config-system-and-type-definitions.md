---
description: Package configuration, network targeting, package IDs, and shared SDK typing.
---

# Config system and type definitions

## Config system and type definitions

The SDK depends on explicit network and package configuration.

That configuration keeps builders and readers pointed at the right chain objects.

### Configuration scope

Key configuration covers:

* Sui network
* MandateOS package IDs
* PTB shim package ID
* protocol adapter settings
* proof and explorer endpoints

### Type system role

Shared types define treasury objects, workflow state, protocol positions, proof records, and route metadata.

They let the UI compose product views without duplicating chain logic.

### Why this matters

A programmable treasury stack fails quickly when IDs drift.

Centralized config reduces that risk.

Shared types also prevent route and workflow mismatches across product surfaces.

### Current status

* Package and network configuration are implemented.
* Type definitions cover treasury, proof, and protocol workflows.
* Some future route types remain integration-ready rather than fully exercised.

### Read next

* [SDK](./)
* [Deployment](../deployment/)
* [Bridge Routing](../bridge-routing/)
