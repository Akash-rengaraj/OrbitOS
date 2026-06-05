# OrbitOS 🪐

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python: FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Frontend: React](https://img.shields.io/badge/Frontend-React-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![Database: PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL_/_pgvector-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![AI Engine: Local LLM](https://img.shields.io/badge/AI_Engine-Ollama-EF4444?logo=ai&logoColor=white)](https://ollama.com/)

OrbitOS is an open-source, centralized corporate operating system and autonomous governance engine. It unifies isolated enterprise data silos—including project management telemetry, financial ledgers, human resource records, and operational wiki documents—into a singular, AI-orchestrated data layer.

Built with enterprise compliance at its foundation, the system implements cryptographic Role-Based Access Control (RBAC) directly inside its data pipelines and large language model (LLM) prompts, ensuring secure data isolation across all organizational tiers.

---

## ⚡ Core Architecture & Features

### 1. Context-Aware RBAC Proxy (Data Guardrails)
OrbitOS intercepts every natural language request through a secure FastAPI middleware proxy. By verifying incoming JSON Web Tokens (JWT), the engine calculates user clearance thresholds. Unauthorized data structures or prompts are intercepted, logged as security compliance anomalies, and sanitized before ever hitting the LLM or database layers.

### 2. Hybrid Neural Query Router (Text-to-SQL + Graph-RAG)
The system eliminates the limitations of standard chatbots by routing conversational queries based on data types. Quantitative requests (financial entries, task metrics) are dynamically translated into deterministic, read-only SQL queries. Qualitative requests (unstructured documentation, meeting transcripts) are parsed via a semantic document pipeline and indexed within a vector store for context retrieval with verified citations.

### 3. Autonomous Telemetry Workers
Background AI agents continuously process event streams from task tracking dashboards and code repositories. The system automatically computes a dynamic **Project Risk Index (PRI)** to actively forecast pipeline delays and budget burn spikes, serving predictive notifications directly to authorized project leads.

---

## 🛠️ The Technical Stack

* **Frontend Client:** React, TailwindCSS, and TypeScript for high-density telemetry dashboard layouts.
* **Gateway API Application:** FastAPI for asynchronous request loops, CORS control, and JWT middleware validation.
* **AI Coordination Framework:** LangGraph / CrewAI for managing deterministic multi-agent operational states.
* **Local Inference Tier:** Ollama hosting open-source models (Llama 3 / Mistral) to guarantee total internal data privacy.
* **Unified Persistence Layer:** PostgreSQL with the `pgvector` extension to consolidate relational records and dense vector embeddings into an atomic database block.

---

## 🚀 Getting Started & Local Installation

### Prerequisites
* Docker & Docker Compose installed locally.
* Python 3.10+ and Node.js 18+ installed.
* Ollama installed locally and running in the background.

### Step 1: Clone the Repository
```bash
git clone [https://github.com/yourusername/OrbitOS.git](https://github.com/yourusername/OrbitOS.git)
cd OrbitOS