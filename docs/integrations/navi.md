---
description: Mainnet lending integration for deposit, withdraw, and position reads.
---

# Navi

## Navi

### What it is

Navi is one of TITAN’s capital deployment targets.

### Why it exists

It provides lending-based yield deployment for treasury capital.

### How it works

The SDK builds wallet-signed deposit and withdraw flows. The UI desk exposes those flows and reads resulting positions.

### Where it lives

* `@mandateos/sdk` DeFi adapters
* `/app/navi-capital`
* Allocation Engine
* Portfolio position reads

### Current status

**Implemented** for desk wiring and position reads.

**Not Yet Verified** for full reference proof coverage.

### References

* [Capital Deployment](../capital-deployment/)
* [Judge Readiness Report](../audit-and-proof-system/judge_readiness_report.md)
