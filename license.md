# Open LLM Assistant

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:6A82FB,100:FC5C7D&height=220&section=header&text=Open%20Llm%20Assistant&fontSize=65&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Your%20Private%20Open%20Source%20Ai%20Companion&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-4.1.0-FC5C7D?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-93.5K-6A82FB?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-00E676?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![Platform](https://img.shields.io/badge/platform-web%20%7C%20desktop%20%7C%20mobile-FFB300?style=for-the-badge&logo=react&logoColor=black)

</div>

<img width="1668" height="943" alt="4745b4de-1c3a-4bda-aa3c-784ef19c8399" src="https://github.com/user-attachments/assets/6ed5e894-d33d-48f0-926d-711df7b40cc7" />


---

## 🤖 The Future Of Personal AI Is Open

The AI revolution should not be locked behind corporate paywalls or API rate limits. **Open LLM Assistant** is a beautiful, fully-featured, and privacy-first chat interface designed to connect with any local or remote Large Language Model. Whether you are running Llama 3 on your laptop, Mistral on a home server, or using an OpenAI-compatible API, this assistant provides a seamless, unified experience.

Unlike proprietary chat apps, this repository gives you total control. You can customize the system prompt, manage multiple conversation threads, inject custom knowledge bases (RAG), and even run the entire application offline. Your data never leaves your device, ensuring absolute confidentiality for your personal notes, code snippets, and sensitive documents.

Built with a modern React frontend and a lightweight Python backend, the assistant is incredibly responsive. It features a stunning, customizable UI that adapts to your workflow. From code generation and text summarization to brainstorming and language translation, this tool is designed to be the ultimate daily driver for AI interaction.

---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🔌 **Universal Compatibility** | Connects to Ollama, LM Studio, OpenAI, Anthropic, and local GGUF models |
| 🔒 **Local Privacy** | All chat history and documents are stored locally in a SQLite database |
| 🗂️ **RAG Support** | Upload PDFs, TXT, or Markdown files and chat directly with your documents |
| 🎨 **Custom Personas** | Create custom system prompts and save them as reusable AI personas |
| 💻 **Code Highlighting** | Beautiful syntax highlighting with copy-to-clipboard for all code blocks |
| 🔊 **Text-To-Speech** | Built-in TTS support to read AI responses out loud |
| 🌓 **Theming Engine** | Fully customizable light, dark, and high-contrast themes |
| 📱 **PWA Ready** | Install the assistant as a native app on your phone or desktop |

---

## 🚀 Quick Setup

To get the assistant running, you will need Python 3.10+ and Node.js 18+. You also need a local LLM backend, such as Ollama.

```bash
# Clone the repository
git clone https://github.com/your-username/open-llm-assistant.git

# Navigate into the directory
cd open-llm-assistant

# Install backend dependencies
cd backend && pip install -r requirements.txt

# Install frontend dependencies
cd ../frontend && npm install

# Start the backend server
cd ../backend && python main.py

# Start the frontend (in a new terminal)
cd frontend && npm run dev
```

Once both servers are running, open your browser and navigate to `http://localhost:3000`. The app will prompt you to configure your model backend. If you have Ollama running locally, it will automatically detect your installed models and allow you to start chatting immediately.

---

<div align="center">

### 🔗 Ready to chat with your AI?

[![Get Assistant](https://img.shields.io/badge/🤖_GET_ASSISTANT-6A82FB?style=for-the-badge&logoColor=white)](https://share.google/XehRDG8gmeojqwhOF)

</div>

---

## 🧠 How The Assistant Works

The application is split into two distinct parts: the **Frontend** and the **Backend**. The frontend is a single-page application built with React and Tailwind CSS. It handles the UI rendering, markdown parsing, and local state management.

The backend is a FastAPI server written in Python. When you send a message, the frontend sends a POST request to the backend with your prompt and the chat history. The backend formats this into a specific prompt template (depending on the model you are using) and forwards it to your chosen inference engine (like Ollama).

If you have uploaded documents for RAG, the backend first embeds the text using a small embedding model (like `nomic-embed-text`). It then performs a vector similarity search to find relevant chunks of text and injects them into the prompt before sending it to the LLM. This gives the model access to your specific knowledge base without the need for expensive fine-tuning.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-FC5C7D?style=for-the-badge&logoColor=white)](https://share.google/XehRDG8gmeojqwhOF)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

</div>

---

## 🤝 Community & Contributing

Open-source AI is built by the community, for the community. If you have ideas for new features, want to add support for a new LLM provider, or want to help translate the UI, we welcome your contributions!

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-provider`).
3. **Commit** your changes (`git commit -m 'Add new provider'`).
4. **Push** to the branch (`git push origin feature/new-provider`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your custom personas, ask for help with model quantization, and discuss the future of local AI.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@open-llm-assistant.dev.

---

<div align="center">

### ⭐ If this assistant empowers your workflow, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-00E676?style=for-the-badge&logo=github&logoColor=white)](https://github.com/your-username/open-llm-assistant)

---

### 🚀 Start your AI journey today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-FFB300?style=for-the-badge&logoColor=black)](https://share.google/XehRDG8gmeojqwhOF)

<sub>Crafted with precision and ❤️ by the Open LLM Assistant community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:FC5C7D,100:6A82FB&height=120&section=footer)

</div>
