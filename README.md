# 🌐 AI Translator Launchpad

> A multi-tool AI-powered language workstation built as my minor project.
> Four independent tools — one unified platform.

![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![Gemini API](https://img.shields.io/badge/Gemini_API-4285F4?style=flat&logo=google&logoColor=white)

---

## 💡 Why I Built This

As a student I always felt that language should never be a barrier — whether you're reading content from another country, chatting with someone in a different language, or trying to generate professional content in your native tongue.

So I built a platform that brings all of that together in one place — using the power of Gemini 2.5 Flash and Web Speech API.

---

## 🛠️ Features

### 1. 🔤 Real-Time Translator & URL Video Summary
- Translate text by typing or using voice input (Speech-to-Text)
- Auto-detects source language — no manual selection needed
- Paste any YouTube or web URL — AI summarizes and translates the content
- Text-to-Speech output — hear the translation spoken back
- Exponential backoff retry system for reliable API calls

### 2. 💬 Real-Time Translation Chat
- Two users chat simultaneously in different languages
- Each user types in their own language — partner reads in theirs
- Powered by Gemini 2.5 Flash for instant AI translation
- Supports 50+ world languages including all major Indian languages
- Download full chat log as .txt file

### 3. 🎙️ Bilingual Conversation Translator
- Turn-based voice translation between two speakers
- Speaker A speaks → AI translates → Speaker B hears it in their language
- Voice Activity Detection (VAD) — auto-stops on silence
- Start/Stop conversation logging
- Download full conversation log as .txt file

### 4. ✍️ AI Content Generator
- Generate professional articles, emails, and creative content
- Set output language and word count constraint
- Animated typewriter response display
- PDF preview before downloading
- Copy to clipboard in one click
- Supports non-Latin languages (Hindi, Arabic, etc.)

---

## 🧰 Tech Stack

| Technology | Purpose |
|---|---|
| HTML · CSS · JavaScript | Core frontend |
| Tailwind CSS | UI styling |
| Gemini 2.5 Flash | AI translation & content generation |
| Gemini 2.5 Flash (Grounded) | URL & video content analysis with Google Search |
| Web Speech API | Voice input (STT) & voice output (TTS) |
| jsPDF | Client-side PDF generation |
| Lucide Icons | UI icons |

---

## 📁 Project Structure

```
AI-Translator-Launchpad/
│
├── index.html                  # Main dashboard
├── url_video_summary.html      # Real-Time Translator & URL Summary
├── realtimechat.html           # Translation Chat
├── biliangual_translator.html  # Bilingual Voice Interface
├── ai_text_generate.html       # AI Content Generator
└── config.js                   # API key configuration
```

---

## ⚙️ Setup & Installation

### Step 1 — Clone the repo
```bash
git clone https://github.com/yourusername/ai-translator-launchpad.git
cd ai-translator-launchpad
```

### Step 2 — Add your Gemini API Key
Create or edit `config.js`:
```javascript
window.APP_CONFIG = {
    API_URL: "YOUR_GEMINI_API_KEY_HERE"
};
```

> 🔑 Get your free Gemini API key at:
> https://aistudio.google.com/app/apikey

### Step 3 — Run locally
Just open `index.html` in your browser — no build tools needed!

```bash
# Or use VS Code Live Server extension
```

### Step 4 — Restrict your API key (Important!)
Go to Google Cloud Console → Credentials → Edit your key
→ Add your deployed domain under HTTP referrers
→ This prevents unauthorized use of your key

---

## 🔐 API Key Security

- API key is stored in `config.js` which is listed in `.gitignore`
- Never push your actual key to GitHub
- Use `config.example.js` as reference (included in repo)
- For production — use a backend proxy to keep key server-side

---

## 🌍 Supported Languages

50+ languages including:
- All major Indian languages — Hindi, Tamil, Telugu,
  Kannada, Malayalam, Bengali, Gujarati, Marathi, Punjabi
- International — English, French, German, Spanish,
  Arabic, Chinese, Japanese, Korean, Russian and more

---

## 🤝 Contributing

This is a personal minor project but contributions
are always welcome!

1. Fork the repo
2. Create your branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -m 'Add your feature'`
4. Push: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 👤 Author

**Nishank Jain**
- 🔗 LinkedIn: [linkedin.com/in/yourprofile](https://linkedin.com/in/yourprofile)
- 💻 GitHub: [github.com/yourusername](https://github.com/yourusername)
- 📧 Email: your@email.com

---

## ⭐ Support

If you found this project useful or interesting — drop a ⭐ on the repo, it genuinely means a lot to a student builder! 🙏

---

*Built with curiosity, late nights, and a lot of Gemini API calls 😄*
