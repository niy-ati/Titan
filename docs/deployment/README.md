---
description: >-
  Testnet deployment, production UI deployment, and mainnet readiness
  boundaries.
---

# Deployment

## Deployment

TITAN has two deployment surfaces today:

* MandateOS packages on Sui testnet
* Command Center on a production HTTPS origin

### Why that split matters

Treasury workflows execute against the published MandateOS testnet package.

DeFi protocol integrations target mainnet adapters. That creates a documented split-network deployment until mainnet MandateOS publish is complete.

### Covered deployment domains

* protocol publish and upgrade
* UI environment configuration
* proof and verification scripts
* mainnet readiness gaps

### Source evidence

* [MandateOS — Sui Testnet Deployment](deployment.md)
* [Deployment Checklist](deployment_checklist.md)
* [Mainnet Readiness Report](mainnet_readiness_report.md)
