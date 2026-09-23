# DevOps Docker Lab

A production-oriented Docker and CI foundation project built to learn and demonstrate containerization, automated testing, Git workflows, and GitHub Actions CI.

## Project Objective

The goal of this project is to build a small Python web application and progressively introduce core DevOps practices around it.

This project focuses on:

- Application containerization
- Docker Compose
- Automated unit testing
- Container health checks
- Git and GitHub workflows
- Continuous Integration with GitHub Actions
- CI failure diagnosis and recovery

---

## Architecture

```text
Developer
    |
    | Git
    v
GitHub Repository
    |
    | Push / Pull Request
    v
GitHub Actions
    |
    +----------------------+
    |                      |
    v                      v
Install dependencies    Run unit tests
                           |
                           | Tests pass
                           v
                     Build Docker image
                           |
                           v
                         CI PASS
```
---

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application runtime |
| Flask | Web application framework |
| unittest | Automated unit testing |
| Docker | Application containerization |
| Docker Compose | Local container workflow |
| Git | Version control |
| GitHub | Remote repository |
| GitHub Actions | Continuous Integration |

---

## Project Structure

```text
devops-docker-lab/
│
├── app/
│   └── app.py
│
├── tests/
│   └── test_app.py
│
├── .github/
│   └── workflows/
│       └── ci.yaml
│
├── Dockerfile
├── compose.yaml
├── requirements.txt
└── README.md
