Features
Log Water Intake: Easily record your daily water consumption in milliliters.
AI-Powered Feedback: Get intelligent insights and feedback on your hydration habits from an integrated AI assistant.
Intake History: View your past water intake data in a clear, interactive dashboard.
Data Visualization: See your hydration trends over time with intuitive charts.
🛠️ Technologies Used
The AI Water Tracker is built using the following technologies:

Frontend:
Streamlit: For creating an interactive and user-friendly web interface.
Backend & AI:
Langchain: An LLM framework for developing the AI agent.
OpenAI: Powers the AI's language capabilities (via OpenRouter API).
FastAPI: A modern, fast (high-performance) web framework for building APIs.
Uvicorn: An ASGI server for running the FastAPI application.
Database:
SQLite: A lightweight, file-based database for storing water intake data.
SQLAlchemy: An SQL toolkit and Object-Relational Mapper (ORM) for Python.
sqlite-utils: A Python library for working with SQLite databases.
Other:
python-dotenv: For managing environment variables.
Loguru: For simplified logging and debugging.
APScheduler: For task scheduling (e.g., for reminders, though not fully implemented in provided files).
Typer: (Optional) For building command-line interfaces.
Pandas: For data manipulation and analysis in the dashboard
Getting Started
Follow these steps to set up and run the AI Water Tracker on your local machine.

Prerequisites
Python 3.8+
pip (Python package installer)
Installation
Clone the repository (if applicable):

git clone <repository_url>
cd water-intake-agent
(Note: As the project was provided as files, this step assumes it's part of a larger repository. If not, simply ensure all files are in a single directory.)

Create a virtual environment (recommended):

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install the required dependencies: The requirements.txt file lists all necessary libraries.

pip install -r requirements.txt
Set up environment variables: Create a .env file in the root directory of your project and add your OPENAI_API_KEY and DATABASE_URL.

OPENAI_API_KEY="your_openrouter_api_key_here"
DATABASE_URL=sqlite:///water-tracker.db
Replace "your_openrouter_api_key_here" with your actual API key from OpenRouter.

Running the Application
Run the Streamlit Dashboard:
streamlit run dashboard.py
This command will open the AI Water Tracker dashboard in your web browser.
🚀 Usage
Start Tracking: Click the "Start Tracking" button on the welcome page.
Enter User ID: Provide a unique user ID in the sidebar. The default is user_123.
Log Water Intake: Enter the amount of water (in ml) you've consumed and click "Submit".
View Feedback and History: The dashboard will display AI feedback and update your intake history, including a line chart visualizing your progress.
