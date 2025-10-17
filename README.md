# Multimodal-Data-Processing-System
A system to process multimodal files (text, images, audio) and answer natural language queries using Gemini.
​1. Project Title and a Short Pitch
​Title: Multimodal Data Processing System.
​    "A Retrieval-Augmented Generation (RAG) system built with Python and Google's Gemini to process documents, images, and videos, allowing users to ask questions in natural language."
​2. Key Features
​Multimodal Input: Supports various file types (.pdf, .docx, .pptx, .txt, .png, .jpg, .mp3, .mp4).
​YouTube Video Processing: Ingests and processes information directly from YouTube links. 
​Intelligent Data Extraction: Uses specific models for each data type (text extraction for documents, vision models for images, speech-to-text for audio/video).
​Natural Language Q&A: Leverages the Gemini LLM to provide conversational and accurate answers based on the uploaded content.
​Interactive UI: A simple and intuitive web interface built with Streamlit.
​3. System Architecture
​Ingestion Pipeline: File Upload → Data Extraction → Text Chunking → Embedding → Vector Database Storage
​Query Pipeline: User Question → Embedding → Vector Search → Context Retrieval → Prompt Augmentation → Gemini LLM → Answer
​4. Tech Stack
​Language: Python 3.10+
​LLM & Embeddings: Google Gemini Pro, Gemini Pro Vision, Google Text Embeddings
​Vector Database: ChromaDB
​UI: Streamlit
​Data Processing: PyPDF2, python-docx, Pillow, OpenAI Whisper
​5. Setup & Installation (Crucial Section)
  5.1 Clone the repository
       git clone https://github.com/your-username/your-repository-name.git
       cd repository-name
  5.2 Create a virtual environment
       python -m venv venv
       source venv/bin/activate  # On Windows: venv\Scripts\activate
  5.3 Install dependencies
        pip install -r requirements.txt
  5.4 Set up environment variables:
        create a file named .env in the root directory.
        add your Google Gemini API key to it:
            GOOGLE_API_KEY="your-api-key-here"
  5.5 How to run the application
        streamlit run app.py
Open your web browser and go to http://localhost:8501 to use the application
6. Project Overview
   This project is a comprehensive solution designed to handle and interpret multimodal data input. It extracts relevant information from various file formats, stores it in a searchable knowledge base, and uses a Large Language Modal(LLM) to answer user queries based on the provided context.

