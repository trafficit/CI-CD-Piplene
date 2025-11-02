# CI-CD-Piplene
CI/CD for FastAPI + Telegram Bot


# FastAPI CI/CD Demo with Telegram Bot

This project demonstrates a production-ready FastAPI application with CI/CD pipeline using GitHub Actions, Docker, and Telegram bot integration.

##  Features

- FastAPI backend with health check
- Telegram bot with conversation flow
- CI/CD pipeline: build, test, Dockerize, deploy
- `.env` secrets injected via GitHub Actions
- Dockerfile + docker-compose for reproducible deployment

##  Technologies

- FastAPI · Uvicorn · Docker · GitHub Actions · Telegram Bot API · systemd · Caddy

##  Project Structure
fastapi-ci-demo/ 
├── app/ 
│ └── main.py 
├── bot/ 
│ └── bot.py 
├── requirements.txt 
├── Dockerfile 
├── docker-compose.yml 
├── .env.example 
└── .github/ 
└── workflows/ 
└── deploy.yml


##  CI/CD Pipeline

- Trigger: push to `main`
- Steps:
  - Checkout code
  - Install dependencies
  - Run tests (placeholder)
  - Build Docker image
  - Inject secrets from GitHub
  - Deploy or run app

##  Telegram Bot

The bot collects user name, email, and project description, then sends it to the admin via Telegram.

##  Setup

```bash
cp .env.example .env
docker-compose up --build

