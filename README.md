# AI-Notes-to-QUIZ
# Quizzer

**Turn your PDFs and PowerPoints into quizzes — instantly.**

Quizzer is a web app that lets students upload lecture notes or slides and get AI-generated quiz questions to study smarter. No manual flashcard creation, no copy-pasting — just upload and go.

---

## Features

- **File Upload** — Drag and drop or browse to upload `.pdf` or `.pptx` files
- **AI-Powered Questions** — Automatically generates targeted multiple-choice questions from your content
- **Instant Quiz** — Jump straight into a quiz after upload with answer feedback and scoring
- **Score Summary** — See your final score with a visual score ring after completing the quiz
- **Clean UI** — Minimal, distraction-free design with smooth transitions and mobile support
- **PWA Ready** — Installable on mobile via a Web App Manifest and Service Worker

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, Tailwind CSS (CDN), JavaScript |
| Backend | Python (Flask / server-side templating with Jinja2) |
| AI | Gorq API — question generation |
| File Parsing | PDF and PPTX text extraction |

---

## How It Works

1. **Upload** your PDF lecture notes or PowerPoint slides
2. **AI processes** the content and extracts key concepts
3. **A quiz is generated** with multiple-choice questions
4. **You answer** each question and get instant feedback
5. **See your score** at the end and review what you got wrong

---

## Getting Started

### Prerequisites

- Python 3.8+
- An Groq API Key

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/quizzer.git
cd quizzer

# Install dependencies
pip install -r requirements.txt

# Add your API key
cp .env.example .env
# Then edit .env and add: ANTHROPIC_API_KEY=your_key_here

# Run the app
python app.py
```

Then open `http://localhost:5000` in your browser.

---

## Supported File Formats

| Format | Description |
|---|---|
| `.pdf` | Lecture notes, textbook excerpts |
| `.ppt` / `.pptx` | Slides from any version of PowerPoint |

---

## Project Structure

```
quizzer/
├── static/
│   ├── manifest.json       # PWA manifest
│   └── sw.js               # Service Worker
├── templates/
│   └── upload.html         # Main UI
├── app.py                  # Flask app + routes
├── requirements.txt
└── .env.example
```

---

## Screenshots

no screenshots yet

---
