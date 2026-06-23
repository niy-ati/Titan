---
description: Read and write layers in @mandateos/sdk and how they map to product workflows.
---

# Readers and clients

## Readers and clients

The SDK splits chain reads from transaction building.

This keeps product views and execution flows separate.

### Reader layer

Readers fetch object state, balances, positions, receipts, and proof-linked data.

They back treasury, portfolio, and proof surfaces.

### Client layer

Clients build PTBs for treasury, workflow, guardian, rule, and protocol actions.

They do not custody keys.

A wallet signs the final transaction.

### Why the split exists

Read paths need stable aggregation.

Write paths need explicit signer control and deterministic transaction assembly.

### Product usage

* treasury creation and funding use client builders
* portfolio and account screens use readers
* proof verification uses proof-specific read paths

### Current status

* Reader and client layers are implemented.
* Treasury and workflow builders are wired into the product.
* Mainnet-unified programmable money remains pending mainnet protocol deployment.

### Read next

* [SDK](./)
* [Workflows](../workflows/)
* [Move Contracts](../move-contracts/)
