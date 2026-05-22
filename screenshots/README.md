![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker)
![Python](https://img.shields.io/badge/Python-3.11-yellow?logo=python)
![Flask](https://img.shields.io/badge/Flask-Web_App-black?logo=flask)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Platform](https://img.shields.io/badge/Platform-Linux-orange?logo=linux)


# 🚀 Docker Flask App

A simple Flask application containerized using Docker.

---

## 📌 Project Objective

This project demonstrates:

- Writing a Dockerfile
- Building Docker images
- Running containers
- Port mapping
- Docker layering concepts

---

## 🛠 Tech Stack

- Python
- Flask
- Docker

---

## 📂 Project Structure

```bash
.
├── app.py
├── requirements.txt
├── Dockerfile
└── README.md
```

---

## 🐳 Dockerfile Used

```Dockerfile
FROM python:3.11

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["python", "app.py"]
```

---

## ⚙ Build Docker Image

```bash
docker build -t flask-app:v1 .
```

---

## ▶ Run Container

```bash
docker run -d -p 5000:5000 --name flask-container flask-app:v1
```

---

## 🌐 Access Application

```bash
http://localhost:5000
```

---

## 📸 Screenshots

### Docker Images
![Docker images](screenshots/docker-ps.png)

### Browser Output
![browser output](screenshots/docker-running.png)

---

## 📚 Concepts Learned

- Dockerfile
- Docker Images
- Containers
- Port Mapping
- Docker Layers
- Docker Build Process

---

## 🧠 Key Learnings

- Difference between image and container
- Why WORKDIR is important
- Why requirements.txt is copied separately
- Importance of port mapping

---

## 🚀 Future Improvements

- Add Docker Compose
- Add MySQL
- Deploy on AWS
- Add NGINX reverse proxy

---

## Author
**Disha Rajput**
Cloud and DevOps enthusiast
