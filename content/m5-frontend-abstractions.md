---
title: Frontend Abstractions
tags:
  - abstractions
  - frontend
  - module-5
order: 2
aliases:
  - Module-5/frontend-abstractions
---

# Frontend Abstractions

## Purpose

Frontend abstractions focus on **ergonomics and design**, simplifying how users interact with the platform by hiding complex details behind simpler interfaces.

## Types of Frontend Abstractions

### Developer Portals

- **Backstage** (open source)
- **Cortex**
- **Port**

Provide visual access to platform capabilities and system status.

### Command Line Interfaces (CLIs)

- Heroku CLI
- GitHub CLI
- Custom platform CLIs

### Declarative Configuration Tools

- **Score**: Platform-agnostic workload specification
- **Radius**: Application graph-based config
- **KubeVela**: OAM-based abstractions

### Natural Language Interfaces

Emerging capability for platform interaction.

## Design Principles

Effective frontend abstractions should be:

- **Visual**: Charts, graphs for clarity
- **Easy to use**: Simple commands and defaults
- **Collaborative**: Input from various personas

## Meeting Developers Where They Are

Consider offering multiple interfaces:

- UI for visibility and management
- CLI for developers who prefer terminal
- Code-based for GitOps workflows

This prevents low adoption from forcing developers out of preferred workflows.
