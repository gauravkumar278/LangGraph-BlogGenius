## 🧠 LangGraph BlogGenius

> **AI-powered autonomous blog writer agent** built with [LangGraph](https://github.com/langchain-ai/langgraph), using [Tavily](https://tavily.com/) for real-time trend research and OpenAI for content creation.  
> Open-source for creators, marketers, devs — and anyone who wants to automate blog writing with smart, modular AI agents.

---

### 🌟 Features

- 🔍 **Trending Topic Discovery** with Tavily (real-time search)
- 🧩 **Modular Agent Flow** using LangGraph
- 📝 **AI Blog Planning & Writing** powered by OpenAI
- 🇮🇳 Focus: Travel & niche blogging (extensible to any domain)
- 🛠️ Easy to plug into existing tools or build upon

---

## 🗂 Folder Structure

```
langgraph-bloggenius/
├── my_agent/
│   ├── __init__.py
│   ├── agent.py           # LangGraph construction and flow
│   ├── state.py           # Shared state class
│   └── nodes/
│       ├── __init__.py
│       ├── topic_searcher.py  # Tavily-powered search node
│       ├── planner.py         # Blog outline generator
│       └── writer.py          # (Optional) Full blog writer
├── .env                  # API keys (not committed)
├── requirements.txt
├── langgraph.json        # LangGraph config
└── README.md             # This file!
```

---

## ⚙️ Setup

### 1. Clone and Install

```bash
git clone https://github.com/your-username/langgraph-bloggenius.git
cd langgraph-bloggenius

# Create virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### 2. Configure `.env`

Create a `.env` file with your API keys:

```env
OPENAI_API_KEY=your-openai-key
TAVILY_API_KEY=your-tavily-key
```

### 3. Run It

```bash
python my_agent/agent.py
```
