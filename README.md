Project - CI/CD Pipeline Setup
Overview
This project demonstrates a complete CI/CD pipeline for a Node.js application using Docker, GitHub Actions, and Minikube. The pipeline automates building a Docker image, running tests, pushing the image to Docker Hub, and deploying the application locally on Minikube.

Technologies Used
Node.js (Express framework)

Docker (Containerization)

GitHub Actions (CI/CD workflows)

Docker Hub (Image repository)

Minikube (Local Kubernetes cluster)

Project Structure
Dockerfile - Defines the Docker image build process.

docker-compose.yml - (If applicable) Manages multi-container setup.

.github/workflows/ci-cd.yml - GitHub Actions workflow for CI/CD.

index.js - Main Node.js application file.

CI/CD Pipeline
The GitHub Actions workflow automates the following steps on every push:

Run Tests: Executes unit tests (if any).

Build Docker Image: Builds the Docker image of the app.

Push Image: Pushes the image to Docker Hub under lucky5683/project1:latest.

Deploy Locally: Pulls and runs the Docker image on a local Minikube Kubernetes cluster.

How to Run Locally
Prerequisites
Docker installed and running

Minikube installed and started

Kubernetes CLI (kubectl) configured

Steps
Start Minikube:

bash
Copy
Edit
minikube start
Deploy the app to Minikube:

bash
Copy
Edit
kubectl apply -f deployment.yaml
Expose the service and get the URL:

bash
Copy
Edit
minikube service project1-deployment --url
Open the URL in your browser to access the running app.

Deliverables
Docker Image:
Available at Docker Hub repository

GitHub Actions Workflow:
Located in .github/workflows/ci-cd.yml in the GitHub repo

Minikube Deployment:
App running on Minikube accessible via provided service URL

Docker Hub Image Page:

Conclusion
This project showcases a full CI/CD cycle integrating containerization and Kubernetes deployment for efficient development and delivery. The automation ensures rapid feedback and consistent deployment environments.
