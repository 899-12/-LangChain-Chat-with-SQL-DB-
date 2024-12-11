# LangChain: Chat with SQL DB

An interactive Streamlit application that enables conversational querying and interaction with SQL databases using LangChain and Groq LLM. This project combines the power of natural language processing with database management for seamless, user-friendly database interactions.

## Features

- **Database Compatibility**: Supports SQLite and MySQL databases.
- **Conversational Querying**: Query databases using natural language with the help of Groq's LLM.
- **Dynamic Configuration**: Easily input database and API credentials via the application interface.
- **Real-Time Feedback**: Leverages `StreamlitCallbackHandler` for live updates on query processing.
- **Secure Input Handling**: API keys and database passwords are securely managed with encrypted input fields.
- **Session Management**: Maintains message history for a continuous conversational experience.

## Technology Stack

- **Streamlit**: For building an interactive frontend.
- **LangChain**: For creating the SQL agent and toolkit.
- **Groq API**: For utilizing LLMs like Llama3-8b-8192.
- **SQLAlchemy**: For database connectivity.
- **SQLite/MySQL**: Supported databases.

## Installation

1. **Clone the repository:**
   ```bash
   [git clone https://github.com/yourusername/langchain-sql-chat.git](https://github.com/899-12/-LangChain-Chat-with-SQL-DB-.git)
   cd LangChain-Chat-with-SQL-DB
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv env
   source env/bin/activate   # On Windows, use `env\Scripts\activate`
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up the database:**
   - For SQLite, place your `student.db` file in the project root directory.
   - For MySQL, ensure your database is accessible and note the connection details.

5. **Run the application:**
   ```bash
   streamlit run app.py
   ```

## Usage

1. Select your database type (SQLite or MySQL) from the sidebar.
2. Provide the necessary connection details:
   - **For SQLite:** The `student.db` file is used by default.
   - **For MySQL:** Input the host, username, password, and database name.
3. Enter your Groq API key in the sidebar.
4. Start querying the database using natural language via the chat interface.

## Example Queries

- "Show me the list of students who scored above 90."
- "What is the average score of students in the Math course?"
- "List all students enrolled in the Science department."

## Project Structure

```
langchain-sql-chat/
├── app.py                 # Main application file
├── requirements.txt       # Python dependencies
├── student.db             # Sample SQLite database (optional)
├── README.md              # Project documentation
```

## Dependencies

- Python 3.8+
- Streamlit
- LangChain
- Groq API SDK
- SQLAlchemy
- SQLite/MySQL Connector

