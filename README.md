# AI Chatbot for Mental Health Screening (WhatsApp)

An AI-powered mental health support chatbot for university students, built with n8n workflow automation, WhatsApp Cloud API, OpenAI LLM, and Firebase Firestore. The chatbot provides empathetic conversations, structured mental health screening, session memory, and crisis detection.

## ✨ Features

- 🤖 AI-powered empathetic chatbot ("Lumi") for university students.
- 💬 Real-time conversations through WhatsApp Cloud API.
- 🧠 Multi-stage mental health screening workflow (Stage 0–4).
- 📝 Conversation memory with Firebase Firestore.
- 🚨 Crisis detection with emergency support guidance.
- 🔄 Session versioning and `/newchat` reset.
- 🌐 Automatic English and Chinese language detection.

---
## 🏗️ System Architecture

WhatsApp User
      │
      ▼
WhatsApp Cloud API
      │
      ▼
n8n Webhook
      │
      ▼
AI Agent (OpenAI)
      │
      ├── Memory
      ├── Prompt Engineering
      └── Crisis Detection
      │
      ▼
Firebase Firestore

---

## 📂 Project Structure
AI-Mental-Health-Chatbot/
│
├── README.md
├── workflow.json
├── poster.png
└── demo.mp4

---

## 🛠️ Technology Stack

| Category | Technology |
|----------|------------|
| Workflow Automation | n8n |
| LLM | OpenAI GPT |
| Messaging | WhatsApp Cloud API |
| Database | Firebase Firestore |
| Programming | JavaScript (n8n Expressions) |
| AI Techniques | Prompt Engineering, Conversation Memory |

---

## 📺 Demo & Presentation
You can check the full project demonstration and poster via the link below:
- 👉 [View Demo Video & Poster on Google Drive](https://drive.google.com/file/d/1Bb_RZPS7JSowgJomtBd3YhPfaM0yzVpy/view?usp=sharing)
![Poster](poster.png)
---

## ⚙️ Setup & Installation
1. Import `My workflow.json` into your **n8n** instance.
2. Configure the required environment variables in n8n:
   - `WHATSAPP_TOKEN`
   - `WHATSAPP_PHONE_ID`
   - `ADMIN_PHONE`
   - `FIREBASE_PROJECT_ID`
3. Set up your Meta WhatsApp Webhook pointing to your n8n Webhook node.

---

## 🚀 Future Improvements

- RAG-based knowledge retrieval
- Voice message support
- Emotion trend visualization dashboard
- Multi-language support
- Therapist dashboard
