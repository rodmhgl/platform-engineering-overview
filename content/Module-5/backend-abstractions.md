---
title: Backend Abstractions
tags:
  - abstractions
  - backend
---

# Backend Abstractions

## Purpose

Backend abstractions are primarily concerned with **automation and lifecycle management** of resources. They deal with **one specific aspect across many things simultaneously**.

## Three-Tier Abstraction Model

| Layer | Why and How | Who | What | Example Tech |
|-------|-------------|-----|------|--------------|
| **Application Choreography** | Deliver value to customers | App developers, DevOps, SREs | UI, CLI, Declarative config, NLI | Backstage, Port, Heroku CLI, Score, Radius |
| **Platform Orchestration** | Provide x-as-a-service, automation, fleet management | App devs, Platform engineers, Enablement, SREs | Platform Orchestrators | Kratix Promise, Humanitec Resource Definitions, Crossplane Compositions |
| **Infrastructure Orchestration** | Provide infrastructure building blocks | App devs, Platform engineers, DevOps, Operators, Sysadmins | IaC, Resource Definitions, Resource Graphs | Terraform, Crossplane, Ansible, Humanitec Resource Definitions |

*Based on: Daniel Bryant, Platform Engineering: Orchestrating Applications, Platforms, and Infrastructure*

## Key Principles

### Full Automation for Self-Service

If a developer isn't permitted to provide a specific detail, **the platform must supply it**—avoiding "TicketOps."

### Platform Orchestrators as Central API

Platform Orchestrators (Humanitec, Kratix, KusionStack) provide:

- **Logical abstraction** over infrastructure
- **Decoupling** from specific implementations
- **Consistent interface** across the platform

## Resource Definitions

Backend abstractions like:

- Humanitec's resource definitions
- Kratix's recipes in Radius
- Crossplane's promises

Guide Platform Orchestrators in fulfilling requests from front-end abstractions like Score.
