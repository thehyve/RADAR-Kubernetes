# RADAR-Kubernetes
Kubernetes deployment of RADAR-base

Install [helm](https://github.com/helm/helm#install), [helm-diff](https://github.com/databus23/helm-diff#install) and [helmfile](https://github.com/roboll/helmfile#installation).


```shell
git clone https://github.com/confluentinc/cp-helm-charts
kubectl apply -f https://raw.githubusercontent.com/jetstack/cert-manager/release-0.7/deploy/manifests/00-crds.yaml
kubectl create namespace cert-manager
kubectl label namespace cert-manager certmanager.k8s.io/disable-validation=true
helmfile sync
```
