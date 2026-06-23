---
description: >-
  Practical SDK usage patterns across treasury, workflow, proof, and protocol
  actions.
---

# Usage examples

## Usage examples

The SDK serves four primary product jobs.

It reads state, builds PTBs, verifies proofs, and normalizes protocol integrations.

### Example categories

#### Treasury

Create a mandate, fund a vault, and register obligations through transaction builders.

#### Workflow

Simulate first, then execute with the approval object returned by the simulation path.

#### Proof

Export proof records and verify each digest against Sui RPC.

#### DeFi

Build wallet-signed protocol transactions for Navi, Scallop, and Cetus.

### What matters most

The SDK is not a generic helper package.

It is the execution and interpretation layer between product flows and chain state.

### Read next

* [Readers and clients](readers-and-clients.md)
* [Config system and type definitions](config-system-and-type-definitions.md)
* [Audit & Proof System](../audit-and-proof-system/)
