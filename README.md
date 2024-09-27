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
- **Multi-Environment Support**: Seamlessly switch between development and production environments.
- **Load Balancing**: Distribute incoming traffic effectively with Kubernetes Services.
- **Simple Configuration**: Use YAML files for easy setup and configuration management.

##  Table of Contents

1. [Getting Started](#getting-started)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Deployment](#deployment)
5. [Usage](#usage)
6. [Contributing](#contributing)
7. [License](#license)

##  Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

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
5. Get the URL to see the output of the deployment as a service:
   ```bash
   minikube service Portfolio-service --url
   ```

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

