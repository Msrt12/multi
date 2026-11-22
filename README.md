
# Multi-Container Docker Application

## Architecture

![Multi-Container Docker Architecture](images/architecture.png)

A multi-container application demonstrating containerization, service communication, and application orchestration using Docker and Docker Compose.

## Overview

This project focuses on deploying a distributed application using multiple Docker containers.

The main objective is to demonstrate how independently containerized services can communicate over Docker networks and operate together as a single application.

## Technology Stack

- **Docker** — Application containerization
- **Docker Compose** — Multi-container orchestration
- **Docker Networking** — Communication between services
- **Docker Volumes** — Persistent data storage
- **Linux** — Container runtime environment

## Architecture

```text
                 Client / Browser
                        |
                        v
                Application Entry
                        |
                        v
                Docker Network
                        |
             +----------+----------+
             |                     |
             v                     v
      Application Service     Supporting Services
             |                     |
             +----------+----------+
                        |
                        v
                 Data Storage
```

## Key Features

- Multi-container application deployment
- Containerized application services
- Docker Compose orchestration
- Internal container networking
- Environment-based configuration
- Service lifecycle management
- Reproducible local environments

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Msrt12/multi.git
cd multi
```

### 2. Build Docker Images

```bash
docker compose build
```

### 3. Start the Application

```bash
docker compose up -d
```

### 4. Verify Running Containers

```bash
docker compose ps
```

### 5. View Application Logs

```bash
docker compose logs -f
```

## Container Management

Restart services:

```bash
docker compose restart
```

Rebuild and restart:

```bash
docker compose up -d --build
```

Stop the application:

```bash
docker compose down
```

## Troubleshooting

Inspect running containers:

```bash
docker ps
```

Check container logs:

```bash
docker compose logs
```

Inspect Docker networks:

```bash
docker network ls
```

## Skills Demonstrated

- Docker Containerization
- Multi-Container Architecture
- Docker Compose
- Container Networking
- Linux
- Application Deployment
- Container Troubleshooting

## Author

**Mykola Dmytrash**

- [GitHub](https://github.com/Msrt12)
- [Portfolio](https://msrt12.github.io/portfolio/)
