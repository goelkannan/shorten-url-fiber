# 🔗 URL Shortener

A high-performance, Dockerized URL shortener built with Go (Fiber), Redis, and HTML/CSS. Supports fast redirection with sub-15ms latency and scalable architecture.

![Go](https://img.shields.io/badge/Go-1.20-blue?logo=go) ![Redis](https://img.shields.io/badge/Redis-InMemory-red?logo=redis) ![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker)

---

## 🚀 Features

- 🔐 Generate short links for any URL
- ⚡ Sub-15ms redirect latency using Redis
- ♻️ Configurable expiry for short URLs
- 📊 Store click metadata (optional)
- 🐳 Dockerized for easy deployment

---

## 📂 Project Structure

shorten-url-fiber/
├── api/
│ ├── database/ # Redis client init
│ ├── helpers/ # Random string, URL validation, etc.
│ ├── routes/ # shorten and redirect route handlers
│ ├── .env # Env config (PORT, Redis)
│ ├── Dockerfile # API container
│ ├── go.mod / go.sum # Go dependencies
│ └── main.go # App entry point
├── db/ # Optional Redis config/data
└── docker-compose.yml # Docker Compose for Redis + API
---

## 🛠️ Tech Stack

- **Backend:** Go, Fiber
- **Database:** Redis (in-memory)
- **Deployment:** Docker + Docker Compose
- **Frontend:** HTML, CSS (basic interface)

---

## 📦 Setup & Run (Local)

> Make sure Docker and Docker Compose are installed.

# Clone the repository
git clone https://github.com/goelkannan/shorten-url-fiber.git
cd shorten-url-fiber

# Build and run containers
docker-compose up --build -d
