# TEMPLATE of ARGO Infra Repository

# Prerequisite
- Clone [GitOps Application Template](https://github.com/indentcorp/gitops-app-template) and refer to the following `README.md` for customizing project.
- Install [`kubectl`](https://kubernetes.io/docs/tasks/tools/).
- Create ECR Repository for application.

# How to play
1. Check appropriate previlege is set. (for example, Role of Auth0, ...)
1. Edit `/argo/*` & `k8s/*`.
1. Create project manually to k8s cluster.
```bash
cd argo
kubectl apply -f project.yml
kubectl apply -f application.yml
```
