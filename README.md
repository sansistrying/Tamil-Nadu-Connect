# Tamil-Nadu-Scheme-Connect
"Tamil Nadu Scheme Connect" is a web application that provides detailed information about Tamil Nadu's services and schemes. It indexes official documents for efficient data retrieval and uses a chat interface to process user queries, ensuring accurate and relevant responses based on the official information from Tamil Nadu's government websites.

## Overview

The Tamil Nadu Scheme Connect is a web application built using Flask, JavaScript, CSS, and HTML, providing users with detailed information about government schemes and services available in Tamil Nadu. The app utilizes advanced document indexing, language translation, and query processing to deliver accurate and concise answers based on user queries.

## Features

- *Document Indexing:* Automatically indexes documents for efficient search and retrieval using a vector database.
- *Query Handling:* Processes user queries to extract relevant information from indexed documents.
- *Language Translation:* Supports Tamil, Hindi, and English to cater to a diverse user base.
- *Google API Integration:* Locates nearby NGOs, hospitals, and blood donation camps.
- *News API:* Retrieves news on topics like legal matters, women empowerment, and welfare.
- *Voice Input:* Allows users to interact with the chatbot using voice commands.

## How It Works

1. *Document Indexing*:
    - The application loads and indexes documents from the ./hack4 directory.
    - Uses a sentence splitter to create nodes and a vector store index for document retrieval.
    - Persists the index in the ./index_store_final/vector directory for future use.

2. *Query Processing*:
    - Queries from users are processed by the OpenAIAgent, which uses a vector query engine to provide detailed responses based on indexed documents.
    - Retrieves additional information from Tamil Nadu government websites using the TavilySearchAPIRetriever.

3. *Google API Integration:*:
    - Locates nearby NGOs, hospitals, and blood donation camps based on user queries

4. *NewsAPI*:
 - Fetches and displays news articles related to legal topics, women empowerment, welfare, and more.

5. *Language Translation:*:
   - Supports Tamil, Hindi, and English, allowing users to switch between languages seamlessly.
  
6. *Voice Input*:
   - Enables users to interact with the chatbot through voice commands for a more interactive experience.

## File Structure
- chatbot_app.py: Main flask application.
- app.py: Main Streamlit application file.
- ./hack4/: Directory containing PDF documents for indexing which has not been added here due to proprietary data.
- ./index_store_final/: Directory for storing the vector indexas the vector.zip.(in drive)
- venv: (Optional) File for environment variables.(in drive)
- requirements.txt: File listing the dependencies.
- Templates folder: chatbot.htnl, index.html, login.html, map.html, newsmain.html
- Scripts folder: mapscripts.js, mapstyles.css, newsscripts.js, newsstyles.css, scripts.js, styles.css


## Dependencies

- Flask: For building the web application backend.
- JavaScript, CSS, HTML: For frontend development.
- Google API: For locating nearby NGOs, hospitals, and blood donation camps.
- News API: For fetching news articles.
- langchain_community: For API retrieval and document processing.
- llama_index: For document indexing and query processing.
- dotenv: For managing environment variables.

## Additional Resources

For convenience, you can download the indexed documents (/index_store_final/) from the following Google Drive link: https://drive.google.com/drive/folders/1X5AOffQVnzLr7H-8lfTrlOQuKWxrTcjT?usp=sharing


## Contact

For any questions or issues, please reach out to sansitakarthik2005@gmail.com, karthikapanchu2004@gmail.com, lakshanikasekhar.pro@gmail.com, vaadhishree@gmail.com.

---

Thank you for using Tamil Nadu Scheme Connect!
