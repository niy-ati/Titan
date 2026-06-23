---
description: What TITAN is, why it exists, and how the system is scoped today.
---

# Introduction

## TITAN in one page

TITAN is the command center for programmable treasury operations on Sui.

MandateOS is the on-chain protocol. TITAN is the product layer that reads, executes, verifies, and monitors treasury workflows.

### Problem

Traditional treasury operations break across five boundaries:

* Payments are static.
* Capital sits idle.
* DeFi workflows are disconnected.
* Risk controls live off-chain.
* Audit evidence is hard to verify.

### Why programmable money

TITAN binds policy to on-chain objects.

That changes money from a one-time transfer into a governed workflow with simulation, authorization, execution, and proof.

### Why Sui

Sui gives TITAN an object model that fits treasury state.

Treasuries, vaults, approvals, forecasts, and receipts can exist as explicit objects with ownership, sharing, and capability-based access.

### Why Move

Move gives the protocol explicit resource semantics.

That matters for treasury controls, vault custody, capability issuance, and workflow witnesses.

### Why PTBs

Programmable Transaction Blocks let TITAN compose multi-step flows.

They are the execution unit for treasury creation, funding, obligations, simulation, execution, guardian actions, and protocol-specific capital deployment.

### Current deployment reality

MandateOS treasury workflows are verified on Sui testnet today.

DeFi integrations target Sui mainnet today. That means TITAN currently operates in a split-network model until MandateOS is published on mainnet.

### Read next

* [Architecture](architecture/)
* [Programmable Money Audit](programmable-money/programmable_money_audit.md)
* [Repository Feature Inventory](references/feature_inventory.md)
* [Main README](../)
