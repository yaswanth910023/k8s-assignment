# 🚀 Kubernetes Deployment Assignment

## 📌 Overview
This project demonstrates deployment of a frontend application using Docker and Kubernetes with rolling updates.

---

## 🌐 Application
Two versions of the application:

- Version 1 → Displays "Version 1"
- Version 2 → Displays "Version 2 - Updated"

---

## 🐳 Docker

docker build -t k8s-app:v1 app/v1/
docker build -t k8s-app:v2 app/v2/

---

## ☸️ Kubernetes

kubectl apply -f k8s/

kubectl get pods
kubectl get svc

---

## 🌐 Access Application

minikube service app-service

---

## 🔄 Rolling Update

kubectl set image deployment/app-deployment app=k8s-app:v2

---

## 📁 Structure

k8s-assignment/
├── app/
├── k8s/
├── docs/
└── README.md

---

## 👨‍💻 Author

Yaswanth
