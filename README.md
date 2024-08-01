# Tamil-Nadu-Scheme-Connect
"Tamil Nadu Scheme Connect" is a Streamlit app that provides detailed information about Tamil Nadu's services and schemes. It indexes official documents for efficient data retrieval and uses a chat interface to process user queries, ensuring accurate and relevant responses based on the official information from Tamil Nadu's government websites.

## Overview

The *Tamil Nadu Scheme Connect* is a web application built using Streamlit that provides users with detailed information about government schemes and services available in Tamil Nadu. The app utilizes advanced document indexing and query processing to deliver accurate and concise answers based on user queries.

## Features

- *Document Indexing*: Automatically indexes documents for efficient search and retrieval.
- *Query Handling*: Processes user queries to extract relevant information from indexed documents.
- *Streamlit Interface*: Provides an interactive web-based interface for users to ask questions and receive responses.
- *Government Sources*: Retrieves additional information from official Tamil Nadu government websites.

## Installation

1. *Clone the Repository*:
    bash
    git clone https://github.com/yourusername/tamil-nadu-scheme-connect.git
    cd tamil-nadu-scheme-connect
    

2. *Set Up Environment*:
    - Create a virtual environment (optional but recommended):
      bash
      python -m venv venv
      source venv/bin/activate  # On Windows use `venv\Scripts\activate`
      
    - Install dependencies:
      bash
      pip install -r requirements.txt
      

3. *Environment Variables*:
    - Create a .env file in the project root directory and add necessary environment variables for API keys and other configurations.

## Usage

1. *Run the Streamlit App*:
    bash
    streamlit run app.py
    

2. *Access the Application*:
    - Open a web browser and navigate to http://localhost:8501 to interact with the application.

## How It Works

1. *Document Indexing*:
    - The application loads and indexes documents from the ./hack4 directory.
    - Uses a sentence splitter to create nodes and a vector store index for document retrieval.
    - Persists the index in the ./index_store_dev/vector directory for future use.

2. *Query Processing*:
    - Queries from users are processed by the OpenAIAgent, which uses a vector query engine to provide detailed responses based on indexed documents.
    - Retrieves additional information from Tamil Nadu government websites using the TavilySearchAPIRetriever.

3. *User Interaction*:
    - Users can input queries into the Streamlit app.
    - The application displays responses based on the indexed documents and additional retrieved sources.

## File Structure

- app.py: Main Streamlit application file.
- ./hack4/: Directory containing PDF documents for indexing which has not been added here due to proprietary data.
- ./index_store_dev/: Directory for storing the vector indexas the vector.zip.
- .env: (Optional) File for environment variables.
- requirements.txt: File listing the dependencies.

## Dependencies

- streamlit: For building the web application interface.
- nest_asyncio: For handling asynchronous operations.
- langchain_community: For API retrieval and document processing.
- llama_index: For document indexing and query processing.
- dotenv: For managing environment variables.

## Contributing

1. *Fork the Repository*: Create a personal copy of the repository.
2. *Create a Feature Branch*: Branch off from main for your changes.
3. *Commit Your Changes*: Include clear, descriptive commit messages.
4. *Submit a Pull Request*: Provide a detailed description of your changes.

## License

This project is licensed under the MIT License.

## Contact

For any questions or issues, please reach out to sansitakarthik2005@gmail.com, karthikapanchu2004@gmail.com, lakshanikasekhar.pro@gmail.com, vaadhishree@gmail.com.

---

Thank you for using Tamil Nadu Scheme Connect!
