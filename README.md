# 📚 AI Reimagine Storytelling

An AI-powered web app to generate illustrated stories for children with live narration, multilingual support, PDF export, and QR sharing — all from one screen.

---

![screenshot](https://via.placeholder.com/1200x600?text=AI+Reimagine+Storytelling+App+Preview)

---

## ✨ Key Features

🧠 AI-Powered Story Generation
Craft unique, multi-scene stories using large language models (LLMs) powered by Ollama.

🎙️ Voice Input for Creativity
Use your microphone to speak your character, genre, theme, or illustration style — no typing needed!

🎨 Scene-by-Scene Illustrations
Generate beautiful AI images for each scene using the DeepAI Text-to-Image API (optional).

🔊 Multilingual Voice Narration
Stories are narrated using Google Text-to-Speech (gTTS) with support for multiple languages and voice speed options.

📄 PDF Export
Convert your entire illustrated story into a print-ready PDF, complete with custom fonts and layout.

📲 QR Code Sharing
Share your story via an auto-generated QR code that links to the downloadable version or cloud copy.

🌗 Responsive, Themed Interface
Enjoy a clean UI with Light/Dark mode toggle, background image support, and styled inputs for better usability.

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
git clone https://github.com/alfagen10/ai-reimagine-storytelling.git
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

Licensed under the **MIT License** — free for personal and commercial use.
See the LICENSE file for full terms.

---

## 👨‍🎨 Author

Made with ❤️ by **Al Faruk Md Omor Sajeeb**  
📧 Email: alfarukmd78@gmail.com
🔗 GitHub: https://github.com/alfagen10


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

