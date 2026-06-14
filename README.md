# 🎓 EduBot AI — AI Education Assistant

<div align="center">

![EduBot AI](https://img.shields.io/badge/EduBot-AI-6c63ff?style=for-the-badge&logo=graduation-cap&logoColor=white)
![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-API-00d2ff?style=for-the-badge)
![Vite](https://img.shields.io/badge/Vite-8-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**An AI-powered education chatbot that helps you learn any subject.**  
Built with React.js and Groq AI API for fast, intelligent responses.

[🚀 Live Demo](#) · [📖 Features](#features) · [🛠️ Setup](#getting-started)

</div>

---

## 📋 About

EduBot AI is a web-based education chatbot built as the **Final Project** for the **"Maju Bareng AI for Data Analyst"** bootcamp by **Hacktiv8**. The project demonstrates the integration of LLM-based tools and API integration for practical applications in education.

### Use Case
- **Education Bot** — An AI assistant that helps users learn across all subjects with customizable interaction styles.

### Creative Parameters
- 🌐 **Bilingual** — Supports Bahasa Indonesia and English
- 🎭 **Communication Style** — Formal, Santai (Casual), or Akademik (Academic)
- 🧠 **Memory** — Maintains conversation history and context
- 📊 **Data Analysis** — Upload CSV/Excel files for AI-powered analysis
- 📈 **Visualization** — Generate charts and graphs from data
- 🎨 **Customizable UI** — Light and Dark theme support

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 💬 **Smart Chat** | Natural language conversation with streaming responses |
| 🧠 **Memory** | Persistent conversation history with multiple threads |
| 📎 **File Upload** | Support for CSV, XLSX, XLS, JSON, TXT, and images |
| 📊 **Data Charts** | Auto-generate bar, line, pie, doughnut, scatter, radar charts |
| 🎨 **Theme Toggle** | Beautiful dark and light mode with smooth transitions |
| ⚙️ **Settings** | API key management, model selection, temperature, max tokens |
| 📝 **Markdown** | Rich text rendering with syntax highlighting |
| 📱 **Responsive** | Works on desktop, tablet, and mobile devices |
| 💾 **Export** | Export conversations as Markdown files |

---

## 🛠️ Tech Stack

- **Frontend**: React.js 19 (Vite)
- **AI API**: Groq API (LLaMA 3.3, Mixtral, Gemma)
- **Charts**: Chart.js + react-chartjs-2
- **Markdown**: react-markdown + remark-gfm
- **Code Highlighting**: react-syntax-highlighter
- **File Parsing**: PapaParse (CSV), SheetJS (Excel)
- **Icons**: Lucide React
- **Styling**: Vanilla CSS with CSS Variables

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- Groq API Key (free at [console.groq.com](https://console.groq.com/keys))

### Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/edubot-ai.git
cd edubot-ai

# Install dependencies
npm install

# Start development server
npm run dev
```

### Configuration
1. Open the app in your browser
2. Click the **Settings** (⚙️) button
3. Paste your **Groq API Key**
4. Click **Save** (optionally **Test** to verify)
5. Start chatting! 🎉

---

## 📸 Screenshots

### Dark Mode
*Welcome screen with suggested prompts in dark theme*

### Light Mode
*Clean and bright light theme with glassmorphism effects*

### Settings Panel
*Full configuration panel with API key, language, style, model, and parameter controls*

### Chat Conversation
*Real-time streaming conversation with markdown rendering*

---

## 📂 Project Structure

```
src/
├── components/
│   ├── Chat/          # Chat window, message bubbles, input, typing indicator
│   ├── Chart/         # Dynamic chart renderer (7 chart types)
│   ├── Common/        # Header, theme toggle
│   ├── Settings/      # Settings panel with all configurations
│   └── Sidebar/       # Conversation list management
├── hooks/
│   ├── useChat.js     # Core chat logic & API integration
│   ├── useTheme.js    # Theme management
│   └── useLocalStorage.js  # Persistent storage
├── services/
│   ├── groqApi.js     # Groq API client with streaming
│   └── fileParser.js  # CSV/Excel/JSON file parsing
├── utils/
│   ├── constants.js   # App configuration & defaults
│   ├── helpers.js     # Utility functions
│   └── systemPrompts.js  # Dynamic AI prompt builder
├── App.jsx            # Root component
├── App.css            # Layout styles
├── index.css          # Design system & global styles
└── main.jsx           # Entry point
```

---

## 🔑 API Configuration

EduBot AI uses the **Groq API** for fast LLM inference. Available models:

| Model | Description |
|-------|-------------|
| LLaMA 3.3 70B | Best for complex reasoning & explanations |
| LLaMA 3.1 8B | Fast & lightweight responses |
| LLaMA 3 70B | Great balance of speed & quality |
| Mixtral 8x7B | Strong multilingual support |
| Gemma 2 9B | Google's instruction-tuned model |

> **Note**: API keys are stored in your browser's localStorage, never in the source code. Your key stays on your device.

---

## 🌐 Deployment (GitHub Pages)

```bash
# Build for production
npm run build

# The build output will be in the 'dist' folder
# Deploy to GitHub Pages using gh-pages or manually
```

For GitHub Pages, update `vite.config.js`:
```javascript
export default defineConfig({
  base: '/your-repo-name/',
  plugins: [react()],
})
```

---

## 👨‍💻 Author

**Final Project — Bootcamp Maju Bareng AI for Data Analyst by Hacktiv8**

---

## 📄 License

This project is for educational purposes as part of the Hacktiv8 bootcamp final project.
