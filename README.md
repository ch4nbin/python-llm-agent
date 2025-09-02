AI Chatbot (LLM Agent)

An LLM-powered AI agent built with LangChain and LangGraph that streams real-time responses and dynamically calls Python tools (like a calculator).
This project uses OpenAI GPT models, UV for dependency management, and .env for secure API keys.

🚀 Features

🤖 LLM Agent Architecture – Uses create_react_agent to reason and act
🛠️ Tool Calling – Dynamically invokes Python functions such as a calculator
⚡ Streaming Responses – Prints AI output token-by-token for a smoother chat experience
🔒 Environment-Secured API Keys – Managed with python-dotenv
📦 Fast Dependency Management – Powered by UV

🗂️ Project Structure
AI Chatbot/
├── main.py          # Main entry point for the chatbot
├── .env             # Stores API keys (excluded from Git)
├── .gitignore       # Ignored files list
├── pyproject.toml   # Dependencies and environment setup
└── README.md        # Project documentation

🛠️ Installation & Setup

1. Clone the repository
git clone https://github.com/YOUR-USERNAME/ai-chatbot.git
cd ai-chatbot

2. Install dependencies with UV
uv init
uv sync

3. Add your API key
Create a .env file in the project root:
OPENAI_API_KEY=sk-...

4. Run the chatbot
uv run main.py

💡 Usage

Type a question or math query (e.g., What is 7+9?)
The agent decides whether to answer directly or use the calculator tool
Type quit to exit the chatbot

📚 Tech Stack

Python 3.12+
LangChain
LangGraph
OpenAI API
UV
 – fast dependency manager
python-dotenv

🔒 Security Notes

.env contains sensitive API keys – never commit this file
.gitignore is pre-configured to exclude .env and other sensitive or unnecessary files

📝 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute it as long as attribution is given.