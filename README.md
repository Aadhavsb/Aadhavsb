# Aadhav S Bharadwaj

Computer Science & Mathematics student at Case Western Reserve University.
Researcher focused on KV cache compression for scalable, memory-efficient LLM inference,
with a strong interest in software engineering, ML infrastructure, and robust full-stack systems.

---

## Highlight Projects

### Arguably — real-time debate platform
A purpose-built platform for structured, moderated live debates (timed turns, audience voting,
moderation controls, real-time feedback). The architecture separates stateful media transport
from application state: a standalone Node.js mediasoup (WebRTC) SFU handles low-latency audio/video,
Socket.IO coordinates signaling and session state, and Supabase Realtime syncs debate state via
PostgreSQL change notifications. OpenAI powers live transcription and real-time fact-checking.

- Stack: TypeScript, Next.js, Prisma ORM, PostgreSQL (Supabase), mediasoup/WebRTC, Socket.IO, OpenAI
- Live: https://arguably.vercel.app
- Repo: https://github.com/Aadhavsb/arguably

### Blackbox-QA — agentic Q&A over NTSB aviation reports
Ask a natural-language question, get a grounded, cited answer over public NTSB aviation incident
reports. A single Postgres/pgvector store backs keyword search, dense vector search, and SQL
aggregation. Retrieval is hybrid (BM25 + dense, fused with Reciprocal Rank Fusion), and a raw
tool-calling agent (no framework) chooses between hybrid search, read-only SQL queries, and
full-report fetches at runtime. Every request is traced in Langfuse, and a frozen gold set drives
an eval-gated CI pipeline designed to act as a retrieval-regression gate.

- Stack: Python, PostgreSQL + pgvector, hybrid retrieval (BM25 + dense, RRF), tool-calling agent, Langfuse, Docker, GitHub Actions
- Repo: https://github.com/Aadhavsb/blackbox-qa

---

## Toolbox

- Languages: Python, JavaScript/TypeScript, Java, C#, C, R
- Frameworks: Next.js, React, Node.js, Express
- Infra & DB: PostgreSQL, MongoDB, Supabase, Firebase, Vercel, Docker
- AI/ML: PyTorch, Transformers, pgvector, NumPy, SciPy

---

## Reach Me

- Email: bharadwajaadhav@gmail.com
- LinkedIn: https://linkedin.com/in/aadhav-bharadwaj
