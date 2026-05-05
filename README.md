# 🚀 Kubernetes Deployment Assignment

---

## 📌 Overview

This project demonstrates deployment of a **versioned frontend application** using **Docker** and **Kubernetes**.

Two versions of the application are implemented:

✨ **Version 1** → Displays *"Version 1"*  
✨ **Version 2** → Displays *"Version 2 - Updated"* (in green with new feature)

---

## 🐳 Docker Images

### 🔹 Build Version 1

```bash
docker build -t k8s-app:v1 app/v1/


🔹 Build Version 2
docker build -t k8s-app:v2 app/v2/

☸️ Kubernetes Deployment
▶️ Start Cluster
minikube start

📦 Apply Deployment & Service
kubectl apply -f k8s/
🔍 Check Running Pods
kubectl get pods
🌐 Service Exposure

Expose the application using NodePort:
minikube service app-service

🔄 Rolling Update
🚀 Update to Version 2
kubectl set image deployment/app-deployment app=k8s-app:v2
👀 Monitor Update Progress
kubectl get pods -w
✅ Features Demonstrated

✔️ Docker image versioning
✔️ Kubernetes Deployment management
✔️ Zero-downtime rolling updates
✔️ Health probes (liveness, readiness, startup)
✔️ Service exposure via NodePort

👨‍💻 Author

Yaswanth
