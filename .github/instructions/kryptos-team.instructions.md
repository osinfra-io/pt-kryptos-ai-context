---
applyTo: "**"
---

# Kryptos Team Instructions

## Ownership Boundary

Kryptos owns secrets infrastructure, OpenBao configuration, authentication methods, policies, and secret-engine lifecycle. Pneuma owns the GKE clusters and cluster-level add-ons on which Kryptos runs.

## Deployment

Kryptos deploys zonal OpenBao workloads after the corresponding Pneuma runtime is available. Sandbox runs on pull requests and applies only to sandbox environments using sandbox credentials. Non-production runs after merge to `main`, and production runs after non-production succeeds for automatic promotion; production can also run by manual dispatch without a successful non-production run. Pull-request runs must not have access to production or non-production credentials.

Consumers must use approved OpenBao authentication and policy paths. Do not store static credentials in repositories, OpenTofu variables, or CI environments.
