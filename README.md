# crossplane

## Prerequisites

- kubectl 
- helm
- a local Kubernetes cluster, or any Kubernetes cluster
- access to the account e.g. Azure or Google where you want to provision your infrastructure

[Authentication mechanisms supported by provider-azure](https://github.com/upbound/provider-azure/blob/main/AUTHENTICATION.md)


> code 
```
kubectl create namespace crossplane-system

helm repo add crossplane-stable https://charts.crossplane.io/stable
helm repo update

helm install crossplane --namespace crossplane-system crossplane-stable/crossplane
```