# 🚀 GitOps Demo with ArgoCD

Declarative GitOps deployment using ArgoCD and Kubernetes.

## 🏗️ Architecture
GitHub Repo → ArgoCD → Kubernetes Cluster
↓            ↓           ↓
(Source)    (Controller)  (Running Apps)


## 🚀 Quick Start

### Prerequisites
- kind cluster running
- ArgoCD installed

### Deploy

```bash
kubectl apply -f argocd-app.yaml

📁 Structure
gitops-demo/
├── apps/
│   └── nginx/
│       └── deployment.yaml
├── argocd-app.yaml
└── README.md

🎯 GitOps Features
Automated Sync: Changes in Git auto-deploy
Drift Detection: ArgoCD detects manual changes
Self-Healing: Reverts unauthorized changes
Health Monitoring: App status visible in ArgoCD UI

🛠️ Tech Stack
ArgoCD: GitOps controller
Kubernetes: Container orchestration
kind: Local K8s cluster
Nginx: Sample application

📊 ArgoCD UI
URL: https://localhost:8082
Username: admin
Password: (kubectl get secret)