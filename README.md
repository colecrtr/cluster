# cluster

## Dependencies

- [Helm](https://helm.sh/)
- [Helmfile](https://github.com/roboll/helmfile)
  - Used for declarative Helm config and bootstrapping the cluster
  - Requires [Helm Diff Plugin](https://github.com/databus23/helm-diff)

## Instructions

Verify the Kubernetes cluster in current context:
```shell script
kubectl config current-context
```

Apply resources:
```shell script
helmfile apply
kubectl apply -f manifests/
```
