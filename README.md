# Kubernetes Minikube Nginx Deployment

This project demonstrates how to run a simple Nginx web server on a local Kubernetes cluster using Minikube on Windows.

It includes:

- A Deployment with 2 replicas of the Nginx container
- A Service of type NodePort to expose the app to your browser
- Steps to scale, roll out updates, and access the app
- Screenshot proof of working pods, service, and UI

---

## 🔧 Prerequisites

- Windows 10/11
- Docker Desktop (with WSL2 backend enabled)
- Minikube
- kubectl
- PowerShell or VS Code terminal

---

## 📁 Files in this Repo

| File             | Description                       |
|------------------|------------------------------------|
| deployment.yaml  | Kubernetes deployment for nginx    |
| service.yaml     | NodePort service to expose nginx   |
| README.md        | This file                          |

---

## 🚀 Steps to Run

### 1. Start Minikube

Make sure Docker Desktop is running, then start Minikube using the Docker driver:

```powershell
minikube start --driver=docker