# 🚀 AWS 3-Tier Java DevOps Application

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazonaws)
![Terraform](https://img.shields.io/badge/Terraform-IaC-623CE4?logo=terraform)
![Docker](https://img.shields.io/badge/Docker-Container-blue?logo=docker)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI-blue?logo=githubactions)
![Java](https://img.shields.io/badge/Java-11-red?logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-2.7-green?logo=springboot)
![Maven](https://img.shields.io/badge/Maven-Build-red?logo=apachemaven)
![License](https://img.shields.io/badge/License-MIT-green)

A production-style **AWS 3-Tier Java Application** demonstrating Infrastructure as Code (Terraform), Docker containerization, GitHub Actions CI, and scalable AWS infrastructure.

---

# 📌 Project Overview

This project demonstrates how a Java Spring Boot web application can be deployed using a highly available AWS 3-tier architecture.

The infrastructure is provisioned using **Terraform**, the application is **containerized using Docker**, and continuous integration is implemented using **GitHub Actions**.

---

# 🏗 Architecture

```text
                    Internet
                        │
                        ▼
          Application Load Balancer (ALB)
                        │
                        ▼
          Auto Scaling Group (EC2 Instances)
                        │
                        ▼
          Spring Boot Login Application
                        │
                        ▼
                Amazon RDS (MySQL)

──────────────────────────────────────────────

Infrastructure Provisioning → Terraform

Application Containerization → Docker

Continuous Integration → GitHub Actions
```

---

# ⚙ Tech Stack

## Cloud

- AWS EC2
- Amazon VPC
- Application Load Balancer
- Auto Scaling Group
- Amazon RDS (MySQL)
- CloudWatch
- IAM

## DevOps

- Terraform
- Docker
- GitHub Actions
- Git
- GitHub

## Backend

- Java 11
- Spring Boot
- Maven

## Database

- MySQL

---

# ✨ Features

- Infrastructure as Code using Terraform
- Multi-tier AWS Architecture
- Auto Scaling
- Application Load Balancer
- Dockerized Spring Boot Application
- GitHub Actions CI Pipeline
- CloudWatch Monitoring
- Modular Terraform Configuration
- Highly Available Infrastructure

---

# 📂 Project Structure

```
aws-3tier-java-devops
│
├── .github
│   └── workflows
│       └── ci.yml
│
├── infrastructure
│   ├── modules
│   │
│   ├── alb
│   ├── asg
│   ├── monitoring
│   ├── rds
│   ├── security
│   └── vpc
│
├── Java-Login-App
│   ├── src
│   ├── Dockerfile
│   ├── pom.xml
│   └── target
│
└── README.md
```

---

# ☁ AWS Infrastructure

The project provisions:

- Virtual Private Cloud (VPC)
- Public Subnets
- Private Subnets
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Application Load Balancer
- Auto Scaling Group
- Launch Template
- Amazon RDS MySQL
- CloudWatch Log Groups
- CloudWatch Alarms
- VPC Flow Logs

---

# 🐳 Docker

## Build

```bash
docker build -t java-login-app .
```

## Run

```bash
docker run -d -p 8080:8080 --name java-app java-login-app
```

## Verify

```bash
docker ps
```

Open:

```
http://localhost:8080
```

---

# 🔄 GitHub Actions CI

The workflow automatically:

- Checks out the repository
- Sets up Java
- Builds the project using Maven
- Validates every push to the `main` branch

Workflow file:

```
.github/workflows/ci.yml
```

---

# 🛠 Local Setup

Clone the repository

```bash
git clone https://github.com/Annie6105/aws-3tier-java-devops.git
```

Navigate

```bash
cd aws-3tier-java-devops
```

Build

```bash
cd Java-Login-App
mvn clean package
```

Run

```bash
mvn spring-boot:run
```

---

# 🚀 Terraform Deployment

```bash
cd infrastructure

terraform init

terraform plan

terraform apply
```

---

# 📸 Application

After successful deployment:

```
http://localhost:8080
```

The application provides a secure Spring Boot login interface backed by MySQL.

---

# 📈 CI Pipeline

```
Developer
      │
      ▼
 Git Push
      │
      ▼
 GitHub Actions
      │
      ▼
 Maven Build
      │
      ▼
 Build Success
```

---

# 📋 Key Learning Outcomes

- Infrastructure as Code (Terraform)
- AWS Networking
- EC2 Deployment
- Docker Containerization
- CI using GitHub Actions
- Maven Build Automation
- Cloud Monitoring
- Auto Scaling
- Load Balancing

---

# 🔮 Future Enhancements

- Kubernetes Deployment
- Amazon EKS
- ArgoCD
- SonarQube
- Trivy Image Scanning
- Prometheus
- Grafana
- AWS Secrets Manager

---

# 💼 Skills Demonstrated

- AWS
- Terraform
- Docker
- GitHub Actions
- Spring Boot
- Java
- Maven
- MySQL
- Infrastructure Automation
- CI/CD
- Cloud Computing

---

# 📄 License

This project is licensed under the MIT License.

---

# 👩‍💻 Maintainer

**Annie Rubha V**

GitHub: https://github.com/Annie6105