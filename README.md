
---

# 💬 Ollama AI Prompt Engineering Chatbot

An interactive web-based chatbot built using **React (frontend)** and **Node.js with Express (backend)** that connects to a **local or cloud Ollama model** through the LangChain `ChatOllama` interface.
This chatbot allows users to experiment with **custom system prompts (templates)** and chat dynamically with an AI specialized.

---

## 🚀 Features

* 🧠 **AI-Powered Responses** — Uses Ollama models via LangChain for intelligent, context-aware chat.
* 🧩 **Custom Prompt Templates** — Users can define their own AI behavior dynamically.
* 💬 **Interactive Chat Interface** — Clean and responsive UI built with React.
* 🔄 **Auto-Scroll to Latest Message** — Chat view automatically focuses on the newest messages.
* ⚙️ **Full Express API Backend** — Simple REST endpoint for handling AI requests.
* 🌐 **CORS-Enabled Communication** — Frontend and backend can run independently during development.

---

## 🏗️ Project Structure

```
project-root/
│
├── backend/
│   ├── server.js              # Express + LangChain + Ollama logic
│   └── .env                   # Environment variables (API keys, etc.)
│
├── frontend/
│   ├── src/
│   │   ├── App.js             # Main React component
│   │   ├── Chatbot.css        # Styling for chat interface
│   │   └── index.js           # React entry point
│   └── package.json           # Frontend dependencies
│
└── README.md
```

---

## ⚡ Setup and Run

### 1. Backend (Node.js + Express)

1. Navigate to the backend folder
2. Install dependencies:

   ```bash
   npm install
   ```
3. Start the server:

   ```bash
   node server.js
   ```
4. The API will run on `http://localhost:5000/api/chat`

### 2. Frontend (React)

1. Navigate to the frontend folder
2. Install dependencies:

   ```bash
   npm install
   ```
3. Start the React development server:

   ```bash
   npm start
   ```
4. Access the app at `http://localhost:3000`

---

## 🧩 How It Works

* The frontend collects user input and an optional **prompt template**.
* On send, it makes a POST request to `/api/chat` with the message and template.
* The backend uses **LangChain’s ChatOllama** to generate a response from the selected model.
* The chat window displays both user and AI messages with smooth scrolling.

---

## 🖌️ UI Overview

* **System Prompt Area:** Customize how the AI behaves (e.g., tone, domain, language).
* **Chat Area:** Displays conversation history with the AI.
* **Input Field:** Type your questions and send them instantly.
* **Auto Scroll:** The chat view always focuses on the latest response.

---

## 🧠 Technologies Used

* **Frontend:** React, CSS
* **Backend:** Node.js, Express, LangChain
* **Model:** Ollama (local or cloud-hosted)
* **Environment Management:** dotenv
* **Cross-Origin Support:** CORS

---

## 📦 Requirements

* Node.js 18+
* Ollama installed locally *(or access to a remote Ollama model)*
* Internet access (for cloud models)

---

## 🔒 Environment Variables

Create a `.env` file in your backend directory:

```
OLLAMA_URL=http://localhost:11434
```



---

## 🧭 Future Improvements

* Add **conversation history persistence** (local storage or database)
* Support **multiple AI models** and dynamic selection
* Integrate **Markdown rendering** for AI responses
* Enable **speech input/output**

---

## 🧑‍💻 Author

**Budi Setiawan**
Passionate about AI, and application development.


---

