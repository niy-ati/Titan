---
description: Create a treasury mandate, vault, and supporting objects.
---

# Treasury Creation

## Treasury creation

Treasury creation is the root workflow.

It establishes the on-chain object graph that every later workflow uses.

```mermaid
sequenceDiagram
  participant U as User
  participant UI as Command Center
  participant SDK as MandateOSClient
  participant MO as MandateOS

  U->>UI: choose template or custom treasury
  UI->>SDK: buildCreateTreasuryTx
  SDK->>MO: create treasury mandate
  MO-->>UI: mandate, vault, constitution, config, caps
```

### Objects created

* `FinancialMandate`
* `MandateVault`
* `FinancialConstitution`
* treasury config and delegation objects
* forecast and governance-linked capabilities

### Current status

Chain verified on testnet.

### References

* [Treasury System](../treasury-system/)
* [MandateOS — Treasury Flow (Testnet)](treasury_demo.md)
