Project Overview

This project aims to design, build, and deploy a cloud-native web application using Kubernetes and Helm for container orchestration and packaging, while implementing a full CI/CD pipeline for automated testing, building, and deployment on AWS. The project demonstrates end-to-end DevOps practices for scalable, resilient, and automated application delivery.

Objectives

Deploy a containerized web application on AWS EKS (Elastic Kubernetes Service).

Use Helm charts to manage application deployments and configurations.

Implement a CI/CD pipeline with GitHub Actions (or GitLab CI/Jenkins) to automate:

Linting & testing.

Docker image builds & pushes to Amazon ECR.

Helm-based deployments to EKS.

Ensure secure, scalable, and observable infrastructure with best DevOps practices.

Architecture

Application Layer

A simple Flask/Node.js web app with REST endpoints.

Containerized using Docker.

Stores data in a managed AWS RDS (PostgreSQL/MySQL) or lightweight SQLite for demo purposes.

Infrastructure Layer

AWS EKS cluster provisioned with Terraform or eksctl.

Helm charts used for:

Web application deployment.

Ingress (NGINX or AWS ALB ingress controller).

Monitoring (Prometheus + Grafana optional).

CI/CD Layer

GitHub Actions pipeline to:

Run tests on pull requests.

Build Docker images and push to ECR.

Deploy via Helm to EKS.

Workflow

Developer pushes code → GitHub triggers CI.

CI runs tests & builds a Docker image → pushed to ECR.

CD step applies Helm chart to deploy the new version to EKS.

Application is exposed via an Ingress → accessible on AWS public endpoint.

Tools & Technologies

AWS: EKS, ECR, RDS, IAM.

Kubernetes: Workloads, Ingress, Services.

Helm: Application packaging & deployment.

CI/CD: GitHub Actions (or alternative).

Docker: Containerization.

Terraform/eksctl: Infrastructure provisioning (optional but recommended).

Stretch Goals (Optional Enhancements)

Add monitoring & logging stack (Prometheus + Grafana + Loki).

Implement blue/green or canary deployments using Helm hooks or Argo Rollouts.

Add AWS S3 integration for file storage.

Add Secrets management with AWS Secrets Manager or Sealed Secrets.

Expected Outcome

By the end of the project, we will have:

A fully automated pipeline that delivers code changes from GitHub to a running Kubernetes app on AWS.

Helm-based configuration for reproducible deployments.

A documented, production-like setup showcasing DevOps principles in real-world environments.
