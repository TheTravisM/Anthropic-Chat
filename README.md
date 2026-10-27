# Anthropic Chat

A small collection of Jupyter notebooks exploring the Anthropic Claude API, including a basic request exercise and a conversational chat loop.

## Contents

- `anthropic_course.ipynb` — Introductory notebook: install dependencies, load environment variables, create an API client, and make multi-turn requests with Claude.
- `001_request_exercise.ipynb` — Interactive chatbot loop that keeps a conversation history and talks to Claude indefinitely.

## Prerequisites

- Python 3.10+
- An Anthropic API key

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/TheTravisM/Anthropic-Chat.git
   cd Anthropic-Chat
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   # macOS/Linux
   source .venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install anthropic python-dotenv
   ```
4. Create a `.env` file in the project root:
   ```env
   ANTHROPIC_API_KEY="your-api-key-here"
   ```

## Usage

Open the notebooks in Jupyter or VS Code and run the cells top to bottom.

- `anthropic_course.ipynb` walks through a single multi-turn conversation with Claude.
- `001_request_exercise.ipynb` runs an interactive `>` prompt loop; type messages and Claude replies until you stop it.

## Notes

- The default model is `claude-haiku-5-5`. Change the `model` variable in the notebooks to try other Claude models.
- Never commit your `.env` file — it is gitignored.

## License

MIT
