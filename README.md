# Agentic-Workflows--GenAI
# 🧠 Agentic Workflows & Multi-Modal GenAI App

[![Streamlit](https://img.shields.io/badge/Built%20With-Streamlit-FF4B4B?logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![OpenAI](https://img.shields.io/badge/LLM-OpenAI-412991)](https://platform.openai.com/)

A powerful, Streamlit-native multi-modal AI workspace that bridges the gap between simple AI utilities and fully autonomous agentic workflows. It serves as a unified operations desk for research synthesis, document intelligence, code generation, content creation, and support triage.

Unlike standard single-prompt demos, this application features multi-step reasoning, retrieval augmentation, and structured AI pipelines.

---

## 🌟 Key Features & Workspaces

The application is cleanly organized into three distinct operational workspaces:

### 1. 📚 Assistant Tool (Agentic Workflows)
Focused on retrieval, planning, reasoning, and workflow-based AI assistance.
- **Research Agent:** Accepts a topic and URLs, creates a research plan, reads sources, synthesizes a cited report, and revises its own output.
- **Document Intelligence:** Extracts text/OCR from PDFs, DOCX, TXT, or images. Classifies the document, extracts key entities, and automatically generates action items and deadlines.
- **Document QnA:** Builds a local FAISS vector index over your uploaded files to answer questions accurately based on document context.
- **Support & Triage Agent:** Classifies support requests by intent and severity, drafts grounded answers, scores its own confidence, and automatically escalates complex issues.

### 2. 🎨 Generator Tool (Creation Workflows)
Focused on multimodal creation and organized output generation.
- **Code Copilot:** Prompt-based code generation with built-in execution/verification checks and automatic self-repair passes if verification fails. (Supports Python, JS, Java, C, C++).
- **Multimodal Content Pipeline:** Autonomously plans a content strategy, writes scripts, generates image prompts, writes platform-specific captions, and generates hashtags.
- **Text-to-Image & Text-to-Speech:** Generates custom images and high-quality audio narrations using local or API-based models.

### 3. 📝 Summarizer Tool
Focused on compressing raw information into structured, readable insights.
- **Text Summarizer:** Condenses long-form text using OpenAI models with fallbacks to local Hugging Face pipelines.
- **YouTube Summarizer:** Automatically extracts YouTube video transcripts and provides concise summaries.
- **Article Summarizer:** Scrapes readable text directly from web URLs and summarizes the core contents.
- **Image Text / OCR Extractor:** Processes image files using Tesseract OCR to extract and summarize visual text.

---

## 🛠️ Technology Stack

This project was built entirely in Python using a robust AI stack:
- **Frontend:** Streamlit
- **AI / LLM:** OpenAI API, LangChain
- **Vector Search:** FAISS
- **Processing:** PyMuPDF (PDFs), python-docx (Word), pytesseract (OCR), youtube-transcript-api
- **Local Fallbacks:** Hugging Face Transformers, PyTorch

---

## 🚀 Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/Tapanwankhade/Agentic-Workflows--GenAI.git
cd Agentic-Workflows--GenAI
```

### 2. Create and activate a virtual environment
```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configuration
You can supply your API key right from the Streamlit UI, or create a `.env` file in the root directory:
```env
OPENAI_API_KEY=sk-your-actual-api-key-here
```

### 5. Run the Application
```bash
streamlit run main.py
```
*The app will automatically launch in your browser at `http://localhost:8501`*

---

## 📋 Requirements & Limitations
- **OpenAI API Key:** Required for all LLM reasoning, code generation, and advanced agentic workflows.
- **Tesseract OCR:** Required to use the "Image Text Extractor". Must be installed on your system (e.g., `C:\Program Files\Tesseract-OCR\tesseract.exe`).
- **Code Copilot Safety:** Local execution is used to verify code. Use caution when running generated code that interacts with the filesystem.

---

## 👨‍💻 Author

**TAPAN JAYDEO WANKHADE**  
Email: [tapanjw@gmail.com](mailto:tapanjw@gmail.com)
