# CI/CD Project: DevOps Shack Ultimate Pipeline

> **Author:** Vibhava N
> **Project Name:** ci-cd project

---

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

## 🦖 Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/nightsky213/cicd-project.git
```

2. **Configure Secrets**

   * GitHub secrets required:

     * `AWS_ACCESS_KEY_ID`
     * `AWS_SECRET_ACCESS_KEY`
     * `DOCKER_USERNAME`
     * `DOCKER_PASSWORD`
     * `SONAR_TOKEN`
    

3. **Update Config Files**

   * Edit `deployment.yml`, `.github/workflows/ci-cd.yml` etc.

4. **Trigger the Pipeline**

   * Push to `main` branch.


