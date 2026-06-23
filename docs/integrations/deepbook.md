---
description: Order-book market data integration for Sui-native liquidity views.
---

# DeepBook

## DeepBook

### What it is

DeepBook is the Sui-native order-book data source in TITAN.

### Why it exists

It gives the Liquidity Terminal live CLOB context instead of generic yield-only data.

### How it works

TITAN reads DeepBook data through a proxy-backed indexer path.

The data feeds market tables and protocol detail views.

### Where it lives

* Liquidity Terminal data layer
* Vercel proxy `/api/deepbook`
* SDK and UI market adapters

### Current status

**Live** for data reads.

### References

* [Liquidity Terminal](../liquidity-terminal/)
* [Repository Feature Inventory](../references/feature_inventory.md)
