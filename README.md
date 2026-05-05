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
