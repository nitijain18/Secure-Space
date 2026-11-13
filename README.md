<div align="center">

# 🛡️ SecureSpace

**An autonomous AI security analyst that investigates threats and explains its findings**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LLMs](https://img.shields.io/badge/LLMs-RAG-2563eb?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In_Progress-orange?style=for-the-badge)

</div>

---

## 📖 About

SecureSpace is an AI-powered security analyst that investigates security logs, suspicious emails, URLs and incident data. It combines **Retrieval-Augmented Generation (RAG)** with **agentic workflows** so it can gather evidence, reason about a threat and give clear, explainable recommendations instead of a bare verdict.

> 🚧 This project is under active development. The features below show the current goals and progress.

## ✨ Features

- **Threat analysis** of security logs, suspicious emails, URLs and incident reports
- **IOC extraction**: pulls out indicators of compromise such as IPs, domains, URLs and file hashes
- **Risk scoring** to rank how dangerous an item is
- **Explainable recommendations** that say why something was flagged and what to do next
- **RAG pipeline** that grounds answers in a security knowledge base
- **Agentic workflow** where the analyst chooses which tools and checks to run

> Mark each feature as done or planned so the README matches your code (see Roadmap below).

## 🧠 How it works

```
Input (log / email / URL / incident)
        │
        ▼
  IOC extraction  ──►  Retrieval from knowledge base (RAG)
        │                         │
        └──────────►  LLM agent reasons with tools
                                  │
                                  ▼
              Risk score + explanation + recommended actions
```

## 🛠️ Tech stack

| Area | Technology |
|---|---|
| Language | Python |
| LLM framework | LangChain |
| AI techniques | LLMs, RAG, Agentic AI, Embeddings, Prompt Engineering |
| Vector store | *(add yours, e.g. FAISS or ChromaDB)* |
| Tools | Git, GitHub, Jupyter Notebook, VS Code |

## 📂 Project structure

```
SecureSpace/
├── app/            # agent, tools and RAG pipeline
├── data/           # sample logs and knowledge base documents
├── notebooks/      # experiments
├── requirements.txt
└── README.md
```

> Rename these to match your real folders.

## 🚀 Getting started

### Prerequisites
- Python 3.10+
- An API key for your LLM provider

### 1. Clone the repo
```bash
git clone https://github.com/nitijain18/SecureSpace.git
cd SecureSpace
```

### 2. Create a virtual environment and install dependencies
```bash
python -m venv venv
venv\Scripts\activate        # on Mac/Linux: source venv/bin/activate
pip install -r requirements.txt
```

### 3. Add your API key
Create a `.env` file in the project root:
```
LLM_API_KEY=your_key_here
```
Never commit this file. Make sure `.env` is listed in your `.gitignore`.

### 4. Run
```bash
python main.py
```

## 🗺️ Roadmap

- [x] Project setup and architecture
- [ ] IOC extraction
- [ ] RAG over security knowledge base
- [ ] Agentic investigation workflow
- [ ] Risk scoring
- [ ] Explainable recommendations
- [ ] Simple web interface
- [ ] Evaluation on sample incidents

> Tick the boxes as you finish each item.

## ⚠️ Disclaimer

SecureSpace is a learning and research project. Its output should be reviewed by a human before any security action is taken.

## 👩‍💻 Author

**Niti Jain**
[LinkedIn](https://linkedin.com/in/nitijain18) · [GitHub](https://github.com/nitijain18) · jainniti1807@gmail.com
