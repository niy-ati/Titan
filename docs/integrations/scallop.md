---
description: Mainnet lending integration for deposit, withdraw, and position reads.
---

# Scallop

## Scallop

### What it is

Scallop is a second lending target in TITAN’s deployment layer.

### Why it exists

It expands capital routing beyond a single lender and enables comparative allocation.

### How it works

The SDK adapter exposes deposit, withdraw, and position-access logic. The UI desk and allocation path consume that adapter.

### Where it lives

* `@mandateos/sdk` DeFi adapters
* `/app/scallop-capital`
* Allocation Engine
* Portfolio position reads

### Current status

**Implemented** for desk wiring and position reads.

**Not Yet Verified** for end-to-end proof evidence.

### References

* [Capital Deployment](../capital-deployment/)
* [DeFi Final Verification](../references/reports/defi_final_verification.md)
