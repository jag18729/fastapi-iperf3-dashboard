# FastAPI iperf3 Dashboard

A modern, high-performance network testing dashboard built with FastAPI and Next.js.

## Stack

- **Backend**: FastAPI, PostgreSQL, Redis, Celery
- **Frontend**: Next.js 14, TailwindCSS
- **Infrastructure**: Docker, Kubernetes ready
- **Testing**: iperf3 integration

## Quick Start

```bash
# Clone repository
git clone https://github.com/jag18729/fastapi-iperf3-dashboard.git
cd fastapi-iperf3-dashboard

# Start development environment
docker compose up -d
```

## Project Structure

```
├── backend/
│   ├── app/
│   │   ├── api/        # FastAPI routes
│   │   ├── core/       # Core functionality
│   │   ├── models/     # Database models
│   │   └── services/   # Business logic
│   └── tests/          # Backend tests
├── frontend/
│   ├── app/           # Next.js 14 app
│   ├── components/    # React components
│   └── lib/          # Shared utilities
└── k8s/              # Kubernetes configs
```

## Features

- Real-time iperf3 test monitoring
- Historical data analysis
- Test scheduling
- User management
- Result visualization
- API documentation

## Development

```bash
# Backend development
cd backend
pip install poetry
poetry install
poetry run uvicorn app.main:app --reload

# Frontend development
cd frontend
npm install
npm run dev
```

## Documentation

- API: http://localhost:8000/docs
- Frontend: http://localhost:3000
- Monitoring: http://localhost:5555