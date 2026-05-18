# 🚀 CI/CD Pipeline Deployment using GitHub Actions & Docker on AWS

![Project Status](https://img.shields.io/badge/status-in--progress-yellow)
![Cloud](https://img.shields.io/badge/cloud-AWS-orange)
![DevOps](https://img.shields.io/badge/focus-DevOps-blue)

---

# 📌 Project Overview

This project demonstrates a DevOps CI/CD workflow using AWS EC2, Docker, GitHub, and GitHub Actions.

The goal is to automate application deployment using containerization and CI/CD practices.

---

# 🏗 Architecture Overview

```text
Developer
   ↓
GitHub Repository
   ↓
GitHub Actions
   ↓
Docker Container
   ↓
AWS EC2 Server
```

---

# 🚀 Day 1 — EC2 & Docker Setup

## 📌 Tasks Completed

- Launched EC2 instance on AWS
- Configured Security Groups
- Connected to server using SSH
- Installed Docker on Amazon Linux 2
- Verified Docker installation

---

# 🔧 Technologies Used

- AWS EC2
- Amazon Linux 2
- Docker
- Linux
- GitHub

---

# 🔐 Security Group Configuration

| Type | Port |
|---|---|
| SSH | 22 |
| HTTP | 80 |
| Custom TCP | 8080 |

---

# 🛠 Commands Used

```bash
sudo yum update -y
sudo amazon-linux-extras install docker -y
sudo systemctl start docker
sudo systemctl enable docker
docker --version
```

---

# 📸 Screenshots

## EC2 Instance Running

<img width="1920" height="797" alt="EC2 Running" src="https://github.com/user-attachments/assets/2913e867-e77c-49d6-bac0-db7d2d458eb8" />

---

## Docker Installed Successfully

<img width="1859" height="878" alt="Docker Installed" src="https://github.com/user-attachments/assets/9261ef83-273c-41f0-a5a0-0b7e225a3e65" />

---

## Security Group Rules

<img width="1920" height="762" alt="Security Group Rules" src="https://github.com/user-attachments/assets/d7d0428b-0981-4a02-8b37-91d031759781" />

---

# 📚 Key Learnings

- Docker installation on AWS EC2
- Linux server management
- Security Group configuration
- Basic containerization concepts

---

# 🚀 Next Step



---

# 🚀 Day 2 — Dockerized Web Application Deployment

## 📌 Tasks Completed

- Created a sample web application
- Built a Docker image using Dockerfile
- Ran the container on AWS EC2
- Configured port mapping for public access
- Verified live application deployment in browser

---

# 🛠 Files Created

## index.html

```html
<h1>Dockerized AWS DevOps Project 🚀</h1>
```

---

## Dockerfile

```dockerfile
FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html
```

---

# 🛠 Commands Used

## Build Docker Image

```bash
docker build -t myapp .
```

---

## Verify Docker Image

```bash
docker images
```

---

## Run Docker Container

```bash
docker run -d -p 8080:80 myapp
```

---

## Verify Running Container

```bash
docker ps
```

---

# 🌐 Application Access

```text
http://PUBLIC-IP:8080
```

---

# 📸 Screenshots

## Docker Image Created

<img width="1887" height="854" alt="docker-images" src="https://github.com/user-attachments/assets/cbf0b059-7728-4dc1-a72f-39b6ae90435a" />

---

## Running Docker Container

<img width="1887" height="854" alt="docker-images" src="https://github.com/user-attachments/assets/ee8cf653-3600-4e48-883a-b537dc177901" />

---

## Browser Output

<img width="1902" height="922" alt="docker-webapp-output" src="https://github.com/user-attachments/assets/b59daf4f-91bb-4ec9-8b44-0c9668084ec7" />

---


# 📚 Key Learnings

- Docker image creation
- Container deployment
- Port mapping concepts
- Running applications inside containers
- Public application access via EC2

---

# 🚀 Next Step

Day 3:
Push Dockerized Application to GitHub & Prepare CI/CD Workflow
