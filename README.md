# SiteWhere Operator based on Helm

## Install

```console
kubectl create -f deploy/service_account.yaml
kubectl create -f deploy/role.yaml
kubectl create -f deploy/role_binding.yaml
kubectl create -f deploy/crds/sitewhere_v1alpha1_sitewhere_crd.yaml
kubectl create -f deploy/operator.yaml
kubectl create -f deploy/crds/sitewhere_v1alpha1_sitewhere_cr.yaml
```

## Cleanup

```console
kubectl delete -f deploy/crds/sitewhere_v1alpha1_sitewhere_cr.yaml
kubectl delete -f deploy/operator.yaml
kubectl delete -f deploy/role.yaml
kubectl delete -f deploy/role_binding.yaml
kubectl delete -f deploy/service_account.yaml
kubectl delete -f deploy/crds/sitewhere_v1alpha1_sitewhere_crd.yaml
```