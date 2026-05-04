# Reva Electronics

A full-stack web application with an Express backend and a React frontend.

## Docker Setup

This project is fully containerized with Docker Compose.

### Services

| Service | Description | Dockerfile |
|---------|-------------|------------|
| **backend** | Express / TypeScript API server | `backend/Dockerfile` |
| **frontend** | React / Vite SPA served by Nginx | `frontend/Dockerfile` |

### Quick Start

```sh
docker compose up --build
```

- **Frontend** → http://localhost:3000
- **Backend API** → http://localhost:4000

The Nginx reverse proxy routes `/api/*` requests to the backend service automatically.

### Build Images Only

```sh
docker compose build
```

### Stop Services

```sh
docker compose down
```
