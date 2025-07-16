# 📚 AI Reimagine Storytelling

An AI-powered web app to generate illustrated children’s stories with live narration, multilingual support, PDF export, and QR sharing — all from one screen.

---

![screenshot](https://via.placeholder.com/1200x600?text=AI+Reimagine+Storytelling+App+Preview)

---

## ✨ Features

- 🧠 Generate children's stories with LLM (via Ollama)
- 🎙️ Use microphone input to speak character/genre/theme
- 🎨 Scene-based illustrations using DeepAI API
- 🔊 Narrate stories using Google Text-to-Speech in multiple languages
- 📄 Export full story to PDF
- 📲 Share with QR Code
- 🌗 Beautiful UI with Dark/Light Mode and background

---

## 🧑‍💻 A–Z Setup Instructions

### 🪜 A. Prerequisites

Make sure these are installed:
- ✅ Python 3.9+ → [Download here](https://www.python.org/downloads/)
- ✅ Git → [Install Git](https://git-scm.com/)
- ✅ FFmpeg (for audio) → `sudo apt install ffmpeg` or use [ffmpeg.org](https://ffmpeg.org/)
- ✅ [Ollama](https://ollama.com/) → to run the local AI model (e.g. `mistral`)

---

### 🪜 B. Clone the Repository

```bash
git clone https://github.com/yourusername/ai-reimagine-storytelling.git
cd ai-reimagine-storytelling
```

---

### 🪜 C. Create and Activate Virtual Environment (Recommended)

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

---

### 🪜 D. Install Required Python Packages

```bash
pip install -r requirements.txt
```

---

### 🪜 E. Configure Your API Key (DeepAI)

Create the folder and secrets file:
```bash
mkdir -p .streamlit
```

Then edit or create `.streamlit/secrets.toml`:

```toml
[api]
deepai_key = "your_deepai_api_key_here"
```

🗝️ Get a free API key at [https://deepai.org/](https://deepai.org/)

---

### 🪜 F. Start the Ollama AI Model

Install Ollama if not yet installed, then:

```bash
ollama run mistral
```

Keep this running in the background.

---

### 🪜 G. Run the App

In another terminal:

```bash
streamlit run app.py
```

Then visit: [http://localhost:8501](http://localhost:8501)

---

## 📦 Folder Structure

```
ai-reimagine-storytelling/
├── app.py
├── requirements.txt
├── README.md
├── DejaVuSans.ttf
├── LICENSE
└── .streamlit/
    └── secrets.toml
```

---

## 🔤 Supported Languages

- English 🇬🇧
- Bengali 🇧🇩
- Hindi 🇮🇳
- Urdu 🇵🇰
- Arabic 🇸🇦
- Chinese 🇨🇳
- Japanese 🇯🇵
- Malay 🇲🇾
- German 🇩🇪
- Spanish 🇪🇸

---

## 📄 License

Licensed under the **Apache License 2.0** — Free for commercial or personal use.  
See [`LICENSE`](LICENSE) for full terms.

---

## 👨‍🎨 Author

Made with ❤️ by **Al Faruk Md Omor Sajeeb**  
📧 [youremail@example.com](mailto:youremail@example.com)  
🔗 [GitHub](https://github.com/alfagen10)

---

## 🙋 FAQ

**Q: Do I need OpenAI or ChatGPT API key?**  
A: ❌ No! This app uses **Ollama** with free, local models like `mistral`.

**Q: Can I run this offline?**  
A: ✅ Yes — once you've downloaded the model and have the packages, it works fully offline.

**Q: Do I need the DeepAI API?**  
A: Only if you want scene illustrations — otherwise, you can skip it.

---

## 🌟 Show Your Story

Use `#AIReimagineStorytelling` on GitHub or social to share what you've made!

