RAG-based CSV Data Analysis Helper APIs is a lightweight and modular backend service that brings Retrieval-Augmented Generation (RAG) capabilities to your local CSV datasets.

Built with FastAPI, LangChain, and Chroma Cloud, it allows users to:

Upload CSV files,

Automatically embed and index their content using HuggingFace embeddings, and

Ask natural language questions to extract insights — powered by Google Gemini models.

The system bridges structured CSV data and conversational AI, enabling semantic querying without needing SQL or manual filtering. It uses semantic retrieval to find relevant chunks of data, then passes them to a large language model for accurate, grounded, and explainable answers.

Whether you’re building a data analysis assistant, automating reporting, or prototyping RAG applications, this project provides a clean foundation to start from.

⚙️ Core Features

📂 Upload any CSV file and auto-index it in Chroma Cloud

🧠 Ask natural language questions about CSV contents

🚀 Powered by FastAPI for high-performance APIs

🧩 Uses LangChain to connect vector retrieval and LLM reasoning

☁️ Persistent Chroma Cloud vector storage for reusability

🔄 Automatically switches active dataset after upload

🛠️ Setup & Installation
1. Clone the repository
