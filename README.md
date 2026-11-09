# Rakesh Gorige — Platform Engineering Portfolio

**Azure · Terraform · Kubernetes · GitHub Actions · Cloud Infrastructure**

This repository contains personal platform engineering builds, demonstrations, and design notes by **Rakesh Gorige** (Dallas, Texas). It is a portfolio of lab work, not a representation of production customer systems.

[GitHub profile](https://github.com/rakeshgorige) · [LinkedIn](https://www.linkedin.com/in/rakeshg1234567/)

## Featured project: PlatformOps Board

A three-tier operations dashboard with **Nginx, Python, and PostgreSQL**, Kubernetes deployment manifests, Terraform-defined Azure Kubernetes Service (AKS) and Azure Container Registry (ACR), and GitHub Actions CI/CD.

- Separate frontend, API, and PostgreSQL tiers.
- OIDC-based Azure deployment design, source-SHA image tags, health checks, and rollout verification.
- Network policies, non-root containers, resource limits, autoscaling configuration, and operational runbooks.
- **CI verified:** PostgreSQL integration, container builds, end-to-end smoke tests, restart persistence, Kubernetes schema checks, and Terraform validation.
- **Not yet verified:** deployment to a live AKS cluster remains a documented acceptance step.

[Project README](three-tier-platform/README.md) · [Architecture](three-tier-platform/docs/architecture.md) · [Demo walkthrough](three-tier-platform/docs/demo.md) · [Verification status](three-tier-platform/docs/verification.md)

## Azure platform delivery lab

A Terraform-driven static website deployment with GitHub Actions and Azure OIDC federation. The design separates Terraform state from application resources and includes validation, saved-plan apply, RBAC, deployment concurrency, and a content smoke test.

[Architecture and engineering case study](docs/azure-platform-lab.md)

The source infrastructure repository is private; the public case study describes the implementation without disclosing account configuration.

## Design principles

1. **Repeatable infrastructure:** declare resources, isolate state, and document provisioning boundaries.
2. **Secure delivery:** favor short-lived identities and scoped cloud permissions.
3. **Operability:** validate before release, record verification evidence, and document troubleshooting.
4. **Developer experience:** provide practical runbooks and clear setup instructions.

## Scope and attribution

This repository contains personal engineering and learning work. CI checks do not prove successful live cloud deployment. Course-derived or third-party content elsewhere on this account should retain appropriate attribution.

**Maintainer: Rakesh Gorige**
