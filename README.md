### MediGuru — Multilingual AI Medical Assistant using LLM and Retrieval-Augmented Generation

---

### Overview

MediGuru is an AI-powered multilingual medical assistant designed to improve accessibility and understanding of healthcare information. The system enables users to upload medical documents and ask questions in multiple languages. It also supports real-time web-based medical knowledge retrieval. The application integrates Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), vector search, and multilingual natural language processing to deliver accurate and context-aware responses.

The goal of MediGuru is to assist users in interpreting medical information and reduce misinformation by combining document understanding with real-time search capabilities.

---

### Features

* Multilingual medical query support
* Automatic language detection and translation
* Question answering from uploaded medical PDF documents
* Retrieval-Augmented Generation for improved accuracy
* Real-time web search for up-to-date medical knowledge
* Context-aware and personalized responses
* Interactive chat-based user interface
* Lightweight and scalable architecture
* Easy deployment using cloud or notebook environments

---

### System Architecture

The system consists of the following modules:

1. User Interface
   A chat-based interface built with Streamlit that allows users to upload documents and interact with the assistant.

2. Multilingual Processing
   The system detects the language of the query and translates it into English for processing. The final response is translated back to the user’s language.

3. Document Retrieval and RAG
   Uploaded PDFs are processed and converted into vector embeddings. Relevant content is retrieved using a FAISS vector database.

4. Large Language Model
   Google Gemini is used to generate accurate and context-aware responses.

5. Web Search Agent
   If document-based information is not sufficient, the system performs real-time web search using DuckDuckGo.

---

### Technology Stack

* Programming Language: Python
* User Interface: Streamlit
* LLM: Google Gemini
* Framework: LangChain
* Vector Database: FAISS
* Embeddings: HuggingFace multilingual sentence transformers
* Translation: Deep Translator
* Language Detection: LangDetect
* Web Search: DuckDuckGo
* Deployment: Ngrok, cloud or notebook environments

---

### Installation and Setup

#### Step 1: Clone the Repository

```
git clone https://github.com/your-username/mediguru.git
cd mediguru
```

#### Step 2: Install Dependencies

```
pip install streamlit faiss-cpu pypdf python-dotenv google-generativeai \
langchain langchain-google-genai langdetect deep-translator \
sentence-transformers pyngrok ddgs
```

#### Step 3: Set Google API Key

Create an environment variable:

```
export GOOGLE_API_KEY="your_api_key"
```

or in Windows:

```
set GOOGLE_API_KEY=your_api_key
```

---

### Running the Application

```
streamlit run app.py
```

The application will start locally and can be accessed in the browser.

---

### Usage

1. Upload a medical PDF file.
2. Ask a question related to the document.
3. The system retrieves relevant information and generates an answer.
4. Alternatively, switch to web search mode for real-time medical queries.
5. The system supports queries in multiple languages.

---

### Advantages

* Improves access to healthcare information
* Reduces misinformation through document-grounded responses
* Supports multilingual users
* Enables personalized medical document understanding
* Provides real-time updated medical insights

---

### Limitations

* The system is not a substitute for professional medical advice
* Accuracy depends on the quality of uploaded documents
* Web search results depend on external sources
* Requires internet connectivity

---

### Future Enhancements

* Voice-based medical assistant
* Medical image analysis (X-rays and scans)
* Integration with Electronic Health Records
* Personalized health monitoring
* Secure cloud-based deployment
* Telemedicine and doctor consultation integration

---

### Disclaimer

This application is intended for informational and educational purposes only. It does not provide medical diagnosis or treatment recommendations. Users should consult qualified healthcare professionals for medical advice.

