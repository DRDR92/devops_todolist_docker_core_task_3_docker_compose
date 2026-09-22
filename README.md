# Django Todolist - Docker Compose Setup

Multi-container Django ToDo application with MySQL database and persistent volumes.

## Project Overview
Django-based todolist application deployed with Docker Compose.
This project from Mate Academy demonstrates containerization, service orchestration, and database persistence.

## What I Implemented
- **Docker Compose orchestration** - coordinated app and database services
- **MySQL integration** - persistent database with Docker volumes
- **Entrypoint automation** - migrations and app startup in single command
- **Volume management** - persistent data storage for MySQL
- **Environment configuration** - proper separation of config and secrets
- **Service networking** - app-to-database communication

## Services
- **Web**: Django application (Port 8000)
- **Database**: MySQL with persistent volume

## Technologies
- Docker & Docker Compose
- Django 4+
- MySQL 8.0+
- Python 3.8+

## Quick Start
```bash
docker-compose up -d
docker-compose logs -f web
# App available at http://localhost:8000
```

## Container Management
```bash
# View logs
docker-compose logs web

# Stop containers
docker-compose down

# Stop with volume cleanup
docker-compose down -v
```

## Project Structure
- `docker-compose.yml` - Multi-container orchestration
- `Dockerfile` - Application container configuration
- `INSTRUCTION.md` - Detailed deployment guide

## Key Learnings
- Docker Compose for local development
- Database migration automation in containers
- Persistent volume management
- Service networking and dependencies
- Container lifecycle management
