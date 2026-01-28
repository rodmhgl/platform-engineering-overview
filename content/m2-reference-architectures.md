---
title: Reference Architectures
tags:
  - architecture
  - examples
  - module-2
order: 4
aliases:
  - Module-2/reference-architectures
---

## What are Reference Architectures?

Reference Architectures serve as **proven blueprints and helpful standards** for understanding and discussing complex platform engineering setups. They were initially launched at PlatformCon 2023.

## Platform Planes

Reference architectures break down an IDP into logical layers or "planes":

### Developer Control Plane

- **Primary interface** for developers and platform engineers
- Includes developer portals like Backstage
- Service catalogues and version control

### Integration and Delivery Plane

- **CI/CD pipelines** and automation logic
- Container registries
- Platform Orchestrators for deployment

### Resource Plane

- **Underlying infrastructure** (cloud, on-prem, hybrid)
- Compute, storage, networking
- Kubernetes clusters

### Monitoring and Logging Plane

- Observability tools
- Logging aggregation
- Metrics collection

### Security Plane

- Identity and access management
- Secrets management
- Key management services

## Getting Started

**Start with the back-end first**:

1. Focus on core logic for automation and standardization
2. Establish solid foundation before building UI
3. Avoid shoehorning logic into front-end
4. Enable future flexibility for multiple interfaces

## Resources

- [Platform Engineering Reference Architectures](https://platformengineering.org)
