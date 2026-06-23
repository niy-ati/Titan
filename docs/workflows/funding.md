---
description: Move capital into a treasury vault and record the funding state.
---

# Funding

## Funding

Funding turns an empty treasury graph into an executable treasury.

The vault must hold usable balance before obligations and workflow execution matter.

```mermaid
sequenceDiagram
  participant U as User
  participant UI as Command Center
  participant SDK as MandateOSClient
  participant MO as MandateOS

  U->>UI: select amount to fund
  UI->>SDK: buildFundVaultTx
  SDK->>MO: fund treasury vault
  MO-->>UI: updated vault balance
```

### Current status

Chain verified on testnet.

### References

* [Treasury Creation](treasury-creation.md)
* [Programmable Money Audit](../programmable-money/programmable_money_audit.md)
