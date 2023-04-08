# Traefik

This release deploys the `traefik` Ingress controller to Kubernetes. This release is managed by `helmfile`, and as suck you'll need to install `helmfile` mentioned within [the root README.md file](../../README.md)

The values that are passed onto the `helm` binary are specified within the file `values.yml.gotmpl`.

The version of the `traefik` helm chart that would be deployed can be obtained from the file `helmfile.lock`. The version that would be deployed is specified within the list called `dependencies`. The object that you are looking for will have the key `name` set to `traefik`. The version of this release can be obtained from the field `version`.
