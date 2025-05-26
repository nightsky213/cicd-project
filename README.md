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
* **Notifications**: Real-time alerts via **Slack**.

---

## 🔧 Tools & Technologies

* **CI/CD**: GitHub Actions
* **Build**: Maven
* **Code Quality**: SonarQube
* **Security**: Trivy, Gitleaks
* **Containerization**: Docker
* **Orchestration**: Kubernetes (EKS)
* **Monitoring**: Prometheus, Grafana
* **Notifications**: Slack

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
        | Slack Notifications   |
        +-----------------------+
```

---

## 📸 Screenshots by Phase

### Phase 1: Infrastructure Setup

* Includes images of Terraform provisioning and AWS EKS setup.

### Phase 2: Code Compilation

* Screenshots of Maven build process for a Java app.

### Phase 3: Security Scan

* Shows Gitleaks and Trivy scanning results.

### Phase 4: Unit Testing

* Test execution outputs validating the application.

### Phase 5: SonarQube Analysis

* Screenshots from SonarQube dashboard.

### Phase 6: Dockerization

* Docker image creation and push to Docker Hub.

### Phase 7: Kubernetes Deployment

* Deployed app UI, includes boardgame list screenshot.

### Phase 8: Slack Notifications

* Slack message for deployment success.

---

## 🛠️ Prerequisites

* **AWS Account**
* **Docker Hub Account**
* **SonarQube Account**
* **Slack Workspace**
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
     * `SLACK_WEBHOOK`

3. **Update Config Files**

   * Edit `deployment.yml`, `.github/workflows/ci-cd.yml` etc.

4. **Trigger the Pipeline**

   * Push to `main` branch.

---

## 📚 Blog Summary

See `BLOG.md` for detailed phase-wise description.

---

## 📋 Additional Resources

* [The Ultimate CICD Corporate DevOps Pipeline](https://medium.com)

---

