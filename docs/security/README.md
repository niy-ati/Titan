---
description: Ownership, capabilities, authority, reserve protection, and execution gating.
---

# Security

## Security

TITAN uses object ownership, capabilities, validation witnesses, and proof re-verification as its core control model.

### Security boundaries

* Governor-owned authority
* Scoped executor delegation
* Vault access through workflow witnesses
* Forecast freshness gates
* Guardian emergency actions
* Reserve and liquidity controls

### High-level model

```mermaid
flowchart LR
  G[Governor] --> C[Capabilities]
  C --> E[Executor]
  E --> W[Workflow witness]
  W --> V[Vault action]
  G --> GP[Guardian policy]
  GP --> B[Block or restrict]
```

### Source evidence

* [README](../../)
* [Mainnet Readiness Report](../deployment/mainnet_readiness_report.md)

### Related pages

* [Guardian System](guardian-system.md)
* [Forecast System](../programmable-money/forecast-system.md)
