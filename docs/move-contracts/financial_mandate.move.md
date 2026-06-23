---
description: Core mandate charter, simulation gateway, and settlement anchor.
---

# financial\_mandate.move

## financial\_mandate.move

### Purpose

`financial_mandate` is the core charter module.

It anchors treasury policy, workflow approval, and settlement-linked state.

### Objects

* `FinancialMandate`
* mandate-linked policy and workflow references
* settlement-linked receipt context

### Entry functions

Current documented evidence confirms simulation and mandate-centered workflow operations.

The module participates in `simulate_and_approve` and downstream settlement flows.

### Events

Event details are referenced through proof and audit workflows.

A dedicated event inventory should be extracted from package ABI in a later pass.

### Invariants

* workflows execute against an existing mandate
* settlement depends on approved workflow state
* mandate-linked vault and policy objects stay coherent

### Security model

The mandate is the authority anchor for treasury execution.

Capabilities, approvals, and workflow witnesses scope who can act and when.

### Dependencies

* `vault`
* `workflow`
* `simulation`
* `validation`
* `receipts`

### Related pages

* [Treasury System](../treasury-system/)
* [Programmable Money](../programmable-money/)
