# Kustomization for deploying Argo CD Operator to OpenShift

This kustomization uses [Argo CD Operator](https://github.com/argoproj-labs/argocd-operator) to deploy Argo CD to OpenShift. The Argo CD Operator documentation can be found [here](https://argocd-operator.readthedocs.io/en/latest/).

## Quick start

Note that some of the following commands require *cluster-admin* role.

Install Argo CD Operator:
```
$ oc apply --kustomize argocd-operator/base
```

Deploy a Argo CD instance:
```
$ oc apply --kustomize argocd-instance/overlays/basic
```
