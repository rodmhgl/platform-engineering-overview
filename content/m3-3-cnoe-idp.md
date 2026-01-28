---
title: "Module 3-3: CNOE Reference Implementation"
tags:
  - cnoe
  - open-source
  - module-3
order: 3
aliases:
  - m3-cnoe-idp
  - Module-3/cnoe-idp
---

# Open Source IDP with Backstage and ArgoCD built with CNOE

## What is CNOE?

CNOE (Cloud Native Operational Excellence) is a framework for scaffolding an Internal Developer Platform using **pipeline-based backend** architecture.

## Key Components

- **Argo Workflows and ArgoCD**: CI/CD and continuous delivery
- **Git**: Version control
- **Container registry**: Image storage
- **Backstage**: Developer portal (optional)

## Architecture

```
Developer Control Plane → Integration/Delivery Plane → Resource Plane
     (Backstage)         (ArgoCD, Argo Workflows)      (Kubernetes)
```

## Important Note

CNOE serves as a **foundational tool** for building an IDP and may require further customization to establish clear separation of concerns between development and operations teams.

## Repository

[CNOE Setup Guide](https://github.com/InternalDeveloperPlatform/pe-course-labs/blob/main/cnoe.md)
