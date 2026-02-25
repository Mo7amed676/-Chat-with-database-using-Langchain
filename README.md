# Chat-with-database-using-Langchain

A conversational interface for interacting with databases using LangChain and Google Generative AI. This project enables users to query databases in natural language through a Streamlit web application.

## Features

- **Natural Language Processing**: Convert user queries to SQL using Google Generative AI
- **Multi-Application Support**: Multiple implementations including basic and advanced Langchain versions
- **Database Integration**: Support for PostgreSQL and other SQL databases via SQLAlchemy
- **Web Interface**: User-friendly Streamlit application
- **Environment Configuration**: Secure handling of credentials via .env files

## Project Structure

- **app.py** - Basic Streamlit application for database interaction
- **app_langC.py** - Advanced Langchain implementation with enhanced capabilities
- **deploy.py** - Deployment utilities and configuration
- **test.py** - Testing module for functionality validation
- **requirements.txt** - Python dependencies
- **Schema.jpg** - Database schema diagram

## Requirements

The project uses the following Python packages:
- `streamlit` - Web application framework
- `pandas` - Data manipulation and analysis
- `sqlalchemy` - SQL toolkit and ORM
- `python-dotenv` - Environment variable management
- `langchain-google-genai` - LangChain integration with Google Generative AI
- `psycopg2` - PostgreSQL database adapter

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Setup

1. Clone the repository:
```bash
git clone https://github.com/Mo7amed676/-Chat-with-database-using-Langchain.git
cd -Chat-with-database-using-Langchain
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Configure environment variables:
   - Create a `.env` file in the project root
   - Add your database connection string
   - Add your Google Generative AI API key

4. Run the application:
```bash
streamlit run app.py
```

Or for the advanced Langchain version:
```bash
streamlit run app_langC.py
```

## Usage

1. Start the Streamlit application
2. Enter your natural language query about the database
3. The system converts your query to SQL using Google Generative AI
4. Results are displayed in the web interface

## Architecture

The system uses a schema-aware approach where:
- Database schema is analyzed and provided to the AI model
- User queries are converted to appropriate SQL statements
- Results are fetched and displayed in an interactive format

See `Schema.jpg` for the database structure.

## Testing

Run tests using:
```bash
python test.py
```

## Deployment

Use `deploy.py` for deployment configuration and utilities.

## Technologies Used

- **LangChain** - Framework for building applications with language models
- **Google Generative AI** - AI-powered query generation
- **Streamlit** - Web application framework
- **SQLAlchemy** - Database abstraction layer
- **PostgreSQL** - Database system

## License

This project is available on GitHub at: https://github.com/Mo7amed676/-Chat-with-database-using-Langchain
