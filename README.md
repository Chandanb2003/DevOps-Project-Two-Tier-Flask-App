# 🚀 DevOps Project: CI/CD Pipeline for a 2-Tier Flask Application on GCP  

![Jenkins](https://img.shields.io/badge/CI%2FCD-Jenkins-blue?logo=jenkins)
![Docker](https://img.shields.io/badge/Containerized-Docker-blue?logo=docker)
![GCP](https://img.shields.io/badge/Deployed%20on-Google%20Cloud-yellow?logo=googlecloud)
![Flask](https://img.shields.io/badge/Backend-Flask-black?logo=flask)
![MySQL](https://img.shields.io/badge/Database-MySQL-orange?logo=mysql)
![Status](https://img.shields.io/badge/Status-Deployed-success?style=flat-square)

**Author (Original Project):** [Prashant Gohel](https://github.com/prashantgohel-dev)  
**Deployed & Automated by:** **Chandan B**  
**Date:** November 2025  

---

## 📘 Project Overview  

This project demonstrates the **deployment and automation** of a 2-tier web application (**Flask + MySQL**) using **Docker**, **Jenkins**, and **GitHub** on a **Google Cloud Platform (GCP)** Virtual Machine.  

The CI/CD pipeline automatically **builds, tests, and deploys** the updated application whenever new code is pushed to the GitHub repository — showcasing a full DevOps workflow from **source control to deployment**.  

---

## 🏗️ Architecture  

Here’s a quick overview of how everything connects:  

**Developer → GitHub → Jenkins → Docker → GCP VM**

1. Developer pushes code to **GitHub**  
2. **Jenkins** automatically pulls the latest code and builds Docker images  
3. The application and database containers are deployed via **Docker Compose** on the **GCP VM**  

This setup forms a clean **2-tier architecture** — Flask as the application layer and MySQL as the database layer.  

---

## ⚙️ Tech Stack  

- **Flask (Python)** – Web application  
- **MySQL** – Database layer  
- **Docker** – Containerization  
- **Docker Compose** – Multi-container orchestration  
- **Jenkins** – CI/CD automation  
- **GitHub** – Source code management  
- **GCP VM Instance** – Cloud infrastructure  

---

## 🧱 Project Workflow  

1. Developer pushes code to **GitHub**  
2. **Jenkins** automatically triggers the build pipeline  
3. Jenkins clones the repo, builds the Docker image, and deploys via **Docker Compose**  
4. Application runs on **Flask (port 5000)** with a connected **MySQL** container  
5. Every new push automatically triggers a rebuild and redeployment  

---

## 🧩 Files Included  

### 🐍 **Dockerfile**  
Defines the Flask app container environment  

### ⚙️ **docker-compose.yml**  
Orchestrates multi-container setup (Flask + MySQL)  

### 🧾 **Jenkinsfile**  
Contains pipeline-as-code configuration for Jenkins automation  

---

## 🚀 Deployment Details  

- **Hosted on:** Google Cloud Platform (GCP)  
- **App URL:** 🌐 [http://34.93.214.230:5000](http://34.93.214.230:5000)  
- **Database:** Persistent volume for MySQL data  
- **Pipeline:** Automatically redeploys on every push to `main` branch  

---

## 🙏 Credits  

A special thanks to **[Prashant Gohel](https://github.com/prashantgohel-dev)** for his original project and detailed documentation — his AWS-based setup inspired me to replicate and deploy it on **Google Cloud** with my own CI/CD pipeline!  

---

## 📎 Repository  

🔗 **GitHub Repo:** [https://github.com/Chandanb2003/DevOps-Project-Two-Tier-Flask-App](https://github.com/Chandanb2003/DevOps-Project-Two-Tier-Flask-App)  

---

## 🧠 Learnings  

- Setting up **Jenkins CI/CD** for automated Docker builds and deployments  
- Managing **multi-container apps** using Docker Compose  
- Understanding **infrastructure automation** on cloud instances  
- Integrating **GitHub + Jenkins + Docker + GCP** for a complete DevOps workflow  
