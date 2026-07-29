# Project Structure

> **MentorAI Repository Structure**

---

# Purpose

This document describes the directory structure of the MentorAI project.

The repository is organized using a modular architecture to separate the frontend, backend, AI services, documentation, infrastructure, and development resources.

---

# Repository Structure

```
mentor-ai/
│
├── frontend/
│
├── backend/
│
├── ai-service/
│
├── database/
│
├── docs/
│
├── architecture/
│
├── prompts/
│
├── docker/
│
├── .github/
│
├── README.md
├── LICENSE
└── .gitignore
```

---

# Directory Details

## frontend/

Contains the complete React application.

Responsibilities:

- User Interface
- Authentication Screens
- Dashboard
- AI Chat
- Quiz Module
- Progress Analytics

Technology:

- React
- TypeScript
- Tailwind CSS
- React Router
- Axios

---

## backend/

Contains the Spring Boot application.

Responsibilities:

- Authentication
- User Management
- REST APIs
- Learning Twin APIs
- Database Management

Technology:

- Java 21
- Spring Boot
- Spring Security
- PostgreSQL
- JWT

---

## ai-service/

Contains all AI-related logic.

Responsibilities:

- LangChain
- LangGraph
- RAG Pipeline
- Quiz Generation
- Adaptive Teaching Engine
- Learning Twin Processing

Technology:

- Python
- FastAPI

---

## database/

Contains database resources.

Examples:

- SQL scripts
- ER diagrams
- Schema definitions
- Migration files

---

## docs/

Project documentation.

Includes:

- Product Principles
- Vision
- Requirements
- Architecture
- Roadmap
- API Design

---

## architecture/

Contains architecture diagrams.

Examples:

- System Architecture
- Sequence Diagrams
- Component Diagrams
- Database ERD
- LangGraph Workflow

---

## prompts/

Stores reusable prompts.

Examples:

- Mentor Prompt
- Quiz Prompt
- Summary Prompt
- Interview Prompt
- Revision Prompt

---

## docker/

Contains Docker configuration.

Examples:

- Dockerfiles
- Docker Compose
- Deployment Scripts

---

## .github/

Contains GitHub configuration.

Examples:

- Issue Templates
- Pull Request Templates
- GitHub Actions
- Workflows

---

# Development Guidelines

- Keep business logic inside the backend.
- Keep AI logic inside the AI service.
- Keep UI logic inside the frontend.
- Avoid mixing responsibilities across modules.
- Maintain clear API contracts between services.

---

# Repository Goals

The repository should be:

- Easy to understand
- Easy to scale
- Easy to test
- Easy to deploy
- Easy for contributors to navigate

---

# Future Expansion

As MentorAI grows, additional directories may be introduced, including:

- mobile/
- monitoring/
- infrastructure/
- analytics/
- testing/
- deployment/

The modular structure allows these components to be added without disrupting the existing project organization.
