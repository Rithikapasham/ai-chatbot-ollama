# 🤖 AI Chatbot using Streamlit and Ollama

A simple AI-powered chatbot built using **Python, Streamlit, and Ollama**. This chatbot uses the **Gemma 3:1B** language model to generate responses and provides an interactive chat interface with conversation history.

## 📌 Project Overview

The AI Chatbot is a locally running conversational application that allows users to interact with an AI model in real time.

It uses Streamlit to create a web-based user interface and Ollama to run the Gemma 3:1B model locally.

## ✨ Features

* 🤖 AI-powered responses using Gemma 3:1B.
* 💬 Interactive chat interface.
* 🧠 Maintains conversation history during a session.
* ⚡ Fast local response generation, depending on your hardware.
* 🖥️ Simple and user-friendly interface.
* 🔒 Runs locally using Ollama.
* ⏳ Loading indicator while generating responses.
* ⚠️ Basic error handling.

## 🛠️ Technologies Used

| Technology | Purpose                   |
| ---------- | ------------------------- |
| Python     | Main programming language |
| Streamlit  | Web application interface |
| Ollama     | Runs the AI model locally |
| Gemma 3:1B | Language model            |

## 📂 Project Structure

```text
AI-Chatbot/
│
├── app.py
├── README.md
└── requirements.txt
```

## ⚙️ Installation and Setup

### 1. Install Python

Install Python 3.10 or later from:

https://www.python.org/downloads/

Verify the installation:

```bash
python --version
```

### 2. Install Ollama

Download and install Ollama from:

https://ollama.com/download

Verify the installation:

```bash
ollama --version
```

### 3. Download the Gemma Model

Open your terminal and run:

```bash
ollama pull gemma3:1b
```

### 4. Create a Virtual Environment

Navigate to your project folder:

```bash
python -m venv venv
```

Activate it on Windows Command Prompt:

```cmd
venv\Scripts\activate.bat
```

For Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks script execution, use Command Prompt or configure your environment according to your system's security settings.

### 5. Install Dependencies

Create a `requirements.txt` file containing:

```text
streamlit
ollama
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

### 6. Run the Application

Make sure Ollama is running, then execute:

```bash
streamlit run app.py
```

The application will open in your browser at:

```text
http://localhost:8501
```

## 💻 How It Works

1. The user enters a message in the Streamlit chat input.
2. The message is stored in Streamlit session state.
3. The chat history is sent to the Ollama model.
4. Gemma 3:1B processes the conversation and generates a response.
5. The chatbot displays the generated response.
6. The conversation is stored for subsequent interactions during the session.

## 🖼️ Application Interface

The chatbot interface includes:

* A title and description.
* A chat input box.
* Separate message bubbles for users and the AI assistant.
* A loading indicator while the AI is generating a response.

## 🚀 Future Enhancements

* 📄 Integrate RAG to answer questions from PDF documents.
* 🎤 Add voice input and speech output.
* 💾 Save chat history between sessions.
* 🌐 Add multilingual support.
* 🎨 Improve the user interface with custom styling.
* 🔍 Add document search and retrieval capabilities.
* 🧠 Support multiple AI models.

## 🐛 Troubleshooting

**Error: ModuleNotFoundError**

Install the missing package:

```bash
pip install streamlit ollama
```

**Error: Ollama connection refused**

Make sure Ollama is running and available locally. You can test it with:

```bash
ollama run gemma3:1b
```

**Error: Model not found**

Download the model:

```bash
ollama pull gemma3:1b
```

**Error: Streamlit command not found**

Run Streamlit through Python:

```bash
python -m streamlit run app.py
```

## 👩‍💻 Author

**P. Rithika**

B.Tech – Computer Science and Engineering

## 📜 License

This project is intended for educational and learning purposes. You may modify and extend it for your own use.
