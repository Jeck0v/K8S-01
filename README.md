
# <p align="center"> FastAPI Kubernetes Project</p>

## Project Overview
This project demonstrates how to deploy a FastAPI application to a local Kubernetes cluster using Docker.

Prerequisites:
- Docker
- Kubernetes (Minikube)
- FastAPI

<hr>
Set up your docker image, then we can get started:

Starting:
```bash
minikube start
```
Apply the deployment:
```bash
 kubectl apply -f deployment.yaml
```
Apply the service:
```bash
 kubectl apply -f service.yaml
```
Access the service:
```bash
 kubectl port-forward svc/fff-service 8000:80
```
Now you can test it : 
http://localhost:8000/docs
