---
description: >-
  Mainnet concentrated liquidity integration for LP deployment and position
  reads.
---

# Cetus

## Cetus

### What it is

Cetus is TITAN’s concentrated-liquidity deployment target.

### Why it exists

It adds LP exposure to the treasury deployment layer.

### How it works

The SDK adapter builds LP actions and reads resulting positions. TITAN uses that adapter in the Cetus desk and allocation views.

### Where it lives

* `@mandateos/sdk` DeFi adapters
* `/app/cetus-capital`
* Allocation Engine
* Portfolio position reads

### Current status

**Implemented** for desk wiring and position reads.

**Not Yet Verified** for end-to-end proof evidence.

### References

* [Capital Deployment](../capital-deployment/)
* [Mainnet Readiness Report](../deployment/mainnet_readiness_report.md)
