<div align="center" style="text-align: center;">
    
# 🧠 PrivateChatGPT: Secure In-House Conversational AI Using DeepSeek

[![Go to PrivateChatGPT App](https://github.com/user-attachments/assets/be31d679-0e1b-46ab-8b61-7ab3cd28f5a4)](https://privatechatgpt.netlify.app/)

A fully offline, locally hosted AI chatbot powered by [DeepSeek](https://github.com/deepseek-ai/DeepSeek-V2) or similar LLMs. Designed for organizations that want the benefits of ChatGPT **without the privacy risks** of sending internal data to external servers.
---
![image](https://github.com/user-attachments/assets/73bbd867-627f-4f9b-aeb7-15528d0ffcb7)


---

## 🔒 Why Use a Local ChatGPT?

Many businesses are interested in using conversational AI, but face strict data privacy or compliance rules. This project shows how companies can:

- Run their **own in-house ChatGPT clone**
- Avoid leaking proprietary information to external APIs
- Deploy it across multiple office computers using simple IT scripts


---

## 🚀 Features

- 💬 **Fully Offline Chat Interface**
- 🔐 **Zero API Calls, Full Privacy**
- 🧑‍💻 **Deployable Across Office Machines**
- 📂 **Internal Document Integration (RAG)**
- ⚙️ **Admin Setup Scripts**
- 🖥️ **Runs on Windows or Linux, with or without GPU**

---

## 🧠 Tech Stack

| Purpose             | Tool/Framework                          |
|---------------------|------------------------------------------|
| LLM                 | [DeepSeek-V2](https://github.com/deepseek-ai/DeepSeek-V2) / LLaMA.cpp |
| Backend Inference   | `llama.cpp`, `vllm`, or `text-generation-webui` |
| Chat UI             | `Gradio` or `Streamlit` |
| Document Support    | `llama-index`, `Haystack`, or custom retriever |
| Deployment          | Bash/PowerShell scripts |
| Platform Support    | Windows & Linux (x86 or GPU-enabled) |

---

## 🧩 Use Cases

- Office IT chatbot for employees
- Secure AI assistant for managers and executives
- Internal documentation/Q&A search (PDFs, DOCX, etc.)
- Onboarding bot for new employees
- Replacement for ChatGPT in regulated environments (healthcare, finance, etc.)

---

## 💻 Helpdesk Features

This project includes tools familiar to any IT support or sysadmin role:

- Automated installer for Windows (`.ps1`) or Linux (`.sh`)
- System tray startup options
- Lightweight logging and self-diagnostics
- Easy configuration file in YAML/JSON
- Network folder sync for shared internal documents

---

## 📁 File Structure

```
private-chatgpt/
│
├── README.md                 # Project overview and usage instructions
├── LICENSE                   # License information
├── install/                  # Installation scripts
│   ├── windows_installer.ps1    # Windows installation script
│   └── linux_installer.sh       # Linux installation script
├── chatbot_ui/              # Frontend UI application
│   └── app.py                   # Streamlit or Flask UI for chat
├── backend/                 # Backend logic and RAG pipeline
│   ├── inference_engine.py      # Handles model inference
│   ├── document_loader.py       # Loads and preprocesses documents
│   └── rag_retriever.py         # Retrieves relevant documents for answers
├── config/                  # Configuration files
│   └── settings.yaml            # YAML config for parameters and paths
├── docs/                    # Project documentation
│   └── architecture_diagram.png # System architecture diagram
└── requirements.txt         # Python dependencies
```



---

## 🛠️ Installation

### 🪟 Windows

```powershell
git clone https://github.com/yourusername/private-chatgpt
cd private-chatgpt\install
.\windows_installer.ps1
```

🐧 Linux

    git clone https://github.com/yourusername/private-chatgpt
    cd private-chatgpt/install
    bash linux_installer.sh
💡 Run on startup using Task Scheduler (Windows) or crontab/systemd (Linux)

---

🧪 How It Works

    Loads a local LLM from disk (DeepSeek / LLaMA)

    Accepts chat input via local web UI

    (Optional) Uses RAG to pull context from internal PDFs/docs

    Responds instantly with no internet usage

🗂️ Example Use: Load Internal Docs

Put your documents in:

private-chatgpt/docs_to_index/

The RAG module will automatically index and inject them into the context window during chat.
📸 Screenshots

Add screenshots or a demo GIF here.
📅 Roadmap

Basic offline chat

Windows/Linux deployment

Internal file indexing

Simple speech-to-text (offline)

More polished UI (Electron)

    Multi-language support

📄 License

MIT License
🙋‍♂️ Contact / Hire Me

Want to implement this in your company? Contact me via GitHub or [your email or portfolio link].
🌐 Credits

    DeepSeek AI

    LLaMA.cpp

    Gradio

    LlamaIndex


---

Let me know if you want to auto-generate the initial code and scripts — I can give you a `main.py`, `document_loader.py`, or even a basic `Streamlit`/`Gradio` UI to get started.
