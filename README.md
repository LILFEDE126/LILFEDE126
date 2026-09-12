# Hi, I'm Federico

I'm a full-stack AI developer with a background in ICT support and system administration.

I build practical AI systems, backend services, and web applications with a focus on retrieval-augmented generation, vector search, reliable data processing, and clear technical documentation.

## What I work on

- Retrieval-augmented generation applications.
- AI agents for document search and question answering.
- Vector retrieval and similarity-based ranking.
- FastAPI backends and REST APIs.
- React and Vite web applications.
- PostgreSQL-backed systems.
- Structured logging, observability, and debugging workflows.
- Local AI applications using Ollama.

## Problems I focus on solving

### Grounding AI responses

I work on pipelines that connect generated responses to retrieved information instead of treating the language model as an authority.

My approach includes:

- controlling the retrieved context;
- checking whether answers are supported by available data;
- validating numerical information when numbers matter;
- using structured output and explicit guardrails;
- keeping deterministic calculations outside the language model;
- streaming responses only when incremental output is useful.

The goal is not to make an AI system sound confident. The goal is to make its behavior easier to inspect, test, and correct.

### Diagnosing retrieval and pipeline failures

AI applications do not always fail completely. Crawling, retrieval, prompt construction, context assembly, and external API calls can each fail in different ways.

I approach these failures by:

1. isolating the scope of the problem;
2. reproducing the behavior under controlled conditions;
3. checking inputs, outputs, logs, and assumptions;
4. testing one change at a time;
5. documenting the cause instead of hiding the symptom.

I use structured HTTP logging and explicit status handling to turn opaque API failures into actionable feedback.

### Connecting technical systems with users

My ICT support and system administration background helps me explain technical problems to non-technical users.

I focus on making clear how:

- query wording affects retrieval;
- context limits affect responses;
- prompt structure influences model behavior;
- database and API errors differ from application failures;
- local services must be configured before an AI workflow can run.

## Technologies

### Backend

- Python.
- FastAPI.
- Flask.
- REST APIs.
- PostgreSQL.
- SQL.
- HTTP middleware.
- Structured logging.

### Frontend

- React.
- Vite.
- JavaScript.
- HTML.
- CSS.

### AI and data

- Retrieval-augmented generation (RAG).
- Embeddings.
- Vector search.
- Cosine similarity.
- TF-IDF.
- Reciprocal Rank Fusion.
- Document processing.
- Ollama.
- Local language models.
- Qdrant.

### Tools and deployment

- Git.
- GitHub.
- Docker.
- Linux.
- Postman.
- Render.

## Featured projects

### BankRagDemo

A local RAG prototype for synthetic banking-support knowledge. It combines FastAPI, PostgreSQL with pgvector, 1024-dimensional multilingual E5 embeddings, Italian full-text search, Reciprocal Rank Fusion, and Ollama-based local generation.

The project is intentionally presented as a prototype: it does not process real customer data, connect to banking systems, or execute financial operations.

[View repository](https://github.com/LILFEDE126/Bank-RAG-demo)

### Demo Searching Backend

FastAPI backend for personalized live-event discovery with JWT authentication, PostgreSQL persistence, external API integration, and hybrid recommendation scoring.

[View repository](https://github.com/LILFEDE126/demo-searching-backend)

### CRM web application

A full-stack CRM demo combining a web interface, backend APIs, and persistent data management.

Repository coming soon.

## Engineering approach

I prefer to understand and document the core logic of the systems I build.

When an AI pipeline produces an unexpected result, I do not treat the model as a black box. I inspect the data flow, retrieval behavior, prompt construction, API responses, logs, database state, and output validation steps.

I use frameworks when they provide value, while keeping important application logic explicit and testable.

I also distinguish clearly between what is implemented, what has been tested, and what remains a future improvement.

## Current focus

I am publishing and documenting complete projects that combine:

- backend engineering;
- databases;
- web applications;
- vector retrieval;
- local AI systems;
- reliable RAG pipelines;
- technical documentation that another developer can follow.

## Contact

- GitHub: [@LILFEDE126](https://github.com/LILFEDE126)
- LinkedIn: [Federico D](https://www.linkedin.com/in/federico-di-ganci-5090aa203)
