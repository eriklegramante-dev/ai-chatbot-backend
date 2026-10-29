# 🤖 SYNTH_MATH // 1984 — Backend Engine

> Modular Full Stack AI platform featuring intelligent multi-agent orchestration, clean architecture, and containerized infrastructure.

---

## 🚀 Overview

**SYNTH_MATH // 1984** is an enterprise-grade backend service built to demonstrate proficiency in Full Stack systems engineering, clean software architecture, and DevOps practices. The platform integrates a resilient REST API, autonomous domain-specialized AI agents, structured conversation memory, and an isolated containerized environment.

---

## ✨ Tech Stack

### Backend Core
- Python 3.11+
- FastAPI (Asynchronous Web Framework)
- Pydantic v2 (Data Validation & Settings Management)

### AI & Multi-Agent Orchestration
- CrewAI (Agent Orchestration Framework)
- LiteLLM (Unified Multi-Model Gateway)
- Groq (Llama 3 Execution Engine)
- Google Gemini (Analytical & Fallback Model)

### Frontend Client
- React / Next.js
- Tailwind CSS
- Retro Synthwave / Cyberpunk Aesthetic

### Infrastructure & DevOps
- Docker & Docker Compose
- Isolated Bridge Networks
- Fine-grained CORS Policies
- Structured File & Console Logging

### Quality Assurance & Testing
- Pytest (Automated Test Runner)
- Pytest-Cov (Coverage Reporting)
- OpenAPI / Swagger Interactive Documentation
- Agent Reasoning & Prompt Validation Tests
- State & Conversation Memory Diagnostics

---

## 🏗 System Architecture

```text
React / Next.js Client
          │
          ▼  HTTP / JSON
   FastAPI REST API
          │
          ▼
   Task Orchestrator
   ├── Senior Mathematician Agent
   └── Retro-Futuristic Writer Agent
          │
          ▼
   Conversation Memory Manager
          │
          ▼
   LiteLLM Gateway
   ├── Groq (Llama 3)
   └── Google Gemini
```

---

## 📂 Project Structure

```text
chat-bot-backend/
├── logs/
│   └── app.log
├── src/
│   ├── agents/
│   │   ├── mathematician.py     # Complex reasoning & math agent
│   │   └── writer.py            # Multilingual retro copywriter agent
│   ├── config/
│   │   ├── llm.py               # Model provider configurations
│   │   └── logger_config.py     # Centralized logging engine
│   ├── memory/
│   │   └── memory_manager.py    # Conversation state & history persistence
│   ├── orchestrators/
│   │   └── orchestrator.py      # CrewAI pipeline execution coordinator
│   ├── schemas/
│   │   └── schemas.py           # Pydantic request & response contracts
│   ├── tools/
│   │   └── tools.py             # Domain-specific agent toolsets
│   └── utils/
│       └── validation.py        # Input sanitization & boundary checks
├── tests/                       # Unit, integration, and agent test suites
├── .env.example
├── Dockerfile
├── docker-compose.yml
├── main.py                      # Application entrypoint & route registry
├── pytest.ini
└── requirements.txt
```

---

## 🤖 Autonomous Agents

### Senior Mathematician Agent
- Resolves complex analytical, algebraic, and algorithmic problems.
- Preserves mathematical context across sequential dialogue turns.
- Generates step-by-step verifiable deductions.

### Multilingual Retro-Futuristic Copywriter
- Produces tailored creative and technical copy across multiple languages.
- Strictly adheres to the retro-futuristic 1980s / Synthwave thematic voice.
- Synthesizes technical inputs into accessible, styled narratives.

---

## ⚙️ Installation & Deployment

### Prerequisites
- Docker & Docker Compose **or** Python 3.11+
- API keys for target LLM providers (Groq, Google Gemini)

### Method 1: Containerized (Recommended)

```bash
git clone [https://github.com/eriklegramante-dev/ai-chatbot-backend.git](https://github.com/eriklegramante-dev/ai-chatbot-backend.git)
cd ai-chatbot-backend 

cp .env.example .env
# Edit .env with your API credentials

docker compose up --build
```

### Method 2: Local Environment

```bash
git clone [https://github.com/eriklegramante-dev/ai-chatbot-backend.git](https://github.com/eriklegramante-dev/ai-chatbot-backend.git)
cd ai-chatbot-backend

python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt

cp .env.example .env
# Edit .env with your API credentials

uvicorn main:app --host 0.0.0.0 --port 8000 --reload
```

---

## 🧪 Testing & Quality Assurance

Run the automated test suite using `pytest`:

```bash
# Run all tests
pytest

# Verbose output with execution metrics
pytest -v

# Run with test coverage report
pytest --cov=src tests/
```

Interactive functional verification and API contract testing are available via Swagger UI.

---

## 📡 API Documentation

Once the service is running, explore the self-documenting API endpoints:

- **Swagger UI:** `http://localhost:8000/docs`
- **ReDoc:** `http://localhost:8000/redoc`

---

## 🎯 Engineering Highlights

- **Decoupled Architecture:** Strict separation of concerns across presentation, orchestration, and model abstraction layers.
- **Robust Schema Enforcement:** End-to-end data validation and schema serialization powered by Pydantic.
- **Production-Ready Containerization:** Multi-stage Docker setup ensuring environment parity across development and deployment.
- **Model Agnosticism:** Unified LLM provider routing via LiteLLM to eliminate vendor lock-in.
- **Traceable Observability:** Structured log emission with automatic rotation and detailed error tracking.

---

## 🔮 Roadmap

- [ ] Response streaming via Server-Sent Events (SSE)
- [ ] Distributed cache and session persistence with Redis
- [ ] Vector database integration (ChromaDB / Qdrant) for RAG capabilities
- [ ] Application telemetry and tracing (OpenTelemetry / Prometheus)
- [ ] Automated CI/CD test and build pipelines (GitHub Actions)
- [ ] Production deployment manifests (Helm / Kubernetes)

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.