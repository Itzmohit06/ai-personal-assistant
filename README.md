# AI Personal Assistant

A small Flask web application that uses the OpenAI API to answer questions and summarize pasted emails.

## Features

- Ask a question and receive an AI-generated response.
- Paste an email and receive a concise summary.
- Simple browser-based interface.

## Requirements

- Python 3.10 or later
- An OpenAI API key with access to the model configured in `main.py` (`gpt-5.4`)

## Setup

Run these commands from the project directory in PowerShell:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

Create a `.env` file in the project root and add your API key:

```text
OPENAI_API_KEY=your_openai_api_key
```

Keep the key private. The `.env` file is excluded from Git.

## Run locally

With the virtual environment activated, start the Flask app:

```powershell
python main.py
```

Open [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser. The app runs with Flask's debug mode enabled for local development; do not use that mode for a public production deployment.

## Project structure

```text
.
├── main.py
├── requirements.txt
├── static/
│   └── style.css
└── templates/
    └── index.html
```
