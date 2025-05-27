# Project1 - CI/CD Pipeline with Docker and Kubernetes

## Overview

This project demonstrates a complete CI/CD pipeline that builds, tests, and deploys a Node.js application using:

- **Docker** for containerization  
- **GitHub Actions** for CI/CD automation  
- **Kubernetes (Minikube)** for deployment  

---

## Features

- Automated Docker image build and push to Docker Hub  
- Automated testing in GitHub Actions workflow  
- Kubernetes deployment and service manifests included  
- Easy to deploy on local Kubernetes cluster (Minikube) or any K8s cluster  

---

## Prerequisites

- Docker installed and running  
- Minikube installed and running (for local Kubernetes cluster)  
- kubectl CLI installed  
- GitHub account with secrets configured for Docker Hub credentials (`DOCKER_USERNAME` and `DOCKER_PASSWORD`)  

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/<your-username>/project1.git
cd project1
