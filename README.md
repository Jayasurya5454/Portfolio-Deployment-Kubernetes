# Portfolio Deployment on Kubernetes
<div align="left">
   <img src="https://techstack-generator.vercel.app/kubernetes-icon.svg" alt="icon" width="50" height="50" />
   <img src="https://techstack-generator.vercel.app/docker-icon.svg" alt="icon" width="50" height="50" />
   
  
</div>


## Overview

Welcome to the **Portfolio Deployment on Kubernetes** project! This repository contains a comprehensive setup for deploying a personal portfolio application using **Kubernetes** and **Docker**. It demonstrates best practices in containerization and orchestration, ensuring scalability and maintainability.

##  Features

- **Dockerized Application**: Easily deploy your portfolio using Docker containers.
- **Kubernetes Orchestration**: Leverage Kubernetes for automated deployment, scaling, and management of your application.
- **Simple Configuration**: Use YAML files for easy setup and configuration management.


###  Prerequisites

Before you begin, ensure you have the following installed:

- [Docker](https://www.docker.com/get-started)
- [Kubernetes](https://kubernetes.io/docs/setup/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/) (for local Kubernetes clusters)

## Deployment

To deploy your portfolio on Kubernetes, follow these steps:

1. Apply the deployment configuration:
   ```bash
   kubectl apply -f Portfolio-Deployment.yaml
   ```
2. Apply the service configuration:
   ```bash
   kubectl apply -f Portfolio-service.yaml
   ```
3. Verify the deployment:
   ```bash
   kubectl get pods
   ```
4. Verify the services:
   ```bash
   kubectl get services
   ```
5.Use the command to forward a service's port to your local machine for easy access:
    ```bash
    kubectl port-forward service/Portfolio-service 8080:80
    ```

6. Run the command to open the deployed service in your default browser:
   ```bash
   minikube service Portfolio-service
   ```

 

