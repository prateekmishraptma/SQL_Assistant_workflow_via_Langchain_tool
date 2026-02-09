# 🧠 SQL Assistant Skill using LangChain (Multi-Agent)

This project demonstrates how to build a **SQL Assistant Skill** using **LangChain’s multi-agent framework**, following the official LangChain documentation on **Skills-based Agents**.

The notebook showcases how LLM-powered agents can intelligently interpret user queries, generate SQL, execute it against a database, and return human-readable answers — all through a structured skill-based architecture.

📘 Reference Documentation:  
https://docs.langchain.com/oss/python/langchain/multi-agent/skills-sql-assistant

---

## 🚀 What This Project Demonstrates

- ✅ Skill-based agent design using LangChain
- ✅ Natural language → SQL query translation
- ✅ Database interaction via a dedicated SQL skill
- ✅ Multi-step reasoning and execution by an LLM agent
- ✅ Clean separation of responsibilities (Agent ↔ Skill ↔ Tool)

This notebook is intended to **showcase LangChain’s agent orchestration capabilities**, not just SQL querying.

---

## 🧩 Architecture Overview

**High-level flow:**

1. User asks a question in natural language
2. Agent interprets intent
3. SQL Skill:
   - Generates SQL query
   - Executes it on the database
   - Retrieves results
4. Agent converts results into a readable response

User Query
↓
LangChain Agent
↓
SQL Skill
↓
Database
↓
Formatted Answer
<img width="359" height="598" alt="image" src="https://github.com/user-attachments/assets/1c8d5989-2ed2-43a5-860e-1f62a466416d" />


---

## 📂 Project Structure

SQL_Assistant_Skill_via_Langchain.ipynb # Main Jupyter notebook
README.md # Project documentation
requirements.txt # Python dependencies


---

## 🛠️ Technologies Used

- **LangChain (Python)**
- **OpenAI / LLM-backed models**
- **SQL Database (via LangChain SQL tools)**
- **Jupyter Notebook**
- **Python 3.9+**

---

## 📦 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone <your-repo-url>
cd <your-repo-name>
2️⃣ Create Virtual Environment (Optional but Recommended)
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Set Environment Variables
export OPENAI_API_KEY="your_api_key_here"
(Windows PowerShell)

setx OPENAI_API_KEY "your_api_key_here"
▶️ How to Run
Open Jupyter Notebook:

jupyter notebook
Open:

SQL_Assistant_Skill_via_Langchain.ipynb
Run cells sequentially to see:

Agent creation

Skill definition

SQL reasoning

Query execution

Final responses

🎯 Key Learning Outcomes
How LangChain Skills encapsulate reusable capabilities

How agents decide when to invoke skills

How to design production-style agent workflows

How to bridge LLMs with structured databases

🔮 Future Enhancements
Add multiple skills (CSV, API, RAG)

Integrate vector search + SQL hybrid querying

Add memory for conversational querying

Deploy as an API using FastAPI or LangServe

🤝 Who This Is For
AI / ML Engineers

LLM Application Developers

LangChain learners

Anyone exploring agentic AI systems

⭐ Acknowledgements
This implementation is inspired by the official LangChain documentation on Multi-Agent Skills:
https://docs.langchain.com/oss/python/langchain/multi-agent/skills-sql-assistant
