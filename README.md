CI/CD Pipeline for Docker Image Deployment using Jenkins

Project Overview
This project demonstrates a simple CI/CD pipeline where Jenkins pulls source code from GitHub, builds a Docker image, and pushes the image to Docker Hub.

Tech Stack Used
AWS EC2 (Ubuntu)
Jenkins
Docker
GitHub
Docker Hub

Project Flow
1. Code is pushed to GitHub
2. Jenkins pulls the code from GitHub
3. Jenkins builds a Docker image using Dockerfile
4. Jenkins logs in to Docker Hub
5. Jenkins pushes the Docker image to Docker Hub

Repository Structure
.
├── Dockerfile
├── app.sh
└── Jenkinsfile

Dockerfile Explanation
The Dockerfile creates a Docker image using Alpine Linux, copies the app.sh file into the container, and executes it when the container starts.

Jenkins Pipeline Stages
Checkout - Clones GitHub repository
Build Docker Image - Builds Docker image
Docker Login - Logs in to Docker Hub
Push Image - Pushes image to Docker Hub

Docker Hub Image
<dockerhub_name>/<repo_name(simple-app:latest)>

Output
When the Docker container runs, it prints:
Hello from Docker built by Jenkins!

Purpose of This Demo
To understand Jenkins pipelines
To learn Docker image creation
To automate Docker image deployment
To gain hands-on CI/CD experience

Author
Lakshman Hari
