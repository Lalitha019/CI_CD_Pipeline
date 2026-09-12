<img width="1321" height="659" alt="image" src="https://github.com/user-attachments/assets/b975bd1d-65ed-4a1f-b0c2-dc2eb8b76acb" />

# CI/CD Pipeline with Jenkins, Docker, Kubernetes & Argo CD

An end-to-end CI/CD and GitOps implementation demonstrating automated
application build, testing, static code analysis, containerization,
Kubernetes deployment, and continuous delivery using Argo CD.

## 🚀 Technology Stack

- AWS EC2
- Jenkins
- Maven
- SonarQube
- Docker
- Docker Hub
- GitHub
- Kubernetes
- Argo CD
- GitOps

## 🔄 Pipeline Flow

```text
GitHub
   ↓
Jenkins
   ↓
Checkout Source Code
   ↓
Maven Build & Test
   ↓
SonarQube Static Code Analysis
   ↓
Docker Image Build
   ↓
Push Image to Docker Registry
   ↓
Update Kubernetes Deployment Manifest
   ↓
GitHub Commit
   ↓
Argo CD
   ↓
Kubernetes
   ↓
Deployed Application

## ✅ Outcome

Successfully implemented an automated CI/CD pipeline that builds,
tests, analyzes, containerizes, and deploys a Maven-based application
to Kubernetes using Argo CD and GitOps practices.
