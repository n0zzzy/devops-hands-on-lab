# FastAPI Application with Docker

Isang web application na binuo gamit ang FastAPI at naka-containerize gamit ang Docker para sa madaling deployment at consistent na environment.

---

## 🛠️ Requirements & Tech Stack

* **Language/Framework:** Python, FastAPI
* **Containerization:** Docker
* **Prerequisites:** 
  * Docker Desktop (kailangang nakabukas)
  * Git

---

## 🚀 Paano Patakbuhin (How to Run)

### 1. Clone ang Repository
Buksan ang terminal/PowerShell at i-clone ang repo:
git clone <ILAGAY_DITO_ANG_GITHUB_REPO_URL_MO>
cd <PANGALAN_NG_FOLDER_MO>

### 2. I-build ang Docker Image
Bumuo ng Docker image gamit ang `Dockerfile`:
docker build -t my-fastapi-app .

### 3. Patakbuhin ang Container
I-run ang container sa background at i-map ang port 8000:
docker run -d -p 8000:8000 --name fastapi-container my-fastapi-app

### 4. Access sa Application
Kapag tumatakbo na ang container, buksan ang browser at pumunta sa:
* **Main API:** http://localhost:8000
* **Interactive Docs (Swagger UI):** http://localhost:8000/docs

---

## 🛑 Management Commands

### Tingnan ang Tumatakbong Container
docker ps

### I-stop ang Container
docker stop fastapi-container

### I-start Ulit ang Container
docker start fastapi-container

### Burahin ang Container (Clean Up)
docker rm fastapi-container

### Burahin ang Unused Containers / Images
docker container prune
