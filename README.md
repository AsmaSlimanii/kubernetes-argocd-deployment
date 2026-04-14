# Kubernetes + ArgoCD Deployment 🚀

## Overview
GitOps-based deployment of a Python Flask application on Kubernetes
using ArgoCD for continuous delivery.

## Architecture
GitHub → ArgoCD → Kubernetes → Flask App

## Tech Stack
- Kubernetes (Minikube) — Container Orchestration
- ArgoCD — GitOps Continuous Delivery
- Docker — Containerization
- Python Flask — Web Application
- GitHub — Source Control

## Kubernetes Resources
- Deployment (2 replicas)
- Service (NodePort)

## How to Run
# Start Minikube
minikube start

# Install ArgoCD
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

# Apply manifests
kubectl apply -f k8s/

# Access the app
minikube service flask-app-service

## Author
Asma Slimani — Junior DevOps Engineer
LinkedIn : https://www.linkedin.com/in/asma-slimani-4a732a296/
GitHub   : https://github.com/AsmaSlimanii
