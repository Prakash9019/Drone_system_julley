# 🛸 Drone Intelligence System for India

An end-to-end AI-powered Drone Intelligence Platform designed for the Indian ecosystem, integrating Retrieval-Augmented Generation (RAG), tool-based computation (MCP), and real-time analytics. This system serves as a centralized knowledge hub for drone regulations, business insights, and operational planning.

Developed as part of the JulleyOnline AI/ML Internship, the project demonstrates production-level AI architecture combining LLMs, vector databases, and deterministic services.

---

## 🌟 Key Features

### 🤖 Agentic RAG System
- Implements a Retrieval-Augmented Generation pipeline using OpenAI embeddings and ChromaDB
- Enables semantic search over Drone Rules 2021, regulations, and industry datasets
- Supports multi-modal ingestion (PDF, CSV, text, images)
- Provides grounded responses with source citations

---

### 🧩 MCP Tooling Layer (Deterministic Intelligence)
- Flight Time Calculator (battery, payload, environmental conditions)
- ROI Calculator (investment, revenue, break-even analysis)
- Regulation Compliance Checker (DGCA rules, no-fly zones)
- Drone Recommendation Engine (budget, use-case based filtering)

---

### 📊 Synthetic Data Engine
- Generates 1,000+ simulated drone flight logs
- Enables analytics, testing, and model validation
- Supports scenario-based business simulations

---

### 📡 FastAPI Backend
- Modular API architecture with route separation
- Intelligent routing between RAG and MCP tools
- File upload and dynamic knowledge base updates
- Scalable and deployable service layer

---

### 🖥️ Interactive Dashboard
- Streamlit-based UI with real-time chatbot
- Tool-driven analytics and visualizations
- Document upload and query interface
- Displays responses with source attribution

---

## 🧠 System Highlights
- Combines **probabilistic AI (LLM)** with **deterministic computation (MCP)**
- Implements **semantic retrieval + re-ranking (MMR)**
- Supports **multi-modal RAG ingestion**
- Designed with **modular, scalable architecture**

---

## 🏗️ Project Structure
```text
drone-intelligence-system/
├── api/                  # FastAPI Backend & Endpoints
├── data/                 # Raw, Processed, and Synthetic Datasets
├── docs/                 # Documentation & Architecture Diagrams
├── frontend/             # Streamlit Dashboard Source
├── mcp_server/           # Model Context Protocol (Calculators)
├── rag/                  # Vector Database & Retriever Logic
├── scripts/              # Data Generation & DB Setup Scripts
└── requirements.txt      # Project Dependencies
```

## 🚀 Quick Start Guide

### 1. Environment Setup
Create a virtual environment and install dependencies:

```bash
python -m venv .venv
.venv\Scripts\activate  # Windows
pip install -r requirements.txt
```

### 2. Configuration
Create a `.env` file in the root directory:

```env
OPENAI_API_KEY=your_actual_key_here
```

### 3. Data & Database Initialization
Generate the synthetic datasets and initialize the ChromaDB vector store:

```bash
python scripts/data_generation.py
python scripts/database_setup.py
```

### 4. Launch the Application
Run the backend and frontend in separate terminals:

**Backend:** `uvicorn api.main:app --reload`

**Frontend:** `streamlit run frontend/src/app.py`

## 🛠️ Tech Stack
* **Language**: Python 3.12
* **AI Framework**: LangChain, OpenAI GPT-4o Mini
* **Vector DB**: ChromaDB
* **API Layer**: FastAPI
* **Visualization**: Plotly, Streamlit