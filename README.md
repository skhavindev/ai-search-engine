# AI Search Engine V1 [Update: I am in the process of updating this to multi agentic system. This works but is inefficient than multi agentic systems]

## Overview

Welcome to **TextFusion.AI Intelligent Search**, a cutting-edge AI-powered search engine designed to deliver intelligent and context-rich answers to user queries. This app utilizes the **Tavily Search API** for retrieving web-based content and the **ChatGroq API** for generating human-like, comprehensive responses based on the retrieved context. The app is built using Streamlit for its web interface.

## Features

- **Custom Search Functionality**: Users can input a query into a search bar, and the app retrieves relevant results from the web.
- **Tavily Search API Integration**: Uses the Tavily Search API to find web content related to user queries.
- **ChatGroq API Integration**: Employs the Groq AI model to generate well-formulated answers based on the search results.
- **Stylish Interface**: Includes a sleek design with a search icon and custom fonts, offering an intuitive user experience.
- **Comprehensive Responses**: Provides detailed and context-driven answers with citations for better user satisfaction.
- **Environment Setup**: API keys can be easily configured using environment variables for both Tavily and Groq APIs.

## Requirements

- **Python 3.8+**
- **Streamlit**
- **Langchain** 
- **Tavily Search API key**
- **Groq API key**

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-repo/ai-search-engine.git
cd ai-search-engine
```

### 2. Install Required Packages

Install the necessary Python packages using `pip`:

```bash
pip install streamlit langchain langchain-community pydantic
```

### 3. Environment Variables

Ensure that the API keys for **Tavily** and **Groq** are set as environment variables. You can do this by creating an `.env` file in the root directory or setting them directly in your system.

```bash
export TAVILY_API_KEY=your_tavily_api_key
export GROQ_API_KEY=your_groq_api_key
```

### 4. Custom CSS (Optional)

If you'd like to use custom styles, make sure you have a `style.css` file in the root folder of the project. If not found, the app will fall back to default styles.

### 5. Run the App

You can run the application locally using the following command:

```bash
streamlit run app.py
```

This will open the app in your default web browser.

## Usage

- Open the app and type a query into the search bar.
- Press **OK** to submit your query.
- The app will retrieve relevant results and generate an intelligent response based on the content.

## Code Structure

- **`SearchEngine` Class**: The core search engine class that integrates Tavily Search API and Groq AI for query resolution.
- **`SearchResult` Class**: Handles the search results retrieved from the Tavily API.
- **Streamlit UI**: The main interface that allows users to interact with the search engine.

### Functions

- `search(query: str)`: Takes a query and returns the search result using Tavily and Groq APIs.
- `local_css(file_name: str)`: Loads local custom CSS for styling.
- `remote_css(url: str)`: Loads external CSS for adding custom fonts or styles.
- `icon(icon_name: str)`: Adds a material icon to the UI.

### External Dependencies

- **Langchain**: Handles the connection between the search API and AI model.
- **Pydantic**: Used for request and response modeling.
- **Streamlit**: Provides the web UI framework.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

If you have any issues, please reach out to us on [Instagram](https://instagram.com/textfusion.ai).

---

**Made by TextFusion.AI✨**
