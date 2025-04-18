# 🔎 LangChain Search Engine

A powerful search engine application built with Streamlit and LangChain that allows users to search the web, arXiv papers, and Wikipedia using natural language queries.

## Features

- **Multi-source Search**: Query information from:
  - Web (DuckDuckGo)
  - arXiv scientific papers
  - Wikipedia articles
- **Conversational Interface**: Chat-based UI for natural interaction
- **AI-powered Responses**: Uses Groq's Llama3-8b model to generate human-like responses
- **Transparent Reasoning**: View the agent's thought process in real-time

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/search_engine.git
   cd search_engine
   ```

2. Create and activate a virtual environment:
   ```
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Get a Groq API key from [Groq's website](https://console.groq.com/).

## Usage

1. Run the Streamlit app:
   ```
   streamlit run app.py
   ```

2. Enter your Groq API key in the sidebar.

3. Start chatting with the search engine by typing your queries in the chat input.

## How It Works

The application uses LangChain to orchestrate multiple tools:
- DuckDuckGo for web searches
- arXiv API for scientific paper searches
- Wikipedia API for encyclopedia lookups

The Llama3-8b model from Groq processes your queries, determines which search tools to use, and generates comprehensive responses based on the search results.

## Requirements

See the `requirements.txt` file for a complete list of dependencies.

## License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.
