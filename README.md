# CI/CD Project: DevOps Shack Ultimate Pipeline

> **Project Name:** ci-cd project

---
## 📖 Project Blog

Read the full story behind this project on Medium: [Built end-to-end CI/CD pipeline](https://medium.com/@vibhavakrishna999/cicd-project-e91852f046ec)

## 🚀 About the Project

The **DevOps Shack Ultimate Pipeline** is a real-time, full-fledged CI/CD pipeline project that automates the entire software development lifecycle. From infrastructure provisioning to application deployment, this project showcases an integrated pipeline utilizing top-tier DevOps tools and practices.

Designed with scalability, security, and automation in mind, this pipeline is ideal for modern cloud-native applications and enterprise-grade workflows.

---

## 🧰 Key Features

* **Multi-Stage CI/CD Pipeline**: Automated steps from code to cloud.
* **Tool Integration**: Includes GitHub Actions, Maven, SonarQube, Docker, Kubernetes, Trivy, Gitleaks.
* **Security Focused**: Security scans using Trivy and Gitleaks.
* **Cloud Native Deployment**: Deploys to **AWS EKS**.


---

## 🔧 Tools & Technologies

* **CI/CD**: GitHub Actions
* **Build**: Maven
* **Code Quality**: SonarQube
* **Security**: Trivy, Gitleaks
* **Containerization**: Docker
* **Orchestration**: Kubernetes (EKS)
* **Monitoring**: Prometheus, Grafana
* **Notifications**: Gmail

---

## 📈 Pipeline Workflow Diagram

```
           +-----------------+
           |   Developer     |
           +--------+--------+
                    |
                    v
       +------------+------------+
       | Push to GitHub Repo     |
       +------------+------------+
                    |
                    v
       +------------+------------+
       | GitHub Actions CI/CD    |
       +------------+------------+
                    |
        +-----------+-----------+
        |  Compile using Maven  |
        +-----------+-----------+
                    |
        +-----------+-----------+
        |  Security Scan (Trivy)|
        |  Secret Scan (Gitleaks)|
        +-----------+-----------+
                    |
        +-----------+-----------+
        |     Unit Testing       |
        +-----------+-----------+
                    |
        +-----------+-----------+
        | SonarQube Code Quality|
        +-----------+-----------+
                    |
        +-----------+-----------+
        |  Docker Build & Push  |
        +-----------+-----------+
                    |
        +-----------+-----------+
        | Deploy to AWS EKS     |
        +-----------+-----------+
                    |
        +-----------+-----------+
        | Gmail Notifications   |
        +-----------------------+
```

---

## 📸 Screenshots by Phase

### Phase 1: Infrastructure Setup

* Includes images of Terraform provisioning and AWS EKS setup, Jenkins, Nexus, SonarQube.

### Phase 2: Github repo setup

* Screenshots of repo setup.

### Phase 3: CICD

* Includes setup steps and images of building cicd.

### Phase 4: Monitor

* Includes setup steps and images of implementing monitoring tools.


## 🛠️ Prerequisites

* **AWS Account**
* **Docker Hub Account**
* **SonarQube Account**
* **GitHub Repository**

---




