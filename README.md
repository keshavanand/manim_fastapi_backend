# Manim Video Generator

A FastAPI-powered backend to generate Manim animations from natural language prompts, with task management via Celery and Redis.

---

## Features

- Generate Manim animations dynamically using AI prompts  
- Asynchronous video rendering with Celery workers  
- Real-time task monitoring via Flower dashboard  
- Video storage with optional AWS S3 integration  
- Prometheus metrics for monitoring performance  
- Easy Docker-based setup for local development and production  

---

## Tech Stack

- **Backend:** FastAPI  
- **Task Queue:** Celery + Redis  
- **Video Rendering:** Manim + FFmpeg + LaTeX  
- **Database:** MongoDB (Beanie ODM)  
- **Monitoring:** Prometheus + Flower + Grafana (optional)  
- **Containerization:** Docker + Docker Compose  

---

## Getting Started

### Prerequisites

- Docker & Docker Compose installed  
- (Optional) AWS credentials for S3 storage  
- GEMINI AI API KEY

### Run Locally

```bash
git clone <repo-url>
cd manim-app
cp .env.example .env   # configure environment variables
docker-compose up --build -d
