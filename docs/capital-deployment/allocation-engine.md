---
description: >-
  Policy-aware capital routing across treasury buckets and protocol
  destinations.
---

# Allocation Engine

## Allocation engine

The allocation engine turns treasury intent into deployment buckets.

It decides how much capital should move and where it should go.

### Responsibilities

The engine considers:

* available treasury capital
* reserve constraints
* target protocol mix
* execution sequencing

### Routing model

Today the engine routes through wallet-signed protocol actions.

It can split deployment across multiple desks, but execution remains sequential.

### Current status

* Allocation flows are implemented.
* Multi-desk product routing exists.
* A single unified multi-protocol PTB remains planned.

### Read next

* [Capital Deployment](./)
* [Allocation](../workflows/allocation.md)
* [Portfolio](../portfolio/)
