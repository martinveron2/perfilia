# PERFILIA

> Professional identity and career intelligence platform.

## Status

**Phase:** Pre-MVP  
**Version:** 0.1.0  
**Repository:** Private product source of truth

## Vision

PERFILIA is a platform that turns a person's professional trajectory into a structured, evolving professional identity and uses it to evaluate opportunities, identify gaps, and guide career decisions.

## MVP

1. Create/import a professional profile.
2. Structure experience, education, skills, certifications, languages, and goals.
3. Add a job opportunity as text or URL.
4. Extract and structure requirements.
5. Compare the opportunity with the professional profile.
6. Explain strengths, gaps, uncertainty, and recommendations.
7. Keep an analysis history.

## Architecture direction

Initial implementation: web application with a modular monolith architecture.

- Frontend: React + TypeScript
- Backend: Python + FastAPI
- Database: PostgreSQL
- AI: provider-agnostic orchestration layer
- Cloud: local development first; AWS after MVP validation

## Repository structure

```text
perfilia/
├── docs/
│   ├── product/
│   ├── architecture/
│   ├── decisions/
│   ├── ai/
│   └── security/
├── frontend/
├── backend/
├── tests/
├── scripts/
└── infrastructure/
```

## Engineering principles

- Product decisions are documented.
- Code is versioned.
- Secrets never live in Git.
- Development, staging, and production remain separated.
- Matching must be explainable.
- AI must not invent experience, credentials, or achievements.
- Personal data is minimized and user-controlled.
- Prefer a modular monolith before introducing microservices.
- Every important change must be reproducible from the repository.

## Documentation

Project strategy and product documentation are maintained in the project's central knowledge base. Technical documentation that is required to reproduce or maintain the software belongs in this repository under `docs/`.

## Development

Development setup will be documented when the initial application scaffold is created.

## License

Not licensed for public reuse at this stage.
