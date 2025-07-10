
🧠 Speak2DB: Natural Language to SQL Query Generator
Turn plain English questions into live SQL queries using Google Gemini and SQLite.

📌 Overview
This project bridges the gap between non-technical users and databases by allowing them to ask questions in natural language and receive real-time SQL query results. It uses Google Gemini API to convert English prompts into SQL, which is then executed on a local SQLite database containing customer data.

💡 Goal
To empower users—regardless of technical background—to retrieve meaningful insights from a database using just natural language.

⚙️ How It Works
User Input
User types a question like:
👉 "How many customers are from US?"

Gemini API Processing
The question is sent to the Google Gemini API, which responds with an SQL query.

SQLite Execution
The SQL query runs on a local SQLite database (database.db).

Output Display
The results are shown to the user in a readable format.

🗂️ Tech Stack
Language: Python
Database: SQLite
AI Model: Google Gemini (via API)
UI (Coming Soon): Streamlit
Libraries:
google-generativeai
sqlite3
python-dotenv
🧾 Dataset Info
Source: Customer Data.csv
Table Name: CustomerData
Columns:
CustomerID
Name
Segment
Country
City
The CSV data is automatically imported into a local SQLite file (database.db) during setup.

📁 Project Structure
Revellabs_project1/ ├── app.py # Main application logic ├── sql.py # CSV to SQLite conversion script ├── database.db # SQLite DB file (auto-created) ├── .env # Google API key ├── requirements.txt # Python dependencies └── README.md # Project documentation

🚀 Setup Instructions
Clone the repository
git clone https://github.com/your-username/Speak2DB.git

2.Add your Google Gemini API key to a .env file

GOOGLE_API_KEY="your-api-key-here"

3.Create a virtual environment (optional but recommended)

python -m venv venv venv\Scripts\activate # Windows source venv/bin/activate # macOS/Linux

4.Install required libraries

pip install -r requirements.txt

5.Run the SQL setup script

python sql.py

6.Launch the main application

python app.py

✅ Features

🔄 Convert natural language to SQL using Google Gemini

⚡ Execute queries in real-time on SQLite database

📊 Designed for customer data analysis

🧩 Easily expandable to support more complex datasets or AI models

🖥️ Streamlit UI integration coming soon

📬 Contact For suggestions or collaboration, reach out to: 📧 krishnachauhannsut@gmail.com

About
No description, website, or topics provided.
Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 0 watching
Forks
 0 forks
Releases
No releases published
Create a new release
Packages
No packages published
Publish your first package
Languages
Python
100.0%
Suggested workflows
Based on your tech stack
Python application logo
Python application
Create and test a Python application.
Django logo
Django
Build and Test a Django Project
SLSA Generic generator logo
SLSA Generic generator
Generate SLSA3 provenance for your existing release workflows
More workflows
Footer
©
