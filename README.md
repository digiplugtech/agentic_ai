# Agentic AI Application

A robust, multi-agent AI application built with **FastAPI**, **LangChain**, and **LangGraph**. This project leverages multiple LLM providers (OpenAI, Gemini, Anthropic) and orchestrates them into autonomous workflows using graph-based agentic logic.

## 🚀 Features

-   **Multi-LLM Support:** Seamlessly switch between OpenAI (GPT-4), Google Gemini, and Anthropic Claude.
-   **Agentic Workflows:** Complex decision-making loops implemented with `LangGraph`.
-   **API First:** Fully exposed via `FastAPI` and `LangServe` for easy integration.
-   **Extensible:** Modular structure for adding new agents, tools, and vector stores.

## 🛠️ Tech Stack

-   **Framework:** FastAPI, Uvicorn
-   **AI Orchestration:** LangChain, LangGraph
-   **Serving:** LangServe
-   **Dependency Management:** Poetry

## 📂 Project Structure

agentic_ai/
├── app/
│   ├── main.py              # Application entry point
│   ├── core/                # Config & LLM Factory
│   ├── agents/              # Agent definitions
│   └── graphs/              # LangGraph workflows
├── pyproject.toml           # Dependencies
└── requirements.txt         # Exported dependencies## ⚡ Getting Started

### Prerequisites

-   Python 3.10+
-   [Poetry](https://python-poetry.org/) (recommended) or pip

### Installation

1.  **Clone the repository:**
    
    git clone https://github.com/your-username/agentic-ai.git
    cd agentic-ai
    2.  **Install dependencies:**
    Using Poetry:
    poetry install
        Or using pip:
    pip install -r requirements.txt
    3.  **Configure Environment:**
    Create a `.env` file in the root directory and add your API keys:
    OPENAI_API_KEY=sk-...
    ANTHROPIC_API_KEY=sk-ant-...
    GOOGLE_API_KEY=AIza...
    LANGCHAIN_TRACING_V2=true
    LANGCHAIN_API_KEY=ls-...
    ### Running the App

Start the development server:

poetry run uvicorn app.main:app --reloadThe API will be available at:
-   **Docs:** `http://localhost:8000/docs`
-   **LangServe Playground:** `http://localhost:8000/agent/playground`

## 🤝 Contributing

1.  Fork the repo
2.  Create your feature branch (`git checkout -b feature/amazing-agent`)
3.  Commit your changes (`git commit -m 'Add some amazing agent'`)
4.  Push to the branch (`git push origin feature/amazing-agent`)
5.  Open a Pull Request
