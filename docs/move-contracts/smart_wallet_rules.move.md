---
description: Satellite automation rules for workflow-linked treasury actions.
---

# smart\_wallet\_rules.move

## smart\_wallet\_rules.move

### Purpose

`smart_wallet_rules` is the satellite automation module.

It lets TITAN create and execute rule objects outside the core package.

### Objects

* rule objects for balance, payroll, and risk triggers

### Entry functions

Current documentation confirms rule creation and rule execution.

### Events

Rule execution is proof-linked and chain verified.

### Invariants

* rules stay attached to workflow intent
* rule execution stays within the published rule type model
* proof and event output must remain attributable

### Security model

Automation remains explicit and wallet-linked.

Autonomous keeper execution is not documented as verified.

### Dependencies

* workflow-linked product flows
* proof and audit capture

### Related pages

* [Smart Wallet Rules](../smart-wallet-rules/)
* [Smart Wallet Rules Verification](../smart-wallet-rules/smart_wallet_rules_verification.md)
