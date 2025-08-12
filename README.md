Agentic AI Executive Personal Assistant
📌 Overview
An AI-powered multi-agent executive assistant designed to automate day-to-day professional tasks like email management, calendar scheduling, intelligent web research, and voice-based interaction.
Inspired by Jarvis, this system uses specialized AI agents orchestrated by a central controller for dynamic, context-aware decision-making.

🚀 Features
Multi-Agent Architecture

Email Agent → Reads, summarizes, and drafts emails via Gmail API.

Calendar Agent → Creates, retrieves, and manages Google Calendar events.

Scraper Agent → Autonomous web navigation & data extraction using Playwright + GPT Vision.

Voice Interaction → Real-time transcription with OpenAI Whisper.

Autonomous Reasoning → GPT-4o-mini for dynamic tool selection & context maintenance.

Web Automation → Playwright browser control + BeautifulSoup for parsing content.

Extensible → Easily add new agents for other domains (e.g., finance, note-taking).

🛠️ Tech Stack
Python, OpenAI GPT-4o-mini, Whisper

Google Calendar API, Gmail API

Playwright, BeautifulSoup

dotenv, pyaudio, keyboard

📂 Project Structure
bash
Copy
Edit
main_agent.py       # Central orchestrator
calendar_agent.py   # Calendar management agent
email_agent.py      # Email management agent
scrapper_agent.py   # Web scraping agent
requirements.txt    # Dependencies
assets/             # Diagrams & workflow

🖼 Workflow

💡 How It Works
User speaks or types a request.

Main Agent decides whether it can answer directly or delegate to a sub-agent.

Sub-Agent performs the task using APIs/tools.

The result is returned to the Main Agent and delivered to the user.

📜 Example Commands
“Summarize my unread emails.”

“Schedule a meeting with Sarah next Friday at 4 PM.”

“Find and summarize the latest AI research news.”

🔑 Setup
Clone Repository

bash
Copy
Edit
git clone https://github.com/<your-username>/Executive-AI-Personal-Agent.git
Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
Add API Key


Create .env file in root:
ini
Copy
Edit
OPENAI_API_KEY=your_openai_key_here
Set Up Google APIs

Enable Gmail API & Google Calendar API in Google Cloud.

Download credentials.json into the root directory.

Run the Project

bash
Copy
Edit
python main_agent.py
