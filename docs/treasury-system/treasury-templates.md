---
description: >-
  Template catalog, intended use cases, created objects, and current
  implementation status.
---

# Treasury Templates

## Treasury templates

Templates package treasury intent into repeatable starting points.

They reduce setup time without changing the core object model.

### How templates work

A template preselects a treasury posture.

That posture defines expected objectives, obligation types, reserve behavior, and likely workflows.

The final treasury still resolves to the same on-chain primitives:

* `FinancialMandate`
* `MandateVault`
* `FinancialConstitution`
* `ObligationRegistry`

### Template catalog

#### Startup treasury

Use this for runway management and controlled operating spend.

It emphasizes cash preservation, recurring obligations, and simple delegation.

#### DAO treasury

Use this for governance-driven pooled capital.

It emphasizes shared policy, mandate transparency, and execution controls.

#### Payroll treasury

Use this for salary and contractor disbursements.

It emphasizes scheduled obligations, budget tracking, and execution discipline.

#### Investment treasury

Use this for yield deployment and portfolio construction.

It emphasizes allocation policy, reserve thresholds, and protocol exposure.

#### Creator treasury

Use this for revenue intake and programmed payouts.

It emphasizes split logic, recurring disbursement, and transparent accounting.

#### Protocol treasury

Use this for treasury operations inside a protocol team.

It emphasizes policy enforcement, runway visibility, and capital deployment.

### What templates influence

Templates can shape:

* default mandate framing
* obligation and payment patterns
* reserve and liquidity posture
* execution workflows surfaced in the UI

### What templates do not change

Templates do not create a separate protocol.

They are product presets over one treasury architecture.

### Current status

* Template-driven treasury creation is implemented in product flows.
* Multiple treasury archetypes exist in the catalog.
* Some templates remain product-facing classifications rather than fully distinct on-chain objects.

### Read next

* [Treasury System](./)
* [Treasury Account](treasury-account.md)
* [Workflows](../workflows/)
* [Feature Inventory](../references/feature_inventory.md)
