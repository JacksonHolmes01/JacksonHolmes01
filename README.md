# Jackson Holmes

I'm passionate about making AI **secure** and **accessible** for learners. I build free, hands-on training modules that teach anyone to **build secure AI systems**, starting from the database up.

Every module runs on your own laptop with Docker, assumes no prior experience, and explains **what** to do, **why** it matters, and **how to prove** each security control actually works.

---

## Secure AI curriculum

Pick one vector database and follow its series in order. Each series ends with the same skills: a locked-down RAG chatbot, measured defenses against prompt injection, hardened containers, and a red-team exercise against your own system.

| Database | Start here | What makes it interesting |
|---|---|---|
| **PostgreSQL + pgvector** | [Secure AI with pgvector](https://github.com/JacksonHolmes01/Training-Module-Secure-AI-pgvector) | Row-level security keeps tenants apart inside the database itself |
| **Chroma** | [Secure AI with Chroma](https://github.com/JacksonHolmes01/Training-Module-Secure-AI-Chroma) | Chroma has no authentication at all, so you build the protection it is missing |
| **Weaviate** | [Securely Install Weaviate](https://github.com/JacksonHolmes01/Training-Module-Securely-Install-Configure-And-Test-Weaviate), then [Production-Grade RAG: Weaviate](https://github.com/JacksonHolmes01/Training-Module-Production-Grade-RAG-Infrastructure-Weaviate) | Built-in roles and multi-tenancy, and a logging blind spot you will find yourself |
| **Qdrant** | [Production-Grade RAG: Qdrant](https://github.com/JacksonHolmes01/Training-Module-Production-Grade-RAG-Infrastructure-Qdrant) | Signed tokens scoped to a single collection |
| **Milvus** | [Production-Grade RAG: Milvus](https://github.com/JacksonHolmes01/Training-Module-Production-Grade-RAG-Infrastructure-Milvus) | Seven containers, default passwords to remove, and helpers to wall off |

### What every series covers

| Stage | You build or break | You measure |
|---|---|---|
| Secure install | The database, locked down: no open ports, least-privilege accounts, TLS, backups | Every control, tested |
| RAG chatbot | Ollama, FastAPI, NGINX, and Gradio around your database | Retrieval, auth at the edge, read-only chat |
| Prompt injection | Eight attacks (direct, indirect, secret leaks, data theft through images), then four layers of defense | Attacks that succeed: 7 of 8, down to 0 |
| Container hardening | Six layers: non-root, no capabilities, read-only, secrets out of env vars, internal TLS, pinned images | An audit score from about 30% to 100%, and an attacker demo that goes from "yes" to "no" |
| Logging and red team | Structured logs, detection rules, and a scripted 12-step attack on your own lab | Detection coverage, gaps you can fix, and gaps you cannot see |

Everything is open: code under MIT, lessons under CC BY-SA 4.0. If a module helped you, a star helps other learners find it.
