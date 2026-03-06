# 🚀 DevOps Mini Project — Containerized Web App Deployment

A personal DevOps project demonstrating containerization, cloud deployment, and CI/CD concepts using Docker, AWS EC2, and GitHub.

---

## 📌 Project Overview

This project involves building and deploying a containerized web application from scratch. The goal was to implement a real-world DevOps workflow — from writing a Dockerfile to deploying on cloud infrastructure.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Docker** | Containerizing the application |
| **AWS EC2** | Cloud server for deployment |
| **GitHub** | Version control & code management |
| **Linux (Ubuntu)** | Server OS on EC2 instance |
| **Shell Script** | Basic automation |

---

## 📐 Architecture

```
Developer Machine
      │
      ▼
   GitHub Repo  ──────────────────────────────┐
      │                                        │
      ▼                                        ▼
  Dockerfile                            AWS EC2 Instance
  (Build Image)                         (Ubuntu Linux)
      │                                        │
      ▼                                        ▼
 Docker Container  ──── Deployed to ────▶  Running App
```

---

## ⚙️ Steps Performed

### 1. Dockerize the Application
- Wrote a `Dockerfile` to containerize the web application
- Built Docker image locally
- Tested container locally before deployment

### 2. AWS EC2 Setup
- Launched an Ubuntu EC2 instance on AWS
- Configured Security Groups (HTTP port 80, SSH port 22)
- Connected to instance via SSH

### 3. Deploy on EC2
- Installed Docker on EC2 instance
- Pulled the Docker image
- Ran the container on the cloud server

### 4. Version Control with GitHub
- Maintained full commit history
- Managed code using branches and pushes

---

## 🚀 How to Run Locally

```bash
# Clone the repository
git clone https://github.com/rahullikhar/my-devops-project.git

# Navigate to project directory
cd my-devops-project

# Build Docker image
docker build -t devops-mini-project .

# Run the container
docker run -d -p 80:80 devops-mini-project

# Visit in browser
http://localhost
```

---

## ☁️ Deployment on AWS EC2

```bash
# SSH into EC2 instance
ssh -i your-key.pem ubuntu@your-ec2-public-ip

# Install Docker
sudo apt update && sudo apt install docker.io -y

# Run the container
sudo docker run -d -p 80:80 devops-mini-project
```

---

## 📚 What I Learned

- How containerization works with Docker
- Setting up and configuring AWS EC2 instances
- Linux server administration basics
- Git workflow — commits, branches, and pushes
- Connecting local development to cloud deployment

---

## 👤 Author

**Rahul Likhar**
- GitHub: [@rahullikhar](https://github.com/rahullikhar)
- Email: rahullikhar099@gmail.com
- Location: Pune, Maharashtra

---

> *This is a personal learning project built to demonstrate hands-on DevOps skills.*
