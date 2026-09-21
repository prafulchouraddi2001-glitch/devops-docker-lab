# DevOps Docker Lab

A hands-on DevOps learning project that packages a small Python web application with Docker.

## Goals

- Build a simple web application
- Package it in a Docker image
- Run it consistently with Docker Compose
- Practice Git, troubleshooting, and deployment-ready configuration

## Run with Docker Compose

1. Start Docker Desktop and wait for the engine to run.
2. From the project root, run:

   ```powershell
   docker compose up --build
   ```

3. Open `http://127.0.0.1:5000/` in a browser.

To stop and remove the Compose-managed container and network:

```powershell
docker compose down
```

## Health Check

Open `http://127.0.0.1:5000/health`.

Expected response:

```json
{"status":"ok"}
```
