📡 StreamSync AI – Real-Time Dockerized Chat with LLMs
A fully dockerized, real-time AI chat application that integrates LangGraph-powered AI agents, multiple LLM providers (Groq & OpenAI), and an optional web search tool — all wrapped in a Streamlit frontend. Built as part of the Generative AI Internship assignment at 21 Spheres.

🚀 Features
✅ Supports LLMs from Groq and OpenAI

✅ Optional real-time web search via Tavily

✅ Dynamically customizable system prompt

✅ Interactive UI built with Streamlit

✅ Asynchronous communication via FastAPI

✅ Fully containerized with Docker & Docker Compose

📁 Project Structure
bash
Copy
Edit
StreamSync-AI/
│
├── .venv/                  # Python virtual environment
├── __pycache__/           # Python cache
├── .dockerignore
├── .env                   # API keys and environment variables
├── docker-compose.yml     # Docker Compose configuration
├── Dockerfile.backend     # Backend Dockerfile
├── Dockerfile.frontend    # Frontend Dockerfile
│
├── requirements.txt       # Python dependencies
│
├── ai_agent.py            # LangGraph AI agent with Tavily tool
├── backend.py             # FastAPI backend for LLM communication
├── frontend.py            # Streamlit UI for chat interaction
🔧 Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/StreamSync-AI.git
cd StreamSync-AI
2. Setup .env File
Create a .env file in the root directory with the following keys:

env
Copy
Edit
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
⚠️ Ensure valid keys for Groq, OpenAI, and Tavily APIs.

🐳 Docker Deployment
Build & Run Containers
bash
Copy
Edit
docker-compose up --build
The FastAPI backend will run on: http://localhost:9999

The Streamlit frontend will be available at: http://localhost:8501

🧠 Supported LLM Models
Provider	Models
Groq	llama-3.3-70b-versatile, mixtral-8x7b-32768
OpenAI	gpt-4o-mini

🧪 Example Workflow
Open the Streamlit frontend

Define your system prompt (e.g., “Act like a travel assistant”)

Select your LLM provider and model

Enable web search if desired

Ask your query!

🛠️ Tech Stack
LangGraph – Agent-based reasoning

LangChain – LLM interfaces

Tavily – External web search

FastAPI – RESTful backend

Streamlit – Frontend UI

Docker – Containerization

