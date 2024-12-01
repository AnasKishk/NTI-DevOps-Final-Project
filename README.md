# NTI-DevOps-Final-Project

## Description
This project shows how to automate the deployment of a Django application on Amazon EKS (Elastic Kubernetes Service). It uses tools like Terraform for setting up infrastructure, Ansible for configuring servers, Docker for creating containers, Kubernetes for managing them, and Jenkins for automating the deployment process.

## Technologies Used
- **Terraform:** For creating and managing cloud infrastructure as code.
- **Ansible:** To install and configure Jenkins on EC2 servers.
- **Docker:** To package the Django app and its dependencies into containers.
- **Kubernetes:** To deploy, scale, and manage the containers.
- **Jenkins:** For automating the build, test, and deployment steps.

## Project Steps

1. **Infrastructure Provisioning with Terraform**
- Creating an Amazon EKS cluster with two node groups.
- Setting up Amazon ECR (Elastic Container Registry) to store Docker images.
- Configuring Amazon RDS (Relational Database Service) as the database for the Django app.
- Launching an EC2 server to host Jenkins.

2. **Jenkins Setup with Ansible**
- Using Ansible to install and configure Jenkins on the EC2 server.
- Installing all necessary tools for Jenkins.

3. **Dockerization of Django App**
- Writing a Dockerfile to package the Django app into a container.
- Building the Docker image and pushed it to Amazon ECR.

4. **Kubernetes Deployment**
- Writing Kubernetes YAML files to deploy the Django app.
- Setting up a Kubernetes service to route traffic to the app.

5. **Jenkins Pipeline Configuration**
- Creating a Jenkins pipeline to automate the build, test, and deployment process.
- Integrating Jenkins with Amazon ECR to build and store Docker images.
- Automating the app deployment to Amazon EKS using Kubernetes.

## Outcome
- Building a fully automated CI/CD pipeline to deploy the Django app quickly and efficiently.
- Making the app scalable and reliable using Kubernetes and Docker.
- Simplifying the deployment process with Terraform and Ansible as Infrastructure as Code (IaC) tools.
