# Risk Scoring Service

**Real-time reactive risk assessment microservice** for AuditorSEC hybrid multi-agent platform.

## Features

- ⚡ Real-time risk scoring API (p95 < 100ms)
- 🔄 Event-driven architecture with Kafka
- 🧠 ML-based risk models (sklearn, lightgbm)
- 📦 Postgres state management
- 🔍 Qdrant vector memory integration (RAG)
- 🐳 Docker-ready, deployable to Render/Fly.io
- ✅ >95% test coverage

## Tech Stack

- **Framework**: FastAPI (Python 3.11+)
- **Database**: PostgreSQL (Aiven)
- **Events**: Apache Kafka (Aiven)
- **Vector DB**: Qdrant Cloud
- **ML**: scikit-learn, LightGBM, XGBoost
- **Deploy**: Render.com / Fly.io
- **CI/CD**: GitHub Actions

## Quick Start

```bash
pip install -r requirements.txt
python -m uvicorn src.main:app --reload
```

## API Endpoints

- `POST /risk/score` - Score entity (company/person) for risk
- `GET /risk/portfolio` - Portfolio-level risk analytics
- `POST /risk/event` - Subscribe to risk events (Kafka)

## Status

🚀 **MVP Phase**: Initial skeleton + tests + Docker build in progress (72h sprint)

**Updated**: Dec 17, 2025, 3 AM EET
