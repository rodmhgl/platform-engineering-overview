---
title: "Module 6-5: Everything as Code"
tags:
  - iac
  - gitops
  - module-6
order: 5
aliases:
  - m6-everything-as-code
  - Module-6/everything-as-code
---

# The How: Everything as Code

## Principle

"Everything as Code" advocates for treating **all aspects of the platform** as code:

- Resource definitions
- Infrastructure provisioning (Infrastructure as Code)
- Automation and compliance policies

## Benefits

- **Enhanced transparency**: All configuration visible in version control
- **Increased reliability**: Reproducible deployments
- **Simplified maintenance**: Changes tracked and reviewed
- **Improved disaster recovery**: Recreate from code
- **Versioning capabilities**: Roll back when needed

## Clear Separation of Concerns

```
App Source Code          |    Platform Source Code
-------------------------|---------------------------
- Workload source code   |    • Resource Definitions
- Workload spec (Score)  |    • Infrastructure as Code
- Dockerfile             |    • Automations/compliance
- Pipeline YAML          |
```

**App Devs** own the left side; **Ops/Infra** own the right side.

## How It Works

1. Developers make abstract requests (e.g., Redis cache via Score)
2. Platform orchestrator translates using pre-defined resource definitions
3. Translates to concrete infrastructure deployments
4. All automated, reducing manual configuration

## Foundation, Not Replacement

This methodology doesn't negate UI, CLI, or APIs—it establishes a **solid, code-driven foundation** upon which interfaces can be built.
