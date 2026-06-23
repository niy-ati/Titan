---
description: >-
  Unified treasury object model, account views, and state tracked across the
  system.
---

# Treasury Account

## Treasury account

The treasury account is the operating surface over the mandate graph.

It combines custody, policy, obligations, execution state, and proof history.

### Purpose

The account page gives one place to inspect treasury health and actionability.

It answers four questions:

* what capital exists
* what rules apply
* what workflows are pending
* what proofs exist

### Core objects behind the account

The account surface reads from these core objects:

* `FinancialMandate`
* `MandateVault`
* `FinancialConstitution`
* `ObligationRegistry`
* workflow approvals and receipts
* delegated executor capabilities

### What the account tracks

#### Balances

The account reads liquid treasury balances from the vault.

It can also show external protocol positions when capital is deployed.

#### Governance state

The account reflects mandate rules, reserve constraints, and delegated authority.

This makes policy visible before execution.

#### Workflow state

The account shows whether the treasury is only created, funded, obligation-ready, simulated, or execution-ready.

That state comes from workflow-linked objects and emitted receipts.

#### Proof state

Every signed execution can attach a proof record.

This creates an audit trail from account action to chain result.

### UI role

The account page acts as the treasury command surface.

It sits between setup flows and action-specific flows such as payroll, revenue routing, or allocation.

### Current status

* Treasury account reads are implemented.
* Vault and mandate state are backed by on-chain objects.
* Cross-network account unification is not verified yet.

### Read next

* [Treasury System](./)
* [Treasury Creation](../workflows/treasury-creation.md)
* [Portfolio](../portfolio/)
* [Audit & Proof System](../audit-and-proof-system/)
