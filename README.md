# Listmonk White Label for Fast Testing 

This project provides a ready-to-use Listmonk environment using Docker Compose.

The goal is to quickly spin up a complete local stack for:

* development
* testing
* DevOps labs
* self-hosted experiments
* API integrations
* newsletter automation
* infrastructure studies
* container orchestration learning

---

# What is Listmonk?

Listmonk is a high-performance open source newsletter and mailing list manager.

Main features:

* newsletter campaigns
* subscriber management
* mailing lists
* REST API
* automation support
* segmentation
* modern admin dashboard
* SMTP support
* self-hosted architecture

Official website:

[Listmonk Official Website](https://listmonk.app?utm_source=chatgpt.com)

Official repository:

[Listmonk GitHub](https://github.com/knadh/listmonk?utm_source=chatgpt.com)

---

# Included Stack

This environment automatically starts:

* PostgreSQL
* Redis
* Docker
* Docker Compose
* Listmonk

---

# Default Application Port

The application runs by default on:

```bash id="vg9ctv"
http://localhost:9000
```

---

# Default Credentials

Username:

```text id="mhl5zy"
admin
```

Password:

```text id="qzbj5z"
listmonk
```

---

# Getting Started

## 1. Clone the repository

```bash id="0awp0v"
git clone <repository>
cd <repository>
```

---

## 2. Configure environment variables

This project already includes an `.env-example` file.

Copy it:

```bash id="g3fq1v"
cp .env-example .env
```

Edit the `.env` file with your own configuration if needed.

---

## 3. Start the containers

```bash id="y7h4s9"
docker compose up -d
```

---

## 4. Verify running containers

```bash id="u7eb4q"
docker ps
```

---

# Available Services

| Service    | Port |
| ---------- | ---- |
| Listmonk   | 9000 |
| PostgreSQL | 5432 |
| Redis      | 6379 |

---

# Useful Commands

## View Listmonk logs

```bash id="qf9e2z"
docker logs -f listmonk
```

---

## Access PostgreSQL container

```bash id="l4m2du"
docker exec -it postgres sh
```

---

## Connect to PostgreSQL

```bash id="s7p1xo"
psql -U admin -d listmonk
```

---

## List databases

```sql id="v9z0j2"
\l
```

---

## List tables

```sql id="h5t3fr"
\dt
```

---

## Exit PostgreSQL

```sql id="f0m8na"
\q
```

---

# Architecture Overview

```text id="t2d1sk"
Listmonk
   │
   ├── PostgreSQL
   ├── Redis
   └── Docker Compose
```

---

# Project Purpose

This repository acts as a lightweight "white label" setup for rapidly testing and experimenting with Listmonk.

It allows developers and students to:

* quickly deploy a complete environment
* study containerized architectures
* practice Docker Compose
* explore self-hosted applications
* test integrations and APIs
* create local DevOps labs

---

# Future Improvements

* SMTP integrations
* Reverse proxy with Nginx
* HTTPS with Traefik
* OAuth authentication
* Automated backups
* Monitoring stack
* CI/CD pipelines
* VPS deployment templates

---
