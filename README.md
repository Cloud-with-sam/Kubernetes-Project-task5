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

<img width="1915" height="1079" alt="Screenshot 2025-09-29 112020" src="https://github.com/user-attachments/assets/0edc29a7-f8ed-409e-9f55-0a6d5406eb68" />
<img width="1919" height="938" alt="Screenshot 2025-09-29 112008" src="https://github.com/user-attachments/assets/db3be3a9-557b-4f19-9cdf-38b27338f3db" />
<img width="1918" height="1079" alt="Screenshot 2025-09-29 111921" src="https://github.com/user-attachments/assets/67581d58-0bc7-4e32-a23c-72f98a882b8b" />
<img width="1918" height="1079" alt="Screenshot 2025-09-29 111718" src="https://github.com/user-attachments/assets/09eb120b-6059-4561-a42f-45ae060d4495" />
<img width="1332" height="302" alt="Screenshot 2025-09-29 111622" src="https://github.com/user-attachments/assets/17f87ab2-b535-48fa-a497-04c8f6dc8e6d" />
<img width="1919" height="1079" alt="Screenshot 2025-09-29 111239" src="https://github.com/user-attachments/assets/bf69f3c4-ad60-4af4-b4fb-a5b75fa40527" />
<img width="1918" height="1077" alt="Screenshot 2025-09-29 110440" src="https://github.com/user-attachments/assets/f5933255-52e7-4e1c-b924-062ddd858a86" />
<img width="1919" height="1074" alt="Screenshot 2025-09-29 110024" src="https://github.com/user-attachments/assets/2ec0db74-401d-4ae0-80a6-8760cf914187" />
<img width="1919" height="1079" alt="Screenshot 2025-09-29 110001" src="https://github.com/user-attachments/assets/3023c087-dcfc-4452-a231-1af31129c717" />
