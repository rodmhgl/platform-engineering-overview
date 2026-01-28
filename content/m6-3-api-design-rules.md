---
title: "Module 6-3: Rules for Designing APIs for Platforms"
tags:
  - api
  - design
  - module-6
order: 3
aliases:
  - m6-api-design-rules
  - Module-6/api-design-rules
---

# Rules for Designing APIs for Platforms

## Importance

A well-designed platform API serves as the **connection point** between different parts of the platform, facilitating integration and automation of features into external processes like CI/CD pipelines.

## Key Principles

### Ubiquitous API

- **Same API** for front-end interactions and underlying services
- Promotes consistency
- Simplifies platform communication

### Interface Agnostic

- Recognize users have existing workflows and preferences
- Support various interfaces: APIs, CLIs, UIs equally
- **API-first approach** facilitates building other interfaces on top

### Prepared for Complex Back-end Logic

- Complexity should be **contained within the back-end**
- Process of binding back-end to uniform front-end should be simple
- Platform orchestrators abstract away this complexity

## Platform Orchestrators as Primary API

Platform orchestrators act as the **primary API layer**, providing:

- Self-service capabilities
- Consistent, easily accessible interface
- Abstraction over complexity
- Connection between resource definitions and Infrastructure as Code

## Result

By following these rules, you create platform APIs that are:

- Consistent
- User-friendly
- Effective at managing underlying infrastructure complexity
- Foster better collaboration and efficiency
