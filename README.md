# 🐳 Docker Learning Repository

A complete hands-on Docker learning repository covering containerization fundamentals, Docker commands, image creation, container management, networking, volumes, and real-world deployment basics for DevOps and Cloud learning.

---

# 🚀 About This Repository

This repository contains practical Docker learning exercises, commands, examples, and mini-projects designed to build strong containerization fundamentals for DevOps, Cloud, SRE, and backend engineering roles.

## 🎯 Objectives

- Learn Docker from scratch
- Understand containerization concepts
- Build and manage Docker containers
- Create custom Docker images
- Work with Docker networking and volumes
- Practice real-world DevOps workflows

---

# 📚 Topics Covered

- Docker Basics
- Docker Installation
- Docker Commands
- Docker Images
- Docker Containers
- Dockerfile
- Docker Volumes
- Docker Networking
- Port Mapping
- Environment Variables
- Docker Compose Basics
- Nginx with Docker
- Python App Containerization

---

# 🛠️ Tech Stack

- Docker
- Linux
- Ubuntu
- Nginx
- Python
- Git & GitHub

---

# 📂 Repository Structure

```bash
Docker/
│── basic-commands/
│── dockerfiles/
│── nginx-project/
│── python-app/
│── networking/
│── volumes/
└── README.md
```

---

# ⚡ Basic Docker Commands

## Check Docker Version

```bash
docker --version
```

## Pull Docker Image

```bash
docker pull nginx
```

## Run Nginx Container

```bash
docker run -d -p 8080:80 nginx
```

## View Running Containers

```bash
docker ps
```

## Stop Container

```bash
docker stop <container_id>
```

## Remove Container

```bash
docker rm <container_id>
```

## Remove Docker Image

```bash
docker rmi <image_id>
```

---

# 🐍 Dockerize Python Application

## Dockerfile

```Dockerfile
FROM python:3.11

WORKDIR /app

COPY . .

CMD ["python", "app.py"]
```

## Build Docker Image

```bash
docker build -t python-app .
```

## Run Python Container

```bash
docker run python-app
```

---

# 🌐 Nginx Container Setup

## Run Nginx

```bash
docker run -d -p 8080:80 nginx
```

## Open in Browser

```bash
http://localhost:8080
```

---

# 💾 Docker Volumes

## Create Volume

```bash
docker volume create myvolume
```

## Use Volume

```bash
docker run -v myvolume:/data nginx
```

---

# 🔗 Docker Networking

## Create Docker Network

```bash
docker network create mynetwork
```

## Run Container in Network

```bash
docker run --network=mynetwork nginx
```

---

# 🎯 Learning Outcomes

After completing this repository, you will understand:

✅ Docker fundamentals  
✅ Container lifecycle management  
✅ Docker image creation  
✅ Port mapping and networking  
✅ Docker volumes and storage  
✅ Running applications inside containers  
✅ Basic DevOps workflows  

---

# 📈 Future Enhancements

- Docker Compose
- Multi-container applications
- CI/CD pipeline integration
- Kubernetes basics
- AWS Docker deployment
- Monitoring containers

---

# 🤝 Connect With Me

## GitHub
https://github.com/Chandrashekhar-cloud

## LinkedIn
https://www.linkedin.com/in/chandrashekhar-68844b3a3?utm_source=share_via&utm_content=profile&utm_medium=member_android

---

# ⭐ Support

If you found this repository useful, give it a ⭐ on GitHub and follow for more DevOps, Cloud, Docker, and AI/ML projects.

---

# 👨‍💻 Author

**Chandrashekhar H S**  
Future DevOps | Cloud | SRE | AI/ML Engineer.