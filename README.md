Agentic AI Executive Personal Assistant

📌 Overview
An AI-powered multi-agent personal assistant capable of managing emails, scheduling meetings, performing intelligent web research, and interacting via voice or text.
The system uses specialized agents orchestrated by a central controller with GPT-4o-mini for reasoning and dynamic tool selection.

🚀 Features
* 📧 Email Agent → Read, summarize, and draft emails via Gmail API.
* 📅 Calendar Agent → Create, update, and retrieve events from Google Calendar.
* 🌐 Scraper Agent → Autonomous web browsing & data extraction using Playwright + GPT Vision.
* 🎙️ Voice Input → Real-time speech-to-text with OpenAI Whisper.
* 🧠 Intelligent Routing → GPT-4o-mini decides which agent to use for a given request.
* 🔌 Extensible → Easily integrate new tools and APIs.

🛠 Tech Stack
* Python
* OpenAI GPT-4o-mini & Whisper
* Google Calendar API & Gmail API
* Playwright, BeautifulSoup
* dotenv, pyaudio, keyboard

📂 Project Structure

main_agent.py       # Central controller
calendar_agent.py   # Calendar scheduling agent
email_agent.py      # Email management agent
scrapper_agent.py   # Web scraping agent
requirements.txt    # Project dependencies
assets/             # Diagrams & visuals

🔑 Setup Instructions

1️⃣ Clone the repository
git clone <repository-url>
cd executive-ai-personal-assistant

2️⃣ Create a virtual environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

3️⃣ Install dependencies
pip install -r requirements.txt
pip install playwright keyboard
python -m playwright install

4️⃣ Add environment variables
Create a .env file in the project root:
OPENAI_API_KEY=your_openai_api_key

5️⃣ Set up Google APIs
Enable Gmail API & Google Calendar API in Google Cloud Console.
Download credentials.json into the project root.
On first run, authorize access — tokens will be stored locally.

6️⃣ Run the assistant
python main_agent.py

🖥 Usage
* Press t → Type a command.
* Hold spacebar → Speak your command.
* Press q → Quit the program.

💬 Example commands:
* “Summarize my unread emails.”
* “Schedule a meeting with Sarah next Tuesday at 2 PM.”
* “Find the latest AI research articles.”


  
