---
title: Front-end and Back-end Designs
tags:
  - architecture
  - design
---

# Front-end and Back-end Designs

## Back-end First Approach

The recommended best practice is to **start with the back-end** when building an IDP. This is similar to building a house—you start with the foundation, not the door.

## Front-end Design

The front-end focuses on **user interaction** and should NOT implement core business logic.

**Concerns with front-end first**:

- Violation of single responsibility principle
- Shoehorning logic into presentation layer
- Limited flexibility for other interfaces (CLI, API)

## Back-end Design

The back-end handles **standardization, security enforcement, automation, and orchestration**.

**Key aspects**:

- **Automation and standardization**: Consistent execution across environments
- **Lifecycle management**: Resource creation, updates, decommissioning
- **Enforcement by design**: Security, compliance, governance built-in
- **Orchestration**: Managing workflows and dependencies

## Backend Architectural Patterns

### Pipeline-based Backends

- Uses CI/CD pipelines (Jenkins, GitHub Actions, GitLab CI)
- Good for simpler use cases focused on environment progression
- Can become complex as platform scales

### Graph-based Backends (Platform Orchestrators)

- Uses tools like Humanitec, Kusion Stack, Kratix
- Manages relationships and dependencies as a graph
- Better for complex logic and scaling
- Developers describe desired state abstractly
