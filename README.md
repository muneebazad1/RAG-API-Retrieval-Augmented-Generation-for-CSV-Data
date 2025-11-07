Project Title:
RAG-based CSV Data Analysis Helper APIs

Description:
RAG-based CSV Data Analysis Helper APIs is a lightweight backend service designed to bring Retrieval-Augmented Generation (RAG) capabilities to CSV datasets.
It allows users to upload CSV files, automatically embed and index their content using HuggingFace embeddings, and ask natural language questions to extract insights.
The system uses FastAPI for serving endpoints, LangChain for building the RAG logic, Chroma Cloud for storing vector embeddings, and Google Gemini models for generating intelligent answers.

The API helps bridge structured CSV data with conversational AI, allowing users to query data semantically instead of using SQL or manual filtering.
It retrieves relevant chunks of information from the embedded dataset, then uses the language model to generate accurate and grounded responses.
This project is ideal for developers, analysts, and researchers looking to build intelligent data interfaces or prototype RAG-based tools.

Core Features:

Upload any CSV file and automatically embed it in Chroma Cloud.

Query data using natural language instead of database queries.

Powered by FastAPI for fast and simple API creation.

Integrates LangChain for RAG pipeline management.

Uses HuggingFace embeddings and Google Gemini for context-aware reasoning.

Automatically switches active datasets after uploads.

Setup and Installation:
Step 1: Clone the repository
bash
git clone https://github.com/muneebazad1/RAG-based-CSV-Data-Analysis-Helper-APIs.git


Step 2: Install dependencies
bash
pip install -r requirements.txt

Step 3: Run the API
bash
uvicorn main2:app --reload

The server will start at http://127.0.0.1:8000


How to Use:

Upload your CSV file using the /upload_csv endpoint from Swagger UI (/docs).

file: choose your CSV file

collection_name: provide a name for your dataset
The system will create and index a new Chroma Cloud collection.

Ask questions using the /ask endpoint with a JSON body.
Example request:
bash
{
"query": "What is the total number of entries for category A?"
}

The API will retrieve relevant data from the vector store and generate a meaningful answer.

Environment Configuration:
You must set your API keys in config.py or in an environment file as follows:
bash
LANGSMITH_API_KEY=your_langsmith_key
GOOGLE_API_KEY=your_google_gemini_key
CHROMA_CLOUD_API_KEY=your_chroma_key

Summary:
This project demonstrates how to combine semantic retrieval and generative AI to interact with CSV data.
It provides a practical example of how Retrieval-Augmented Generation can be used for data analysis, exploration, and intelligent query systems.
RAG-based CSV Data Analysis Helper APIs offers a flexible foundation for building data-aware assistants, analytics tools, or AI-driven backend services.
