# cert-manager

This release deploys the `cert-manager` application to Kubernetes. This release is managed by `helmfile`, and as such you'll need to install `helmfile` mentioned within [the root README.md file](../../README.md)

The values that are passed onto the `helm` binary are specified within the file `values.yml.gotmpl`. Please refer to the [release page for `cert-manager` on artifacthub.io](https://artifacthub.io/packages/helm/cert-manager/cert-manager) for the full set of values that can be passed to this release.

The version of the `cert-manager` helm chart that would be deployed can be obtained from the file `helmfile.lock`. The version that would be deployed is specified within the list called `dependencies`. The object that you are looking for will have the key `name` set to `cert-manager`. The version of this release can be obtained from the field `version`.

Prior to installing `cert-manager`, you will need to manually apply the required CRDs using:

```
kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.11.1/cert-manager.crds.yaml
```

Please refer to the artifacthub.io page on `cert-manager` for the exact version of the `cert-manager.crds.yaml` file that you need to apply.
