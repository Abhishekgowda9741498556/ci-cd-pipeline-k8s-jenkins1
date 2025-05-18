# ci-cd-pipeline-k8s-jenkins1
CI/CD pipeline to deploy Java app on Kubernetes using Jenkins, Docker, and Helm



# README.md
# CI/CD Pipeline with Jenkins & Kubernetes

## Tools Used
- Jenkins
- Docker
- Kubernetes
- Helm
- Maven
- GitHub

## Description
This project demonstrates a complete CI/CD pipeline setup for deploying a Java application into a Kubernetes cluster using Jenkins.

## Stages in Pipeline
1. Clone repo
2. Build with Maven
3. Dockerize
4. Push image to Docker Hub
5. Deploy to K8s using Helm

## How to Run
```bash
# Make sure Docker, Kubernetes, and Jenkins are configured
kubectl create namespace java-app
helm upgrade --install java-app ./k8s/helm-chart --namespace java-app
```
