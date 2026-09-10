# Hi, I'm Federico

I'm a Full-Stack AI Developer with a background in ICT support and system administration.

I build practical AI systems, backend services, and web applications with a focus on retrieval-augmented generation, vector search, reliable data processing, and clear technical documentation.

## What I work on

- Retrieval-Augmented Generation (RAG) applications
- AI agents for document search and question answering
- Vector retrieval and similarity-based ranking
- FastAPI backends and REST APIs
- React and Vite web applications
- PostgreSQL-backed systems
- Observability, structured logging, and debugging workflows
- Local AI applications using Ollama

## Problems I focus on solving

### Grounding AI responses

I work on pipelines that connect generated responses to retrieved information.

My approach includes:

- controlling the retrieved context;
- validating numerical information;
- checking whether answers are supported by available data;
- using structured output and guardrails;
- streaming responses with NDJSON when incremental processing is useful.

The goal is to reduce unsupported answers and make AI behavior easier to inspect and debug.

### Diagnosing retrieval and pipeline failures

AI applications do not always fail completely. Sometimes crawling, retrieval, prompting, or context construction fails silently or produces incomplete results.

I separate these cases by:

1. Isolating the scope of the problem.
2. Reproducing the behavior under controlled conditions.
3. Testing possible solutions.
4. Reviewing logs, test cases, and concrete hypotheses before escalation.

I also use structured HTTP logging and explicit status handling to turn opaque API failures into actionable feedback.

### Connecting technical systems with users

My ICT and system administration background helps me explain technical problems to non-technical users.

I focus on making clear how:

- query wording affects retrieval;
- context limits affect responses;
- prompt structure influences model behavior;
- API and data retrieval errors differ from application failures.

## Technologies

### Backend

- Python
- FastAPI
- Flask
- REST APIs
- PostgreSQL
- SQL
- HTTP middleware
- Structured logging

### Frontend

- React
- Vite
- JavaScript
- HTML
- CSS

### AI and data

- Retrieval-Augmented Generation (RAG)
- Embeddings
- Vector search
- Cosine similarity
- TF-IDF
- Document processing
- Ollama
- Local language models
- Qdrant

### Tools and deployment

- Git
- GitHub
- Docker
- Linux
- Postman
- Render

## Featured projects

### Demo searching backend

FastAPI backend for personalized content discovery with JWT authentication, PostgreSQL persistence, external API integration, and recommendation scoring.

[View repository](https://github.com/LILFEDE126/demo-searching-backend)

### AI/RAG agent

An AI agent focused on document retrieval, context selection, and grounded question answering.

Repository coming soon.

### CRM web application

A full-stack CRM demo combining a web interface, backend APIs, and persistent data management.

Repository coming soon.

## Engineering approach

I prefer to understand and document the core logic of the systems I build.

When an AI pipeline produces an unexpected result, I do not treat the model as a black box. I inspect the data flow, retrieval behavior, prompt construction, API responses, logs, and output validation steps.

I use frameworks when they provide value, while keeping important application logic explicit and testable.

## Current focus

I am publishing and documenting complete projects that combine:

- backend engineering;
- databases;
- web applications;
- vector retrieval;
- local AI systems;
- reliable RAG pipelines.

## Contact

- GitHub: [@LILFEDE126](https://github.com/LILFEDE126)
- LinkedIn: [Federico D](https://www.linkedin.com/in/federico-di-ganci-5090aa203?utm_source=share_via&utm_content=profile&utm_medium=member_android)
