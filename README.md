# Final Project — DevOps

**Title:** PTR — Project to Rescue (Login System)

## Overview

The project is a full-stack login system demonstrating DevOps practices. It includes a Node.js frontend, a Python Flask backend, and a PostgreSQL database. All components are containerized and deployed locally with Docker Compose, and to Kubernetes using Helm charts.

## Objectives

* Build a login/signup system with session management.
* Store user and group data in PostgreSQL.
* Containerize frontend, backend, and database.
* Deploy locally with Docker Compose.
* Deploy on Kubernetes with Helm charts.
* Automate builds, tests, and deployments with GitLab CI/CD.

## Tech stack

* Frontend: Node.js
* Backend: Flask (Python)
* Database: PostgreSQL
* Containerization: Docker
* Orchestration: Docker Compose + Kubernetes (Helm)
* CI/CD: GitLab CI/CD

## Plan

1. **Frontend (Node.js):** Login/signup UI, calls backend API.
2. **Backend (Flask):** Handles authentication, sessions, connects to DB.
3. **Database (PostgreSQL):** Stores users, groups, sessions.
4. **Docker Compose:** Local setup of all services.
5. **Helm Charts:** Kubernetes deployment with dev/prod values.
6. **GitLab CI/CD:** Build, test, push images, deploy via Helm.

## Deliverables

* Source code (frontend, backend, DB schema).
* Dockerfiles, `docker-compose.yml`, and Helm charts.
* GitLab CI/CD pipelines.
* Documentation and short demo showing login, signup, sessions, and deployment.

---

*End of project summary.*
