# RAG-Based Document Question Answering System 🤖📄

A powerful Retrieval-Augmented Generation (RAG) chatbot that enables users to upload PDF documents and ask intelligent questions based on their content. This system leverages advanced AI models to provide accurate, context-aware answers by retrieving and analyzing relevant document sections.

## 🚀 Features

- **PDF Document Processing**: Seamlessly extract and process text from uploaded PDF files
- **Intelligent Chunking**: Automatically split documents into optimal-sized chunks for better retrieval
- **Advanced Embeddings**: Utilize Cohere's state-of-the-art embedding models for semantic understanding
- **Scalable Vector Storage**: Employ Pinecone for efficient vector similarity search and storage
- **Contextual Q&A**: Generate precise answers using Cohere's language models with retrieved document context
- **Interactive Web Interface**: User-friendly Streamlit-based UI for easy document upload and querying
- **Real-time Chat History**: Maintain conversation context with persistent chat history
- **Reranking for Accuracy**: Implement document reranking to prioritize the most relevant information

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI/ML**: Cohere (embeddings, chat, reranking)
- **Vector Database**: Pinecone
- **PDF Processing**: PyMuPDF (Fitz)
- **Language**: Python 3.8+

## 📋 Prerequisites

- Python 3.8 or higher
- API keys for:
  - [Cohere](https://cohere.ai/) - For embeddings and language models
  - [Pinecone](https://pinecone.io/) - For vector storage and retrieval

## 🏗️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/RahulBuilt/RAG-based-DQAS.git
   cd RAG-based-DQAS
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 📂 GitHub Repository

- **Repository**: [RahulBuilt/RAG-based-DQAS](https://github.com/RahulBuilt/RAG-based-DQAS)
- **Issues**: [Report bugs or request features](https://github.com/RahulBuilt/RAG-based-DQAS/issues)
- **Pull Requests**: [Contribute to the project](https://github.com/RahulBuilt/RAG-based-DQAS/pulls)

## 🚀 Usage

1. **Obtain API Keys**
   - Sign up for Cohere and get your API key
   - Sign up for Pinecone and get your API key

2. **Run the application**
   ```bash
   cd src
   streamlit run app.py
   ```

3. **Access the web interface**
   - Open your browser and navigate to `http://localhost:8501`

4. **Use the chatbot**
   - Enter your Cohere and Pinecone API keys in the sidebar
   - Upload a PDF document
   - Ask questions about the document content
   - View responses and chat history

## 📁 Project Structure

```
├── LICENSE                 # Apache License
├── README.md              # Project documentation
├── requirements.txt       # Python dependencies
└── src/
    ├── app.py            # Main Streamlit application
    ├── chatbot.py        # Chatbot logic and response generation
    └── vectorstore.py    # PDF processing, embeddings, and vector operations
```

## 🔧 How It Works

1. **Document Processing**: PDF text is extracted and split into manageable chunks
2. **Embedding Generation**: Each chunk is converted to vector embeddings using Cohere
3. **Vector Indexing**: Embeddings are stored in Pinecone for efficient similarity search
4. **Query Processing**: User questions are embedded and used to retrieve relevant document chunks
5. **Response Generation**: Cohere's chat model generates answers using retrieved context
6. **Reranking**: Results are reranked for improved relevance and accuracy

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Cohere AI** for providing powerful language models and embeddings
- **Pinecone** for scalable vector database infrastructure
- **Streamlit** for the intuitive web application framework
- **PyMuPDF** for reliable PDF text extraction

## 🔮 Future Enhancements

- Support for multiple document formats (DOCX, TXT, etc.)
- Multi-language document processing
- Batch document upload and management
- Export functionality for chat history
- Integration with additional vector databases
- Cloud deployment options
- Advanced UI features (themes, export options)

---

**Note**: This project requires valid API keys for Cohere and Pinecone services. Ensure you have active accounts and sufficient API quotas for optimal performance.