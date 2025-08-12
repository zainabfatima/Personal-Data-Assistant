🤖 Personal LLM Data Assistant
A personalized AI assistant that can read, understand, and answer questions about your own documents and datasets using Large Language Models (LLMs).
It combines LangChain, OpenAI GPT models, and vector databases to give you context-aware answers from your local data.

🚀 Features
📂 Document Ingestion – Upload PDFs, TXT, or CSV files for analysis.

🧹 Text Processing – Automatic text cleaning and chunking for better retrieval.

🧠 Vector Search – Store embeddings in a vector database for semantic search.

💬 LLM-Powered QA – Use GPT-based models to answer questions about your files.

🔍 Semantic Retrieval – Finds the most relevant text chunks for your query.

🌐 Streamlit Interface – Clean and interactive web-based UI.

📁 Project Structure
graphql
Copy
Edit
Personal-LLM-Data-Assistant/
├── app.py                        # Main Streamlit application
├── requirements.txt              # Python dependencies
├── utils.py                       # Helper functions (loading, chunking, embedding)
├── vectorstore/                   # Stores FAISS index files
├── data/                          # Folder for uploaded documents
└── README.md                      # Documentation
⚙ How It Works
Document Loading – Uses libraries like PyPDF2 and pandas to read files.

Chunking – Splits large documents into smaller overlapping chunks using LangChain’s RecursiveCharacterTextSplitter.

Embedding – Converts chunks into numerical vectors via OpenAIEmbeddings.

Vector Storage – Saves vectors in FAISS for fast semantic search.

Query Processing – When you ask a question, it:

Searches FAISS for the most relevant chunks

Sends them to GPT-3.5 or GPT-4

Returns a concise, context-based answer.

📤 Input
.pdf, .txt, .csv files containing your personal or project data.

📈 Output
Context-aware answers about your files.

Extracted insights and summaries.
