# 💬 Chit Chat with PDFs

## 🚀 Project Overview
This project enables users to chat with their PDF documents 📄 by asking questions. It uses **LangChain** and **Google Generative AI** to retrieve relevant content from the uploaded PDFs and generate answers based on them.

## 🔑 Key Components

- **📄 PDF Parsing**: The uploaded PDF files are read using `PyPDF2` to extract plain text.
- **📝 Text Splitting**: The extracted text is split into chunks using `RecursiveCharacterTextSplitter` to manage large documents efficiently.
- **📊 Embeddings & Vector Store**: The chunks are embedded using **Google Generative AI**, and stored in **FAISS** for fast similarity searches.
- **🤖 Conversational Chain**: The system retrieves relevant chunks and generates answers using **Google's Gemini-Pro** model. If no answer is found in the document, it responds accordingly.
- **🎨 Streamlit Interface**: Users can easily upload PDFs, ask questions, and receive answers via an intuitive **Streamlit** interface.

## ✨ Features
- ✅ Upload Multiple PDFs
- ✅ Smart Q&A based on PDF content
- ✅ Persistent FAISS Vector Store
- ✅ Simple User Interface with Streamlit

## 🔧 Technical Stack
- 🌐 **Streamlit**: User interface for uploading PDFs and interacting with the system.
- 📝 **PyPDF2**: Extracts text from PDF documents.
- 🧠 **LangChain**: Handles text chunking, embeddings, and QA chain.
- 🤖 **Google Generative AI**: Embeddings and conversational AI.
- ⚙️ **FAISS**: Efficient similarity search based on embeddings.
- 🔑 **dotenv**: Manages API keys securely.

## 🎯 Use Cases
With this project, users can query long PDF documents to find specific information. It's especially useful in:

- 📚 **Research Assistance**: Find information in academic papers or research reports quickly.
- ⚖️ **Legal Review**: Search through legal documents for relevant sections.
- 📝 **Document Search**: Query any lengthy document for specific answers.

## 🔐 API Key Configuration
Ensure to configure your `.env` file with your own **Google Generative AI API Key**:

```plaintext
GOOGLE_API_KEY=your_google_api_key
