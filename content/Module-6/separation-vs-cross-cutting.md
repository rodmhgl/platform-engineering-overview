---
title: Separation of Concerns vs Cross-cutting Concerns
tags:
  - architecture
  - concerns
---

# Separation of Concerns vs Cross-cutting Concerns

## Separation of Concerns

An architectural principle emphasizing **division of responsibilities** within a platform.

### Key Distinction

- **Application source code**: Owned by application teams (product code)
- **Platform source code**: Owned by platform teams (infrastructure, resource definitions, automation)

### Benefits

- Teams specialize in their domains
- Reduced cognitive load
- More maintainable and understandable systems

### Implementation

Well-defined APIs serve as **handover points** between application developers (managing workload specs and application logic) and platform engineers (managing IaC and resource definitions).

## Cross-cutting Concerns

Aspects that **permeate all layers and components** of the platform, regardless of separation of concerns.

### Examples

- Security
- Compliance
- Observability
- Cost management (FinOps)

### Handling Cross-cutting Concerns

These concerns are often **embedded into platform source code**, particularly within:

- Resource definitions
- Automation processes
- Managed by platform engineering team in collaboration with security and finance teams

### Why This Matters

When developers provision resources through self-service:

- Cross-cutting concerns are **automatically addressed**
- Individual application teams don't handle intricate security/compliance details
- Consistent and governed self-service experience

## Balance

While separation of concerns promotes focus and maintainability, cross-cutting concerns define **overarching requirements** that must be consistently applied across all separated domains.
