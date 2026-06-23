---
description: Reference coverage for the rest of the MandateOS core package.
---

# Remaining core modules

## Remaining core modules

This page covers the remaining core modules that are present in the v5 package but not yet broken into their own pages in this pass.

### Shared and authority modules

* `mandateos` — package init and admin entry surface
* `types` — shared structs and enums
* `authority` — role and permission wiring
* `receipts` — audit and settlement receipts

### Policy and intent modules

* `rules` — rule graph structure
* `constitutional` — enforceable treasury limits
* `operational_risk` — risk profile and stress-mode controls
* `intent` — workflow intent objects
* `intent_compiler` — intent-to-plan compilation
* `templates` — on-chain template registry

### Treasury and workflow-specific modules

* `treasury_mandate` — treasury account lifecycle
* `dao_treasury_mandate` — DAO treasury variant
* `payroll_mandate` — payroll workflow
* `subscription_mandate` — recurring payment workflow
* `revenue_allocation_mandate` — revenue split workflow
* `auto_investment_mandate` — investment workflow

### Status

These modules are included in the documented package inventory.

Workflow-level evidence exists across treasury, payroll, revenue, investment, delegation, guardian, and proof flows. Function-by-function ABI extraction is still pending for this grouped set.

### References

* [Repository Feature Inventory](../references/feature_inventory.md)
* [README module table](../../)
