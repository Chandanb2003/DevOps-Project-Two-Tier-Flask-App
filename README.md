🚀 DevOps Project: CI/CD Pipeline for a 2-Tier Flask Application on GCP

Author (Original Project): Prashant Gohel

Deployed & Automated by: Chandan B
Date: November 2025

📘 Project Overview

This project demonstrates the deployment and automation of a 2-tier web application (Flask + MySQL) using Docker, Jenkins, and GitHub on a Google Cloud Platform (GCP) Virtual Machine.

The CI/CD pipeline automatically builds, tests, and deploys the updated application whenever new code is pushed to the GitHub repository — showcasing a full DevOps workflow from source control to deployment.
+-----------------+      +----------------------+      +-----------------------------+
|   Developer     |----->|     GitHub Repo      |----->|        Jenkins Server       |
| (pushes code)   |      | (Source Code Mgmt)   |      | (on GCP VM)                 |
+-----------------+      +----------------------+      |                             |
                                                       | 1. Clones Repo              |
                                                       | 2. Builds Docker Image      |
                                                       | 3. Runs Docker Compose      |
                                                       +--------------+--------------+
                                                                      |
                                                                      | Deploys
                                                                      v
                                                       +-----------------------------+
                                                       |      Application Server     |
                                                       |       (Same GCP VM)         |
                                                       |                             |
                                                       | +-------------------------+ |
                                                       | | Docker Container: Flask | |
                                                       | +-------------------------+ |
                                                       |              |              |
                                                       |              v              |
                                                       | +-------------------------+ |
                                                       | | Docker Container: MySQL | |
                                                       | +-------------------------+ |
                                                       +-----------------------------+
⚙️ Tech Stack

Flask (Python) – Web application

MySQL – Database layer

Docker – Containerization

Docker Compose – Multi-container orchestration

Jenkins – CI/CD automation

GitHub – Source code management

GCP VM Instance – Cloud infrastructure

🧱 Project Workflow

Developer pushes code to GitHub.

Jenkins automatically triggers the build pipeline.

Jenkins clones the repo, builds the Docker image, and deploys via Docker Compose.

Application runs on Flask (port 5000) with a connected MySQL container.

New pushes automatically trigger a rebuild and redeployment.

🧩 Files Included
Dockerfile

Defines the Flask app container environment.

docker-compose.yml

Orchestrates multi-container setup (Flask + MySQL).

Jenkinsfile

Contains pipeline-as-code configuration for Jenkins automation.

🚀 Deployment Details

Hosted on Google Cloud Platform (GCP)

Accessible at: 🌐 http://34.93.214.230:5000

Uses persistent volumes for MySQL data

Automatically redeploys with every new commit to main branch

🙏 Credits

A special thanks to Prashant Gohel
 for his original project and documentation — his AWS-based approach inspired me to replicate and deploy it on Google Cloud with my own CI/CD workflow!

📎 Repository

🔗 GitHub Repo: https://github.com/Chandanb2003/DevOps-Project-Two-Tier-Flask-App

🧠 Learnings

Setting up Jenkins CI/CD for automated Docker builds and deployments

Managing multi-container apps using Docker Compose

Understanding infrastructure automation on cloud instances

Integrating GitHub + Jenkins + Docker + GCP for an end-to-end DevOps workflow
