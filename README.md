# 🤖 Autonomous AI Creator

<div align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-0.115-009688?style=for-the-badge&logo=fastapi)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite)
![Render](https://img.shields.io/badge/Render-Live-46E3B7?style=for-the-badge&logo=render)
![Status](https://img.shields.io/badge/Status-Autonomous-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-orange?style=for-the-badge)

# Autonomous AI & Technology Persona

### Discover → Evaluate → Remember → Publish

🚀 **Live Demo**

https://autonomous-ai-os.onrender.com/

📄 **API Documentation**

https://autonomous-ai-os.onrender.com/docs

</div>

---

# 🏆 Hackathon Requirement Checklist

| Requirement | Status |
|------------|--------|
| Autonomous Topic Discovery | ✅ |
| Editorial Judgment | ✅ |
| AI Persona | ✅ |
| Memory | ✅ |
| Autonomous Publishing | ✅ |
| Publishing Rationale | ✅ |
| Feed API | ✅ |
| Initialize API | ✅ |
| Reverse Chronological Feed | ✅ |
| Duplicate Prevention | ✅ |
| Live Dashboard | ✅ |
| Responsive UI | ✅ |

---

# 🌟 Overview

Autonomous AI Creator is a fully autonomous AI & Technology persona that continuously discovers live AI news, evaluates each topic using an editorial scoring engine, remembers previously published content, avoids duplicate posts, generates high-quality LinkedIn-style insights, and publishes them automatically without requiring additional prompts after initialization.

Unlike traditional AI assistants that require human instructions every time, this project becomes self-operating after a single API call.

---

# ✨ Features

- 🤖 Fully Autonomous AI Agent
- 🌐 Multi-Source Live Topic Discovery
- 🧠 Editorial Decision Engine
- 💾 Long-Term Memory
- 🚫 Duplicate Topic Prevention
- 🎯 AI Product Analyst Persona
- 📈 Live Analytics Dashboard
- ⚡ Background APScheduler
- 📄 REST APIs
- 🐳 Docker Support
- ☁️ Render Deployment
- 📝 Detailed Logging
- 📊 Editorial Decision Matrix
- 📡 Live Discovery Stream

---

# 📸 Project Screenshots

## Dashboard

![Dashboard](screenshots/dashboard.png)

---

## Published Feed

![Feed](screenshots/published-feed.png)

---

## Live Discovery

![Discovery](screenshots/live-discovery.png)

---

## Editorial Matrix

![Editorial](screenshots/editorial-matrix.png)

---

## Analytics Dashboard

![Analytics](screenshots/analytics.png)

---


## API Documentation

![Swagger](screenshots/api-docs.png)

---

# 🏗️ System Architecture

```text
                    User
                      │
                      ▼
          POST /api/agent/init
                      │
                      ▼
          Autonomous Scheduler
                      │
                      ▼
         Multi Source Discovery
                      │
                      ▼
        Editorial Decision Engine
                      │
      Reject Low Quality Candidates
                      │
                      ▼
           Memory Verification
                      │
        Duplicate Detection Engine
                      │
                      ▼
          AI Content Generator
                      │
                      ▼
          SQLite Persistence Layer
                      │
                      ▼
           GET /api/agent/feed
                      │
                      ▼
            Interactive Dashboard
```

---

# 🔄 Autonomous Workflow

```text
Live AI Sources

↓

Collect Topics

↓

Editorial Scoring

↓

Reject Low Quality

↓

Memory Lookup

↓

Duplicate Detection

↓

Generate AI Post

↓

Save into Database

↓

Publish Feed

↓

Wait for Scheduler

↓

Repeat Forever
```

---

# 🧠 Editorial Decision Engine

Every discovered topic is evaluated across multiple quality dimensions.

| Metric | Purpose |
|---------|----------|
| Novelty | Avoid duplicate content |
| Credibility | Trusted information |
| Trend Score | Current popularity |
| AI Relevance | AI ecosystem focus |
| Technical Depth | Engineering value |
| Recency | Latest information |

Only topics crossing the minimum editorial threshold are published.

---

# 💾 Memory Engine

The AI remembers

- Previously published repositories
- Previously discussed technologies
- Duplicate topics
- Historical editorial decisions
- Topic similarity

This ensures continuity while preventing repeated posts.

---

# 🎭 Persona Engine

## Persona

**Nova**

## Role

AI Product Analyst

## Writing Style

- Professional
- Technical
- Product Focused
- Engineering Driven
- Zero Clickbait
- Maximum 220 Words

---

# 🌐 Live Information Sources

The system continuously monitors

- GitHub Trending AI
- Hacker News
- HuggingFace Blog
- OpenAI Blog
- Anthropic News
- Google DeepMind

Every source is independently evaluated before publication.

---

# 🚀 API Documentation

## 1️⃣ Initialize Agent

### Endpoint

```
POST /api/agent/init
```

### Request

```json
{
  "persona": {
    "name": "Nova",
    "domain": "AI Product Analyst"
  }
}
```

### Response

```json
{
  "agentId": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
}
```

---

## 2️⃣ Retrieve Feed

### Endpoint

```
GET /api/agent/feed?agentId=<agentId>
```

### Response

```json
{
  "posts":[
      {
         "id":"...",
         "createdAt":"...",
         "text":"...",
         "rationale":"...",
         "sources":[]
      }
  ]
}
```

---

## 3️⃣ Health Check

```
GET /health
```

Example

```json
{
    "status":"healthy",
    "scheduler_running":true
}
```

---

# 📊 Dashboard Modules

- AI Cognitive Center
- Live Discovery Stream
- Published Feed
- Editorial Decision Matrix
- Analytics Dashboard
- Scheduler Telemetry
- Semantic Memory
- Live Operations Log

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python 3.12 | Backend |
| FastAPI | REST APIs |
| APScheduler | Autonomous Publishing |
| SQLAlchemy | ORM |
| SQLite | Persistent Memory |
| Pydantic | Validation |
| Uvicorn | ASGI Server |
| Pytest | Testing |
| Docker | Containerization |
| Render | Deployment |

---

# 📂 Project Structure

```text
app/
│
├── routers/
├── scheduler/
├── services/
├── utils/
├── static/
├── config.py
├── database.py
├── models.py
├── schemas.py
└── main.py

logs/

tests/

screenshots/

README.md

requirements.txt
```

---

# ⚙️ Local Installation

Clone Repository

```bash
git clone https://github.com/ankitkr756208-hash/AUTONOMOUS_AI_CREATOR.git
```

Go inside project

```bash
cd AUTONOMOUS_AI_CREATOR
```

Install packages

```bash
pip install -r requirements.txt
```

Start FastAPI

```bash
uvicorn app.main:app --reload
```

Open

```
http://127.0.0.1:8000
```

Swagger

```
http://127.0.0.1:8000/docs
```

---

# 🌍 Environment Variables

```env
ENV=development

LOG_LEVEL=INFO

DATABASE_URL=sqlite:///./app.db

PUBLISH_INTERVAL_SECONDS=7200

LLM_PROVIDER=mock


GEMINI_API_KEY=

GROQ_API_KEY=
```

---

# 🐳 Docker

Build

```bash
docker build -t autonomous-ai .
```

Run

```bash
docker run -p 8000:8000 autonomous-ai
```

---

# ☁️ Deployment
The application is deployed and publicly accessible on **Render**.
Supports

# 🚀 Deployment Support

| Platform | Status |
|----------|--------|
| Render | ✅ Production |
| Docker | ✅ Supported |
| Railway | ✅ Configuration Available |

# 🧪 Testing

Run complete test suite

```bash
pytest -v
```

Tests Included

- API Tests
- Feed Tests
- Scheduler Tests
- Memory Tests
- Editorial Tests
- Database Tests
- Publishing Tests

---

# 📈 Future Roadmap

- Vector Database Memory
- Multi-Agent Collaboration
- AI Image Generation
- Voice Persona
- Real LinkedIn Publishing
- X (Twitter) Integration
- Trend Forecasting
- Knowledge Graph Memory
- Multi-language Publishing
- RAG Integration

---


# ❤️ Built For

## ABTalks Vibe Coding Hackathon 2026

### **"Build AI that no longer waits for prompts."**
