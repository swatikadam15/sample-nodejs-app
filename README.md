🚀 CI/CD Pipeline Deployment using Jenkins, Docker & Kubernetes on AWS EC2
📌 Project Overview

This project demonstrates a complete CI/CD pipeline for deploying a static website using:

Jenkins for automation
Docker for containerization
Kubernetes for orchestration
AWS EC2 instances for infrastructure

The application is automatically built and deployed whenever code changes are pushed to GitHub.

🏗️ Architecture
Infrastructure Setup

Three AWS EC2 instances were created:

Server	Purpose
Jenkins Server	CI/CD Pipeline & Docker Deployment
Kubernetes Master Node	Cluster Management
Kubernetes Worker Node	Application Deployment
⚙️ Technologies Used
AWS EC2
Jenkins
Docker
Kubernetes (K8s)
GitHub
Linux (Ubuntu/Amazon Linux)
Docker Hub
🔄 CI/CD Workflow
Developer pushes code to GitHub repository
Jenkins pipeline gets triggered
Jenkins pulls latest source code
Docker image is built
Docker image is pushed to Docker Hub
Kubernetes deployment is updated
Application gets deployed on Worker Node
