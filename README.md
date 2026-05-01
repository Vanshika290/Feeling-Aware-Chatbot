# 🎤 Feeling-Aware Chatbot

### A Voice-First, Emotionally Intelligent AI for Real Conversations

> *Not just a chatbot. A system that listens, understands, and responds like a human should.*

---

## 🚀 Overview

**Feeling-Aware Chatbot** is a real-time, multilingual, voice-first AI system designed to provide **empathetic conversational support**. Unlike traditional chatbots that rely on typed input and generic responses, this system enables users to **speak freely** and receive responses that are **emotion-aware, context-sensitive, and human-like**.

The project integrates **speech processing, emotion detection, and large language models** into a seamless pipeline that transforms raw voice input into meaningful, supportive dialogue.

---

## 💡 Why This Project Matters

In a world where conversations are increasingly digital, most systems still fail at one thing: **understanding human emotion**.

This project addresses that gap by:

* Interpreting not just *what users say*, but *how they say it*
* Delivering responses that feel natural, calm, and supportive
* Creating a safe space for users to express thoughts without friction (no typing)

---

## 🌟 Key Highlights

### 🎙️ Voice-First Experience

* Fully microphone-based interaction (zero typing)
* Real-time audio capture and processing
* Natural speech responses using high-quality TTS

### 🌍 Multilingual Intelligence

* Supports: English, Hindi, Marathi, Bengali, Kannada
* Automatic language detection via Whisper
* Contextually accurate responses in the same language

### 🧠 Dual-Layer Emotion Detection (Core Innovation)

* **Text Emotion Analysis** → sentiment + intent
* **Voice Emotion Analysis** → pitch, energy, tempo using Librosa
* Combined to infer user's true emotional state

> Example: A user saying “I’m fine” in a low-energy tone is detected as *distressed*, not neutral.

### 💬 Empathetic Response Engine

* Custom-designed system prompt for emotional intelligence
* Avoids robotic replies and clichés
* Uses:

  * Emotion acknowledgment
  * Validation
  * Gentle follow-up questions

### 🚨 Safety & Crisis Handling

* Detects distress signals (self-harm, hopelessness)
* Responds with calm, supportive messaging
* Provides India-specific helpline suggestions
* Designed responsibly (not a replacement for therapy)

### 📊 Mood Awareness (Extensible)

* Tracks session-level emotions
* Enables future features like mood trends and insights

---

## 🏗️ System Architecture

```id="arch01"
User Voice 🎤
   ↓
WebSocket Streaming
   ↓
Speech-to-Text (Whisper)
   ↓
Emotion Detection (Text + Audio)
   ↓
Crisis Detection Layer ⚠️
   ↓
LLM (Empathetic Response Generation)
   ↓
Text-to-Speech (Natural Voice)
   ↓
Frontend Playback 🔊
   ↓
Emotion Data Storage 📊
```

---

## 🧩 Project Structure

```id="struct01"
feeling-aware-chatbot/
├── backend/
│   ├── main.py
│   ├── services/
│   │   ├── stt_service.py
│   │   ├── llm_service.py
│   │   ├── tts_service.py
│   │   └── emotion_service.py
│   ├── utils/
│   │   └── audio_utils.py
│   ├── database.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── MicButton.jsx
│   │   │   ├── Waveform.jsx
│   │   │   └── EmotionDisplay.jsx
│   │   ├── App.jsx
│   │   └── index.css
│   ├── package.json
│   └── vite.config.js
└── .env
```

---

## ⚙️ Tech Stack

### Frontend

* React (Vite)
* Web Audio API
* WebSockets (real-time communication)

### Backend

* FastAPI (Python)
* Async WebSocket handling
* SQLite (prototype database)

### AI & Audio Pipeline

* **Speech-to-Text**: OpenAI Whisper
* **LLM**: GPT-4o (low-latency, high-context understanding)
* **Text-to-Speech**: OpenAI TTS / ElevenLabs
* **Emotion Detection**:

  * Text: LLM-based sentiment analysis
  * Audio: Librosa (pitch, energy, tempo extraction)

---

## 🔄 Execution Flow

```id="flow01"
🎤 User speaks
   ↓
📝 Speech converted to text
   ↓
🧠 Emotion inferred (text + voice)
   ↓
⚠️ Safety check triggered if needed
   ↓
💬 AI generates empathetic response
   ↓
🔊 Response converted to speech
   ↓
🎧 User hears response
```

---

## 🚀 Getting Started

### Clone Repository

```bash id="cmd01"
git clone https://github.com/Vanshika290/Feeling-Aware-Chatbot.git
cd feeling-aware-chatbot
```

### Backend Setup

```bash id="cmd02"
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Frontend Setup

```bash id="cmd03"
cd frontend
npm install
npm run dev
```

### Environment Variables

```id="env01"
OPENAI_API_KEY=your_api_key
ELEVENLABS_API_KEY=your_api_key
```

---

## 🧪 Validation Strategy

* Multilingual voice testing (EN + HI)
* Emotion variance testing (tone-based)
* Safety trigger testing (distress scenarios)
* Latency and real-time response validation

---

## ⚠️ Disclaimer

This system is intended for **supportive conversation purposes only**.
It is **not a medical or therapeutic tool**.

---

## 🔮 Future Enhancements

* Real-time streaming transcription (partial STT)
* Advanced emotion recognition models (deep learning-based SER)
* Persistent memory & personalization
* Mobile app deployment
* Background calming audio integration

---

## 🏆 What Makes This Stand Out

* True **voice-first interaction** (no fallback to typing)
* **Emotion-aware AI**, not just intent-based
* **Multilingual conversational intelligence**
* Combines **AI, audio processing, and human-centered design**
* Built with **real-world usability and responsibility in mind**

---

## 👩‍💻 Author

**Vanshika Saxena**
B.Tech | AI/ML Enthusiast | Aspiring Software Engineer

---

## ⭐ If this project resonates with you, consider starring the repository!
