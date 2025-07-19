# 🧠 Friday — Your Personal AI Assistant

**Friday** is a Python-based personal AI assistant inspired by *JARVIS* from Iron Man — developed by **Syed Ahmad Alisha**. It uses **LiveKit**, a real-time communication platform, along with cutting-edge plugins to perform a range of intelligent tasks including voice interactions, web-based chat, web search, email automation, weather reporting, and even camera vision.

> 🎩 “Greetings. I am Friday, the personal assistant engineered by Syed Ahmad Alisha. How may I assist you today?”

---

## 🚀 Features

- 🔍 **Web Search** — Powered by DuckDuckGo to fetch quick, privacy-focused results  
- 🌤️ **Weather Report** — Get real-time weather updates by city  
- 📨 **Send Emails** — Compose and send emails using Gmail SMTP and app passwords  
- 📷 **Camera Vision** — Uses your webcam to see and analyze input *(via Web UI)*  
- 🗣️ **Voice Assistant** — Speech recognition and voice-based replies  
- 💬 **Chat UI** — Web-based real-time chat interface to talk to Friday  
- 🎙️ **Noise Cancellation** — Uses LiveKit plugins to enhance voice clarity  
- 🧠 **LLM Integration** — Uses OpenAI for natural conversations  
- 📡 **LiveKit Cloud** — Real-time session handling and voice room integration  

---

## 🧰 Tech Stack

- **Python 3.10+**
- **LiveKit Agents & Plugins**
- **OpenAI GPT-4o**
- **Silero VAD**
- **Deepgram STT**
- **Google / ElevenLabs TTS**
- **LangChain Tools**
- **DuckDuckGo Search**
- **Flask / Web Frontend**

---

## 📦 Installation Guide

### 1. Clone this repository

```bash
git clone https://github.com/your-username/live_kit_jarvis
cd live_kit_jarvis
```

---

### 2. Create a virtual environment

```bash
python -m venv venv
```

---

### 3. Activate the environment

#### On Windows:
```bash
.\venv\Scripts\activate
```

#### On macOS/Linux:
```bash
source venv/bin/activate
```

---

### 4. Install required packages

```bash
pip install -r requirements.txt
```

---

## 🔐 Environment Setup

Create a `.env` file in the root of the project and add your credentials:

```env
LIVEKIT_URL=your_livekit_url
LIVEKIT_API_KEY=your_api_key
LIVEKIT_API_SECRET=your_api_secret

OPENAI_API_KEY=your_openai_api_key

GMAIL_USER=your_email@gmail.com
GMAIL_APP_PASSWORD=your_gmail_app_password
```

> 💡 To generate a Gmail App Password:  
> Go to [Google App Passwords](https://myaccount.google.com/apppasswords) and create a new one for "Mail".

---

## ✅ Running the Agent

### Voice Agent Mode:

```bash
python agent.py console
```

### Web Assistant Mode:

```bash
python agent.py web
```

### Download Required Files (if supported by your setup):

```bash
python agent.py download-files
```

> This may trigger downloads for language models, TTS engines, or VAD components.

---

## 📁 Project Structure

```
live_kit_jarvis/
├── agent.py                 # Main agent script
├── tools.py                # Tool functions: weather, email, search
├── prompts.py              #contains Agent and Session Instructions 
├── requirements.txt        # Dependencies                    
├── .env                    # API keys and secrets
└── README.md
```

---

## 🤖 Personality & Behavior

Friday is designed with a unique persona:

- Speaks like a classy butler
- Sarcastic tone with formal elegance
- Responds in **only one sentence**
- Acknowledges tasks like:
  - “Will do, Sir.”
  - “Roger Boss.”
  - “Check!”

---

## 🧠 Credits & Inspiration

- [LiveKit](https://livekit.io)
- [OpenAI](https://openai.com)
- [DuckDuckGo Search](https://duckduckgo.com)
- [LangChain](https://www.langchain.com/)
- Inspired by *Tony Stark’s J.A.R.V.I.S.*

---

## 📞 Need Help?

If you run into issues or want to contribute, feel free to reach out or create a GitHub issue.

---

## ⭐ Star this Repo

If you like this project, consider starring it! It helps others discover it too.

---
