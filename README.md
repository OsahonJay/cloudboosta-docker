# Cloudboosta WordPress Docker Deployment

## Overview
This project deploys a WordPress website using Docker Compose as part of the Cloudboosta DevOps assignment. It containerises WordPress and MySQL, ensuring consistent deployment across environments.

## Architecture
- **wordpress** — WordPress application container (port 8080)
- **db** — MySQL 8.0 database container
- Both services run on a shared Docker network
- Persistent volumes ensure data survives container restarts

## Prerequisites
- Docker Desktop installed and running
- Docker Compose v2+

## How to Run

### Start the containers
```bash
docker compose up -d
```

### Access WordPress
Open your browser and go to: http://localhost:8080

### View logs
```bash
docker compose logs -f
```

### Monitor container resources
```bash
docker stats
```

### Stop the containers
```bash
docker compose down
```

## Submission
- GitHub repo contains `docker-compose.yml` and this README
- Screenshots of deployment and WordPress dashboard included in submission PDF