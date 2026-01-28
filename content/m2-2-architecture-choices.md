---
title: "Module 2-2: Platform Architecture Choices"
tags:
  - architecture
  - design
  - module-2
order: 2
aliases:
  - m2-architecture-choices
  - Module-2/architecture-choices
---

# Platform Architecture Choices

## Key Decisions

When designing your IDP, consider:

- **Build vs Buy**: Which components to build internally vs adopt
- **Centralized vs Federated**: Level of platform team control
- **Opinionated vs Flexible**: How much choice to give developers

## Architecture Patterns

### Fully Managed

- Platform team owns and operates everything
- Maximum standardization
- Lower developer flexibility

### Self-Service with Guardrails

- Developers choose within boundaries
- Balance of flexibility and control
- Most common approach

### Federated

- Multiple teams contribute components
- Higher coordination overhead
- Suits large organizations
