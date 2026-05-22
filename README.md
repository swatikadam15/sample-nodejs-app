# Node.js CI/CD Pipeline Deployment using Jenkins, Docker & Kubernetes

## 📌 Project Overview

This project demonstrates a complete CI/CD pipeline for deploying a Node.js application using:

- Jenkins
- Docker
- Docker Hub
- Kubernetes (K8s)
- AWS EC2

The pipeline automatically:

1. Pulls code from GitHub
2. Builds Docker image
3. Pushes image to Docker Hub
4. Deploys application on Kubernetes cluster

---

## 🛠️ Technologies Used

- Node.js
- Jenkins
- Docker
- Docker Hub
- Kubernetes
- AWS EC2
- Git & GitHub

---

## 🏗️ Architecture

GitHub → Jenkins → Docker Build → Docker Hub → Kubernetes Deployment

---

## 📂 Project Structure

```bash
sample-nodejs-app/
│── Dockerfile
│── Jenkinsfile
│── package.json
│── package-lock.json
│── server.js
│── deployment.yaml
│── service.yaml
└── README.md
```

---

## 🚀 Jenkins Pipeline Stages

### 1. Checkout Code
Jenkins pulls source code from GitHub repository.

### 2. Build Docker Image
Docker image is created using Dockerfile.

```bash
docker build -t image-name .
```

### 3. Push Image to Docker Hub

```bash
docker push username/image-name
```

### 4. Deploy to Kubernetes

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

---

## 🐳 Docker Setup

Build Docker image manually:

```bash
docker build -t sample-nodejs-app .
```

Run container:

```bash
docker run -d -p 3000:3000 sample-nodejs-app
```

---

## ☸️ Kubernetes Setup

Deploy application:

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

Check pods:

```bash
kubectl get pods
```

Check services:

```bash
kubectl get svc
```

---

## 🔧 Jenkins Configuration

- Installed Jenkins on EC2
- Added Docker Hub credentials
- Configured SSH for deployment server
- Created Multibranch Pipeline Job

---

## 📸 Screenshots

Add screenshots here:

- Jenkins Pipeline Success

- Option 1: EC2 server
docker run -d -p 80:3000 repo/sample-app:latest
<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/404f8abe-7eb5-48f3-8877-b93be7324475" />


- 
- Docker Hub Image
- Kubernetes Pods
- Running Application

---

## 👩‍💻 Author

Swati Kadam
