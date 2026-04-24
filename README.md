# docker-hello-api

A containerized REST API built with FastAPI and Docker.

## Tech Stack
- Python 3.12 + FastAPI
- Docker (single-container setup)

## Run locally (without Docker)
```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

## Run with Docker
```bash
docker build -t hello-api:v1 .
docker run -d -p 8000:8000 hello-api:v1
```

API is available at: http://localhost:8000

## Endpoints
| Method | Path | Description |
|--------|------|-------------|
| GET | `/` | Hello World response |
| GET | `/health` | Health check |