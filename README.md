# 📄 Document QA Chatbot

Welcome to the Document QA Chatbot — an AI-powered assistant that allows you to upload a PDF file and ask questions based on its contents.  
It uses LangChain, Groq's LLaMA-3 model, and HuggingFace embeddings to perform intelligent document-based question answering.

------------------------------------------------------------

🧠 HOW IT WORKS

This app is powered by:
- LangChain: For chaining logic and document processing
- LangGraph (optional): Can be added for memory or multi-agent interaction
- Groq LLaMA-3: As the large language model for answering questions
- HuggingFace Embeddings: For semantic search
- Chroma: As the vector store for retrieving relevant document chunks
- Streamlit: For the frontend UI
- PyMuPDF: For reading PDF documents

------------------------------------------------------------

🚀 FEATURES

- Upload any PDF document
- Asks questions and gets accurate answers from the document
- Uses semantic chunking and vector-based retrieval
- Lightweight and blazing fast with Groq's low-latency models

------------------------------------------------------------

🔧 INSTALLATION

1. Clone the repository:

   git clone https://github.com/yourusername/document-qa-bot.git
   cd document-qa-bot

2. Create a virtual environment and activate it:

   python -m venv venv
   source venv/bin/activate       # On Windows: venv\Scripts\activate

3. Install dependencies:

   pip install -r requirements.txt

4. Set up environment variables:

   Create a `.env` file in the root folder and add:

   GROQ_API_KEY=your_groq_api_key_here

------------------------------------------------------------

▶️ RUN THE APP

   streamlit run streamlit_app.py

Once the app is running:

1. Upload a PDF file using the uploader.
2. Ask a question related to the contents of the document.
3. Receive an accurate, context-aware answer based only on your document.

------------------------------------------------------------

📂 FILE STRUCTURE

- `app.py` → Streamlit frontend
- `docQA.py` → PDF loader, text splitter, embedding, vector store, and QA logic
- `.env` → For storing your GROQ API Key
- `requirements.txt` → Dependencies list

------------------------------------------------------------

📦 requirements.txt

streamlit  
langchain  
langchain-groq  
langchain-community  
python-dotenv  
pymupdf  
chromadb

------------------------------------------------------------

💡 FUTURE IDEAS

- Support multiple PDFs or multi-file vector stores  
- Add citation to exact document pages  
- Add chatbot memory and threading using LangGraph  
- Use advanced chunking strategies (semantic / recursive)  
- Export Q&A pairs from the session

------------------------------------------------------------

🧠 Example Usage

1. Upload a contract or research paper.
2. Ask: “What are the key terms of the agreement?”
3. Bot will search relevant text chunks and answer with high accuracy.

------------------------------------------------------------

Built with using LangChain + Groq + Streamlit.
