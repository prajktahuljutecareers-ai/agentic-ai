# Agentic AI

This repository contains initial LangChain examples written in Python. The notebooks demonstrate language-model integration, tools, messages, structured output, middleware, and agent workflows.

## Prerequisites

- Python 3.14 or later
- Git
- VS Code with the Python and Jupyter extensions
- A Google Gemini API key
- `uv` for Python environment and dependency management

Install `uv` on Windows with PowerShell:

```powershell
irm https://astral.sh/uv/install.ps1 | iex
```

Verify the installation:

```powershell
uv --version
python --version
```

## Get a Google Gemini API key

1. Open [Google AI Studio](https://aistudio.google.com/apikey).
2. Sign in with your Google account.
3. Select **Create API key**.
4. Copy the key and keep it private.

Never commit an API key to GitHub. If a key is exposed, revoke it and create a new one.

## Set up the project

Clone the repository and enter its folder:

```powershell
git clone https://github.com/prajktahuljutecareers-ai/agentic-ai.git
cd agentic-ai
```

Create the project environment and install dependencies:

```powershell
uv sync
```

Create `.env` in the project root, beside `pyproject.toml`:

```powershell
Copy-Item .env.example .env
```

Open `.env` and replace the placeholder:

```env
GOOGLE_API_KEY=your_google_api_key
```

The `.env` file is ignored by Git and must remain on your computer only.

## Run the notebooks

1. Open the repository in VS Code.
2. Open a notebook under `updatedlangchain/`.
3. Select the project Python environment as the notebook kernel.
4. Run the cells from top to bottom.

The notebooks use `python-dotenv` to load `GOOGLE_API_KEY` from `.env`.

