# How to deploy

## Install dependencies
1. Kubernetes cluster
2. Install Ingress Controller
3. Install Argocd (in argocd namespace)

## Create Ingress for ArgoCD Server (UI)
```bash
  kubectl apply -f argocd-config/argocd-server-ingress.yaml
```

## Create applications
```bash
  kubectl apply -f apps/dev-application.yaml
  kubectl apply -f apps/staging-application.yaml
```
