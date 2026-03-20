# 🤖 AI Auto Project Generator (Agentic AI)

An AI-powered tool that generates complete academic project blueprints for MCA / Engineering students. Powered by **local LLMs** via Ollama — **no paid APIs required**.

Enter your domain, skill level, preferred technologies, and complexity, and the AI agents will produce a structured blueprint covering:

1. Project Title  
2. Problem Statement  
3. Why This Project Is Useful  
4. Real-World Applications  
5. Technology Stack  
6. Dataset Suggestions  
7. System Architecture  
8. Step-by-Step Implementation  
9. Folder Structure  
10. Future Enhancements  
11. Resume Description  

---

## 📁 Project Structure

```
project_generator/
├── app.py              # Streamlit UI
├── agent.py            # Agentic LLM pipeline (Planner → Generator → Parser)
├── generator.py        # Prompt templates & output parsing
├── styles.css          # Custom CSS for modern UI
├── requirements.txt    # Python dependencies
└── README.md           # This file
```

---

## 🚀 Installation & Setup

### 1. Prerequisites

| Tool | Version | Install |
|------|---------|---------|
| Python | 3.10+ | [python.org](https://python.org) |
| Ollama | latest | [ollama.com](https://ollama.com) |

### 2. Install Ollama & Pull a Model

```bash
# Install Ollama (follow instructions at https://ollama.com)
# Then pull a model:
ollama pull llama3
# (or)
ollama pull mistral
```

### 3. Start Ollama

```bash
ollama serve
```

> Keep this terminal open — the app needs Ollama running in the background.

### 4. Clone & Install Dependencies

```bash
cd project_generator
pip install -r requirements.txt
```

### 5. Run the App

```bash
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`.

---

## 🎨 Features

- **Agentic AI Pipeline** — Planner Agent → Generator Agent → Output Formatter
- **Beautiful Modern UI** — Glassmorphic cards, gradient background, smooth animations
- **PDF Export** — Download your project blueprint as a PDF
- **Copy Buttons** — Easily copy individual sections
- **Example Prompts** — One-click example configurations for quick demos
- **100 % Local** — No data leaves your machine. No API keys needed.

---

## ☁️ Deployment (Streamlit Community Cloud)

> **Note:** Cloud deployment requires an Ollama-compatible endpoint. For a fully local experience, run on your own machine.

1. Push this folder to a **public GitHub repository**.
2. Go to [share.streamlit.io](https://share.streamlit.io).
3. Click **New app** → select your repo, branch, and `app.py`.
4. Add any required secrets/environment variables for your Ollama endpoint.
5. Click **Deploy**.

For local-only usage, simply run `streamlit run app.py`.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Python 3.10+ |
| UI Framework | Streamlit |
| LLM Runtime | Ollama (local) |
| LLM Models | Llama 3 / Mistral |
| Agent Framework | LangChain |
| PDF Export | fpdf2 |

---

## 📄 License

This project is open-source and free to use for academic purposes.
