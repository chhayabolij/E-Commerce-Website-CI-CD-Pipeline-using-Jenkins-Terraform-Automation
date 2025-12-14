# 🛒 E-Commerce Website CI/CD Pipeline using Jenkins & Terraform

## 🌟 Project Highlights

* Fully automated **CI/CD pipeline** using Jenkins
* **Infrastructure as Code (IaC)** with Terraform
* **AWS Cloud Deployment** (EC2 + RDS)
* Secure, scalable, and maintainable architecture
* Modern tech stack: **Spring Boot, MySQL, AWS, Jenkins, Terraform, Maven**

---

## 🏗 Architecture Diagram

![](./img/CI_CD%20pipeline%20flowchart%20for%20e-commerce.png)


### 🔄 Architecture Flow

1. Code pushed to **GitHub** triggers Jenkins via **Webhook**.
2. Jenkins builds and tests the **Spring Boot** application using **Maven**.
3. **Terraform** provisions AWS infrastructure (VPC, EC2, RDS, IAM, Security Groups).
4. Jenkins deploys the application artifact to **EC2**.
5. The application connects securely to **MySQL RDS** for persistent data storage.



---

## 💻 Tech Stack

| Layer                | Technology               |
| -------------------- | ------------------------ |
| Backend              | Java Spring Boot         |
| Database             | MySQL (AWS RDS)          |
| Cloud Infrastructure | AWS EC2, AWS RDS         |
| CI/CD                | Jenkins, GitHub Webhooks |
| IaC                  | Terraform                |
| Build Tool           | Maven                    |
| Version Control      | Git & GitHub             |
| OS                   | Ubuntu / Linux           |

---

## ⚡ Features

* End-to-end automated CI/CD pipeline
* Terraform-managed AWS infrastructure
* Spring Boot application hosted on EC2
* Secure RDS database with Security Group rules
* GitHub Webhook-based automated deployments
* Production-ready and scalable setup

---

## 🖼 Screenshots

  ![](./img/mansi%20kadam.png)

* **Jenkins Pipeline Execution**
![](./img/jenkins%20pipeline.jpg)

* **Terraform Infrastructure Deployment**
![](./img/mansi%20kadam%202.png)

---

## 🚀 Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/chhayabolij/E-Commerce-Website-CI-CD-Pipeline-using-Jenkins-Terraform-Automation.git
 cd ecommerce-terraform-jenkins
```

### 2️⃣ Provision Infrastructure with Terraform

```bash
cd terraform
terraform init
terraform plan
terraform apply
```

**This provisions:**

* EC2 instance
* MySQL RDS
* IAM roles
* VPC & Security Groups

### 3️⃣ Jenkins CI/CD Configuration

* Install Jenkins plugins: **Git, Maven, Pipeline, SSH Agent**
* Create a **Pipeline Job** using the provided `Jenkinsfile`
* Configure **GitHub Webhook** for automatic triggers

### 4️⃣ Application Deployment

* Jenkins builds the JAR using Maven
* Artifact is copied and deployed to EC2
* Access the application via **EC2 Public IP**

---

## 🔄 CI/CD Workflow

1. Code Commit → GitHub
2. GitHub Webhook → Jenkins
3. Jenkins → Build, Test & Package
4. Terraform → Infrastructure Provisioning
5. Jenkins → Application Deployment
6. Application Live & Connected to RDS

---

## 📌 Notes & Best Practices

* Update `terraform/variables.tf` with AWS details and DB credentials
* Allow inbound **HTTP (80)** and **SSH (22)** in EC2 Security Group
* Allow EC2 access to RDS on **port 3306**
* Store secrets securely using **Jenkins Credentials Plugin**
* Never hardcode passwords or keys in code

---

## 📈 Project Status

✅ **Completed & Fully Functional**

* Automated Terraform provisioning
* Jenkins CI/CD fully integrated
* Application deployed and tested on AWS

---


