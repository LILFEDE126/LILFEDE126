# Hi, I'm Federico

I'm a full-stack AI developer with a background in ICT support and system administration.

I build practical AI systems, backend services, and web applications with a focus on retrieval-augmented generation, vector search, deterministic validation, and clear technical documentation.

## What I work on

- Retrieval-augmented generation (RAG) architectures without opaque framework abstractions.
- Static Python AST code inspection and automated architectural verification.
- Hybrid retrieval combining dense vector search (HNSW) and lexical full-text search (GIN) via Reciprocal Rank Fusion.
- FastAPI backends, REST APIs, and Streamlit diagnostic interfaces.
- React and Vite web applications.
- PostgreSQL and `pgvector` data layers.
- Structured logging, concurrency guards, and debugging workflows.
- Multi-provider AI workflows supporting both local models (Ollama) and cloud APIs (Gemini, Groq, OpenRouter).

## Problems I focus on solving

### Grounding AI responses

I work on pipelines that connect generated responses to retrieved information instead of treating the language model as an authority.

My approach includes:

- controlling the retrieved context with explicit similarity and lexical thresholds;
- stopping generation when local context is insufficient instead of guessing;
- validating numerical information (amounts, percentages, technical units, and codes) with exact `Decimal` arithmetic;
- enforcing structured outputs via Pydantic schemas and self-stabilizing retry loops;
- keeping deterministic calculations and AST checks outside the language model;
- isolating a single verifiable hypothesis instead of blending multiple retrieved chunks.

The goal is not to make an AI system sound confident. The goal is to make its behavior easier to inspect, test, and correct.

### Diagnosing retrieval and pipeline failures

AI applications do not always fail completely. Crawling, retrieval, prompt construction, context assembly, and external API calls can each fail in different ways.

I approach these failures by:

1. isolating the scope of the problem;
2. reproducing the behavior under controlled conditions;
3. checking inputs, outputs, logs, and assumptions;
4. testing one change at a time;
5. documenting the cause instead of hiding the symptom.

I use structured UTC logging, explicit event codes, and exponential backoff on transient HTTP errors (such as rate limits) to turn opaque API failures into predictable behavior.

### Connecting technical systems with users

My ICT support and system administration background helps me explain technical problems to non-technical users.

I focus on making clear how:

- query wording and cross-lingual normalization affect retrieval;
- context limits and similarity thresholds affect responses;
- prompt structure and schema constraints influence model behavior;
- database and API errors differ from application failures;
- local services and containers must be configured before an AI workflow can run.

## Technologies

### Backend & Verification

- Python.
- FastAPI.
- Flask.
- Pydantic.
- Static AST analysis (`ast`, `tokenize`, Radon).
- Pytest.
- PostgreSQL & `pgvector`.
- SQL.
- Structured logging.

### Frontend & UI

- React.
- Vite.
- JavaScript.
- Streamlit.
- HTML & CSS.

### AI and data

- Retrieval-augmented generation (RAG).
- Hybrid search (HNSW cosine + PostgreSQL Full-Text GIN).
- Reciprocal Rank Fusion (RRF).
- Numeric grounding and write-barrier validation (`Decimal`).
- Cross-lingual query normalization (EN / ES / IT).
- Ollama (local LLMs and embeddings).
- Cloud LLM APIs (Google Gemini, Groq, OpenRouter, DeepSeek, OpenAI).
- Qdrant.

### Tools and deployment

- Git & GitHub.
- Docker & Docker Compose.
- Linux.
- Postman.
- Render & Streamlit Community Cloud.

## Featured projects

### Bottega Leonardesca & THE Engine

A deterministic hybrid RAG engine, static Python AST inspector, and closed-loop diagnostic solver built without LangChain or LlamaIndex. It structures 13 Python modules across 5 strictly acyclic layers (verified via AST unit tests) and combines PostgreSQL/`pgvector` 3-way retrieval (HNSW + Italian/Simple FTS + Reciprocal Rank Fusion), guarded semaphore routing, `Decimal` numeric write-barrier validation, thread-safe concurrency control, and multilingual support (EN/ES/IT) across local Ollama and free cloud APIs.

Includes a suite of 26 pure unit tests running offline in under 0.5s with zero database or network dependencies.

[View repository](https://github.com/LILFEDE126/BOTTEGA-)

### BankRagDemo

A local RAG prototype for synthetic banking-support knowledge. It combines FastAPI, PostgreSQL with `pgvector`, 1024-dimensional multilingual E5 embeddings, Italian full-text search, Reciprocal Rank Fusion, and Ollama-based local generation.

The project is intentionally presented as a prototype: it does not process real customer data, connect to banking systems, or execute financial operations.

[View repository](https://github.com/LILFEDE126/Bank-RAG-demo)

### Demo Searching Backend (Concert Compass)

FastAPI backend for personalized live-event discovery with JWT authentication, PostgreSQL persistence, external API integration, and hybrid recommendation scoring.

[View repository](https://github.com/LILFEDE126/demo-searching-backend)

### CRM web application

A full-stack CRM demo combining a web interface, backend APIs, and persistent data management.

Repository coming soon.

## Engineering approach

I prefer to understand and document the core logic of the systems I build.

When an AI pipeline produces an unexpected result, I do not treat the model as a black box. I inspect the data flow, retrieval behavior, prompt construction, API responses, logs, database state, and output validation steps.

I use frameworks when they provide value, while keeping core application logic explicit, modular, and testable with pure unit tests.

I also distinguish clearly between what is implemented, what has been tested, and what remains a future improvement.

## Current focus

I am publishing and documenting complete projects that combine:

- backend engineering;
- relational and vector databases;
- web applications;
- hybrid retrieval and deterministic output validation;
- local and cloud AI systems;
- technical documentation that another developer can verify and run.

## Contact

- GitHub: [@LILFEDE126](https://github.com/LILFEDE126)
- LinkedIn: [Federico Di Ganci](https://www.linkedin.com/in/federico-di-ganci-5090aa203)
