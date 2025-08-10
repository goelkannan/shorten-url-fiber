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

<img width="421" height="202" alt="{AE30F530-F5F6-4D7A-940A-69C54A436E63}" src="https://github.com/user-attachments/assets/1f3e255c-f05e-4245-b1b3-82095f858e2f" />

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
