#  AI-First CRM HCP Module (Final Submission)

## 📌 Overview

This project is an **AI-first CRM system** designed for **Healthcare Professional (HCP) interaction management**, built as part of Round 1 Technical Assignment.

It enables field representatives to **log, analyze, and manage interactions** using:

- Structured Form Interface
- Conversational AI Interface (LangGraph Agent)

This system demonstrates how AI can enhance CRM workflows in the **Life Sciences domain**.

---

## 🎯 Assignment Objective

As per the assignment requirements :contentReference[oaicite:1]{index=1}:

- Build a **Log Interaction Screen**
- Support **dual input modes (Form + Chat)**
- Use:
  - React + Redux (Frontend)
  - FastAPI (Backend)
  - LangGraph (AI Agent)
  - Groq LLM (gemma2-9b-it)
- Implement **minimum 5 AI tools**
- Demonstrate complete working system

---

## 🧠 Key Features

### 🔹 Dual Interaction Logging
- Structured form-based logging
- Conversational AI logging

### 🔹 AI-Powered Processing
- Automatic entity extraction
- Intelligent summarization
- Sentiment classification
- Follow-up recommendation

### 🔹 Real-time CRM Workflow
- Log → Analyze → Update → Recommend

---

## 🏗 Architecture

```

Frontend (React + Redux)
↓
FastAPI Backend
↓
LangGraph Agent
↓
Tool Selection (LLM-driven)
↓
Groq LLM Processing
↓
Database (PostgreSQL / SQLite)

```

---

## 🤖 LangGraph Agent (Core Component)

The LangGraph agent acts as an **AI orchestrator**:

- Understands user intent using LLM
- Dynamically selects appropriate tools
- Maintains interaction context
- Generates structured outputs

👉 Flow:

```

User Input → LangGraph Router → Tool Selection → Tool Execution → Response

````

---

## 🛠 AI Tools Implemented (MANDATORY)

### 🔴 1. Log Interaction (Required)
- Converts natural language → structured CRM data
- Extracts:
  - HCP Name
  - Topics
  - Sentiment
  - Follow-up actions

---

### 🔴 2. Edit Interaction (Required)
- Updates existing interaction records
- Example:
  - Change sentiment
  - Modify outcomes

---

### 🟡 3. Summarization Tool
- Converts raw notes → structured summary
- Includes:
  - Executive summary
  - Key points
  - Business impact

---

### 🟡 4. Sentiment Analysis Tool
- Classifies:
  - Positive / Neutral / Negative
- Provides reasoning + confidence

---

### 🟡 5. Follow-up Recommendation Tool
- Suggests next actions:
  - Meeting
  - Sample sharing
  - Product discussion

---

### 🟢 Bonus Tools

- Extract Entities
- Validate Interaction (Compliance Check)

---

## 💻 Tech Stack

| Layer | Technology |
|------|-----------|
| Frontend | React, Redux Toolkit, Tailwind CSS |
| Backend | FastAPI (Python) |
| AI Agent | LangGraph |
| LLM | Groq (gemma2-9b-it) |
| Database | PostgreSQL / SQLite |

---

## ▶️ How to Run

### 🔹 Frontend

```bash
npm install
npm run dev
````

---

### 🔹 Backend

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## 🔐 Environment Variables

```env
GROQ_API_KEY=your_api_key_here
DATABASE_URL=your_db_url
```

---

## 🧪 Example Prompts

Use these in chat:

* "Met Dr. Sharma, discussed Product A, positive response"
* "Summarize my last interaction"
* "Suggest follow-up actions"
* "Change sentiment to neutral"
* "Check if interaction is valid"

---

## 🎥 Demo Coverage (As Required)

The system demonstrates:

* ✅ Logging interaction (chat + form)
* ✅ Summarization
* ✅ Sentiment analysis
* ✅ Follow-up generation
* ✅ Editing interaction
* ✅ LangGraph orchestration

---

## 🧠 Key Learnings

* AI agents can automate CRM workflows
* LangGraph enables structured tool orchestration
* LLMs can convert unstructured data into actionable insights
* Real-world systems require both UI + AI integration

---

## 👨‍💻 Author

Manish Ranjan
