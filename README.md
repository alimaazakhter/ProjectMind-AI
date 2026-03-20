# 🚀 ProjectMind AI

### 🤖 AI Auto Project Generator (Agentic AI)

An AI-powered tool that generates complete academic project blueprints for MCA / Engineering students.

Originally designed to run fully on **local LLMs using Ollama (100% offline, no paid APIs)**, the system was later enhanced with **Google Gemini API support** to enable fast and scalable cloud deployment.

---

## 🧠 How It Works

This project follows an **Agentic AI pipeline**:

* 🧩 **Planner Agent** → Breaks down user input
* ⚙️ **Generator Agent** → Creates structured content
* 📝 **Formatter/Parser** → Cleans and organizes output

---

## ⚡ Dual Mode Support (Key Highlight)

This project supports **two modes of operation**:

### 🟢 1. Local Mode (Ollama)

* Runs fully on your system
* No internet required
* No API key needed
* Uses models like Llama3 / Mistral

### ☁️ 2. Cloud Mode (Gemini API)

* Fast responses
* No local setup required
* Easily deployable on Streamlit Cloud
* Uses Google Gemini models

> 🔥 This hybrid design ensures both **privacy (local AI)** and **scalability (cloud AI)**.

---

## ✨ Features

* 🧠 Generate full project blueprints
* ⚡ AI-powered structured output
* 📊 Tech stack & dataset suggestions
* 📝 Viva questions generator
* 📅 Project timeline generation
* 💻 Starter code suggestions
* 📄 Export to PDF, DOCX, PPT
* 🎯 Clean modern UI

---

## 📁 Project Structure

```
project_generator/
├── app.py
├── agent.py
├── generator.py
├── styles.css
├── requirements.txt
└── README.md
```

---

## 🚀 Installation & Setup (Local - Ollama Mode)

### 1. Install Ollama

```bash
ollama pull llama3
# or
ollama pull mistral
```

### 2. Start Ollama

```bash
ollama serve
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run App

```bash
streamlit run app.py
```

---

## ☁️ Cloud Setup (Gemini Mode)

1. Get a free API key from Google AI Studio
2. Add in Streamlit Secrets:

```
GOOGLE_API_KEY="your_api_key"
```

3. Deploy on Streamlit Cloud

---

## 🛠️ Tech Stack

* Python
* Streamlit
* LangChain
* Ollama (Local LLMs)
* Google Gemini API
* FPDF / python-docx / python-pptx

---

## 💡 Why Both Ollama and Gemini?

* Ollama → **Privacy + Offline capability**
* Gemini → **Speed + Deployment support**

This combination makes the system flexible for both **local development** and **real-world usage**.

---

## 🌐 Deployment

Deployed on Streamlit Community Cloud using Gemini API for cloud inference.

---

## 👨‍💻 Author

Developed by **Alimaaz Akhter**

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
