# Kubernetes Deployment Assignment

## 📌 Overview
This project demonstrates deployment of a frontend application using Kubernetes with rolling updates.

---

## 🌐 Application
- Version 1: Basic UI (Blue)
- Version 2: Updated UI (Green + new feature)

---

## 🐳 Docker Images
Built using nginx base image.

### Build Commands:
```bash
docker build -t k8s-app:v1 .
docker build -t k8s-app:v2 .
