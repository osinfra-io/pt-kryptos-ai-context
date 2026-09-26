---
applyTo: "**/pt-kryptos*/**"
---

# Kryptos Team Instructions

## Ownership Boundary

Kryptos owns secrets infrastructure, OpenBao configuration, authentication methods, policies, and secret-engine lifecycle. Pneuma owns the GKE clusters and cluster-level add-ons on which Kryptos runs.

## Deployment

Kryptos deploys zonal OpenBao workloads after the corresponding Pneuma runtime is available. Sandbox runs on pull requests, non-production runs after merge to `main`, and production runs only after non-production succeeds.

Consumers must use approved OpenBao authentication and policy paths. Do not store static credentials in repositories, OpenTofu variables, or CI environments.
