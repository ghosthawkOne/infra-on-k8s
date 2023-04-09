# cert-manager-issuers

This release creates a `ClusterIssuer` CRD instance from `cert-manager`.

You need to install [`cert-manager`](../cert-manager/) before installing this.

## Deploying

1. Install the [`cert-manager` release](../cert-manager/)

2. Execute `helmfile [-e <environmentName>] apply`
