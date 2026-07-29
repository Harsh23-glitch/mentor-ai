# System Architecture

> **MentorAI – High-Level System Architecture**

---

# Purpose

This document describes the overall architecture of MentorAI and explains how different components interact to deliver an adaptive AI learning experience.

The architecture follows a modular, scalable, and service-oriented design.

---

# High-Level Architecture

```
                        +----------------------+
                        |      React App       |
                        |  (Frontend UI)       |
                        +----------+-----------+
                                   |
                          REST API / JWT
                                   |
                        +----------v-----------+
                        |   Spring Boot API    |
                        | Authentication       |
                        | User Management      |
                        | Learning Data        |
                        +----------+-----------+
                                   |
                  -----------------|------------------
                  |                |                 |
                  |                |                 |
         PostgreSQL          AI Service         File Storage
           Database           (FastAPI)        (Local / AWS S3)
                                   |
                          +--------v---------+
                          |    LangGraph     |
                          +--------+---------+
                                   |
               ---------------------------------------
               |                 |                   |
               |                 |                   |
         LangChain          Vector Database      LLM
        Orchestration     (FAISS / Qdrant)   (Gemini/OpenAI/Groq)
```

---

# System Components

## 1. Frontend

Technology:

- React
- TypeScript
- Tailwind CSS

Responsibilities:

- Authentication
- Chat Interface
- Dashboard
- File Upload
- Progress Analytics
- Quiz Interface

---

## 2. Backend (Spring Boot)

Technology:

- Java 21
- Spring Boot
- Spring Security
- JWT Authentication

Responsibilities:

- User Management
- Authentication
- Session Management
- Learning Twin Storage
- Dashboard APIs
- Quiz APIs

---

## 3. AI Service

Technology:

- Python
- FastAPI

Responsibilities:

- AI Chat
- RAG Pipeline
- Learning Twin Updates
- Adaptive Teaching
- Quiz Generation
- Revision Notes

---

## 4. LangGraph

LangGraph manages the AI workflow.

Responsibilities:

- Route user requests
- Decide teaching strategy
- Retrieve knowledge
- Update Learning Twin
- Generate final response

---

## 5. LangChain

LangChain provides:

- Prompt management
- Document loading
- Embeddings
- Retrieval pipeline
- Output parsing

---

## 6. Vector Database

Development:

- FAISS

Production:

- Qdrant

Responsibilities:

- Store embeddings
- Semantic search
- Document retrieval

---

## 7. PostgreSQL

Stores:

- Users
- Learning Twin
- Chat History
- Quiz Results
- Progress Analytics
- Uploaded File Metadata

---

## 8. Large Language Model (LLM)

Supported providers:

- Google Gemini
- OpenAI GPT
- Groq
- Ollama (Local)

Responsibilities:

- Generate explanations
- Answer questions
- Create quizzes
- Summarise documents

---

# Request Flow

Example:

1. Student asks a question.
2. Frontend sends request to Spring Boot.
3. Spring Boot forwards the request to the AI Service.
4. LangGraph determines the teaching strategy.
5. LangChain retrieves relevant documents.
6. Vector Database returns matching content.
7. LLM generates a personalised response.
8. Learning Twin is updated.
9. Response is returned to the student.

---

# Design Principles

The architecture is designed to be:

- Modular
- Scalable
- Secure
- Maintainable
- AI-first
- Cloud-ready

---

# Future Enhancements

Future versions may include:

- Redis caching
- Kubernetes deployment
- Multi-agent workflows
- Voice interaction
- Real-time collaboration
- Mobile application

---

# Summary

MentorAI separates business logic from AI logic, making the system easier to maintain, test, and scale as new AI capabilities are added.
