---
description: Forecast freshness, oracle capability, and execution gating inputs.
---

# deepbook\_forecast.move

## deepbook\_forecast.move

### Purpose

`deepbook_forecast` links forecast state to treasury execution policy.

It exists to gate actions on market freshness and forecast validity.

### Objects

* `OracleCap`
* `MarketForecast`
* DeepBook-linked forecast state

### Entry functions

Current documentation ties the module to forecast gating and mandate-linked market hooks.

### Events

Forecast lifecycle events are not yet listed as a standalone reference.

### Invariants

* stale forecasts must not pass as fresh
* execution can be blocked by forecast age
* forecast state must remain attributable to a treasury context

### Security model

Forecasts are used as execution gates, not marketing analytics.

### Dependencies

* `validation`
* `financial_mandate`
* market hook state

### Related pages

* [Programmable Money](../programmable-money/)
* [Security](../security/)
