🦜 LangChain SQL Chatbot with Streamlit & Groq

A Streamlit-based AI-powered chatbot that lets you query a SQL database (SQLite or MySQL) using natural language, powered by LangChain and Groq's LLaMA3 model.


🚀 Features
🤖 Chat with your database using plain English


🗃️ Connects to either:

Local SQLite (student.db)

Remote MySQL

🧠 Powered by LangChain agents + Groq LLaMA3-8B

🧰 Uses SQLDatabaseToolkit for schema-aware queries

💬 Interactive, persistent chat history with reset option

📦 Requirements
Python 3.8+
```
pip install -r requirements.txt
```
🔌 Required Packages:
bash
```
streamlit
langchain
langchain_groq
python-dotenv
sqlalchemy
mysql-connector-python
```

You can install them using:

bash
```
pip install streamlit langchain langchain_groq python-dotenv sqlalchemy mysql-connector-python
```

🔐 Environment Variables
Create a .env file in the project root with:

env
```
GROQ_API_KEY=your_groq_api_key_here
```
🗂️ Folder Structure
bash
```
project-root/
│
├── student.db                  # Sample SQLite database (optional)
├── app.py                      # Main Streamlit app
├── .env                        # API key here
└── README.md                   # This file
```

💻 How to Run
bash
```
streamlit run app.py
```

🧠 How It Works
User selects either SQLite or MySQL.

The app connects to the selected DB using SQLAlchemy.

LangChain uses SQLDatabaseToolkit and create_sql_agent with Groq's LLM.

The agent intelligently understands and runs SQL queries behind the scenes.

Responses are streamed in the chat window with real-time feedback.


🧪 Example Prompts
"What is the average score of students in class 10?"

"List the top 5 students by marks."

"How many students registered after Jan 2023?"

🔧 TODO / Enhancements
 Add upload option for user’s own .db files

 Add support for PostgreSQL

 Add query logging and export

 Add role-based access or authentication

 <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8428c18b-75b0-4a8f-b498-20a448e8fa8a" />





🧑‍💻 Author
Built with ❤️ by Mansi Arora

Feel free to contribute or raise an issue!
