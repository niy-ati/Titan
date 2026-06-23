---
description: Dry-run validation and approval generation before settlement.
---

# Simulation

## Simulation

Simulation is the policy checkpoint before execution.

It evaluates whether a workflow should be approved under the current treasury state.

```mermaid
sequenceDiagram
  participant U as User
  participant SH as PTB Shim
  participant MO as MandateOS
  participant A as Approval Object

  U->>SH: simulate and approve
  SH->>MO: open simulation and run projection
  MO-->>SH: validation result
  SH-->>A: SimulationApproval object
```

### Output

Simulation produces an approval witness that later execution consumes.

### References

* [Move Contracts](../move-contracts/)
* [Deployed System Diagrams](../audit-and-proof-system/proof/diagrams.md)
