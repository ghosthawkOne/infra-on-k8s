# infra-on-k8s

Contains various pieces of infrastructure (Databases, monitoring, etc.) that can be deployed to a kubernetes cluster

## Getting started

You will need the following tools:

1. A Kubernetes cluster (each helm release was tested against a Kubernetes cluster started by Docker for Windows Desktop on Windows 10)

2. [`helm`](https://github.com/helm/helm/releases)

3. [`helmfile`](https://github.com/helmfile/helmfile/releases)

4. [`kubectl`](https://kubernetes.io/docs/tasks/tools/)

5. [The `helm diff` plugin](https://github.com/databus23/helm-diff)

## Applications covered

This repository covers the following applications:

1. [Traefik](helmfile-releases/traefik)

2. [Cert-manager](helmfile-releases/cert-manager/) and [Issuers](helmfile-releases/cert-manager-issuers/)
