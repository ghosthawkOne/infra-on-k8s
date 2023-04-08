# Traefik

This release deploys the `traefik` Ingress controller to Kubernetes. This release is managed by `helmfile`, and as such you'll need to install `helmfile` mentioned within [the root README.md file](../../README.md)

The values that are passed onto the `helm` binary are specified within the file `values.yml.gotmpl`. Please refer to the [release page for `traefik` on artifacthub.io](https://artifacthub.io/packages/helm/traefik/traefik) for the full set of values that can be passed to this release.

The version of the `traefik` helm chart that would be deployed can be obtained from the file `helmfile.lock`. The version that would be deployed is specified within the list called `dependencies`. The object that you are looking for will have the key `name` set to `traefik`. The version of this release can be obtained from the field `version`.
