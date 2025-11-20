# CPF_Knowledge_Assistant

This project develops a Retrieval-Augmented Generation (RAG) chatbot for CPF, designed to centralize and retrieve distributed organizational knowledge across the Feed–Farm–Food operations.
The system can understand natural language questions, search internal documents, synthesize accurate answers, and support employees in decision-making with reliable information.

🎯 Core Features
- Natural Language Q&A (Thai & English) powered by LLM
- Full RAG Pipeline: Retrieve → Rerank → Assemble → Generate → Validate
- Intent Detection & Question Rewriting for improved accuracy
- End-to-end Data Pipeline: OCR, Chunking, Captioning, Embedding
- Semantic Search using Qdrant Vector Database
- User & Admin Modules
- Users: chat, conversation history, feedback rating
- Admins: upload/edit documents, dashboard, FAQ insights, system prompt management
- LLM-powered summarization with context-grounded answers
- Conversation history & user data stored in PostgreSQL

🏗 System Architecture
- Frontend: Next.js
- Backend API: FastAPI
- Vector Database: Qdrant
- Relational Database: PostgreSQL
- AI Models: HuggingFace (OCR, Embedding, Captioning) + external LLM
- RAG Components: Hybrid retrieval, reranker, context assembler, validation layer
- Deployment: Docker containers

📂 Main Pipelines
1) Data Pipeline
   - OCR / image captioning
   - Text chunking
   - Embedding generation
   - Store vectors in Qdrant
2) RAR Pipeline (Retrieval-Augmented Reasoning)
   - Query preprocessing
   - Hybrid retrieval (vector + keyword/metadata)
   - Cross-encoder reranking
   - Evidence assembly
   - Prompt building
   - LLM reasoning / grounded generation
   - Validation layer (hallucination check, numeric accuracy, schema validation)
   - Answer rendering
3) User Workflow
   - Ask → Rewrite → Intent → Retrieve → Reason → Validate → Answer → Save history

🛠 Tech Stack
- Next.js (frontend)
- FastAPI (backend)
- Python (AI pipelines)
- Qdrant (vector search)
- PostgreSQL (user data & history)
- HuggingFace Models
- Docker
- Git / GitHub
- VS Code
