# 🐳 FastAPI + Docker: DevOps Hands-On Lab

**A FastAPI web app containerized with Docker for a consistent, deploy-anywhere environment.** My hands-on intro to containerization and DevOps workflows.

![Python](https://img.shields.io/badge/Python-0d1117?style=for-the-badge&logo=python&logoColor=dc2626)
![FastAPI](https://img.shields.io/badge/FastAPI-0d1117?style=for-the-badge&logo=fastapi&logoColor=dc2626)
![Docker](https://img.shields.io/badge/Docker-0d1117?style=for-the-badge&logo=docker&logoColor=dc2626)

---

## 🛠️ Tech Stack

- **Language / Framework:** Python, FastAPI
- **Containerization:** Docker
- **Prerequisites:** Docker Desktop (running) and Git

## 🚀 Run it

```bash
git clone https://github.com/n0zzzy/devops-hands-on-lab.git
cd devops-hands-on-lab

docker build -t devops-hands-on-lab .
docker run -d -p 8000:8000 --name devops-lab devops-hands-on-lab
```

Open **http://localhost:8000**. Interactive API docs are at **http://localhost:8000/docs**.

## 🧹 Clean up

```bash
docker stop devops-lab && docker rm devops-lab
```

## 📁 Files

| File | Purpose |
|---|---|
| `main.py` | FastAPI application |
| `requirements.txt` | Python dependencies |
| `Dockerfile` | Container image definition |

---

<sub>Built by <a href="https://github.com/n0zzzy">Russel Carlo</a>.</sub>
