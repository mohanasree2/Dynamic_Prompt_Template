# AI Research Paper Summarization Tool
## Dynamic_Prompt_Template

An interactive, LLM-powered web application that generates structured, customizable summaries of groundbreaking AI and Deep Learning research papers. Built using **Streamlit**, **LangChain Core**, and **Google Gemini (GenAI)**.

This tool allows users to select a foundational AI research paper and configure a summary based on their desired explanation style (e.g., Beginner-Friendly, Technical, Code-Oriented, Mathematical) and response length constraints.

---

##  Features

- **Multi-Style Explanations**: Adapt outputs from conceptual intuition/analogies to hard math or functional code snippets.
- **Dynamic Prompt Templating**: Leverages LangChain's `PromptTemplate` to safely assemble structured metadata payloads.
- **Strict Guardrails**: Explicitly structured to prevent model hallucinations ("Insufficient information available" fallback).
- **Modern LLM Integration**: Orchestrated with Google's state-of-the-art `gemini-2.5-flash` engine.

---

##  Project Structure

```text
research-paper-summarizer/
│
├── prompt_ui.py         # Main Streamlit application file
├── requirements.txt     # Python dependencies tracking
├── .env                 # Environment secrets (API Keys)
├── .gitignore           # Git ignore configurations
└── README.md            # Documentation
```
## Configure Your Virtual Environment
```bash
# Create the virtual environment
python -m venv venv

# Activate the environment
# On Windows (Command Prompt):
venv\Scripts\activate
# On Windows (PowerShell):
.\venv\Scripts\Activate.ps1
# On macOS/Linux:
source venv/bin/activate
```
## Install Required Dependencies
```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```
## Authentication Configuration
```Plaintext
GOOGLE_API_KEY=your_actual_gemini_api_key_here
```
## How to run the application
```Bash
python -m streamlit run prompt_ui.py
```

