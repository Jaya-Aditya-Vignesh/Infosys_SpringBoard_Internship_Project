# Medical Chatbot

A robust Medical Chatbot application built with **Streamlit**, **LangChain**, and **Pinecone**, designed to provide answers to medical questions based on user-provided datasets (PDFs, URLs, or default data). The chatbot uses advanced machine learning and language processing models to retrieve contextually accurate responses.

---

## Features

- **Interactive Chat Interface**: Users can ask medical-related questions and receive answers.
- **Multiple Data Source Options**:
  - Upload PDFs containing medical information.
  - Input URLs to extract medical content for analysis.
  - Use default medical data for general queries On Viruses.
- **Real-time Data Processing**: Automatic data chunking and vector storage for efficient retrieval.
- **Customizable Prompt Templates**: Ensures contextually accurate responses.
- **Chat History**: View past questions and answers for reference.

---

## Requirements

### Python Packages

The application relies on the following libraries:

```plaintext
streamlit~=1.41.1
langchain~=0.3.15
langchain-community~=0.3.13
python-dotenv~=0.21.0
pinecone~=5.4.2
langchain-core~=0.3.31
```

To install these dependencies, run:

```bash
pip install -r requirements.txt
```

### Environment Variables

Create a `.env` file in the root directory with the following keys:

```dotenv
GROQ_API=<Your_Groq_API_Key>
PINECONE_API_KEY=<Your_Pinecone_API_Key>
```

Replace `<Your_Groq_API_Key>` and `<Your_Pinecone_API_Key>` with your respective API keys.

---

## Usage

### 1. Clone the Repository

```bash
git clone <repository_url>
cd <repository_name>
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Application

```bash
streamlit run app.py
```

### 4. Interact with the Chatbot

- **Choose a Data Source**: Use the sidebar to select PDF, URL, or Default data.
- **Provide Data**:
  - Upload PDFs or input URLs for processing.
  - Default data will be used automatically if no data is uploaded.
- **Ask Questions**: Type your question in the input box and click **Get Answer**.
- **View Chat History**: Expand the "Chat History" section to review past interactions.

---

## File Structure

```plaintext
.
├── app.py                  # Main application code
├── functions.py            # Helper functions for data processing
├── requirements.txt        # Required Python libraries
├── .env                    # API keys and environment variables
├── Medical_PDF.pdf         #Default Dataset PDF          
└── README.md               # Documentation
```

---

## Technologies Used

- **Streamlit**: For building an interactive web app.
- **LangChain**: For retrieval-based question-answering.
- **Pinecone**: Vector database for efficient data retrieval.
- **HuggingFace Embeddings**: To convert text into numerical vectors.
- **PyPDFLoader**: For loading and parsing PDF documents.

---


## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgments

- [Streamlit Documentation](https://docs.streamlit.io/)
- [LangChain Documentation](https://python.langchain.com/)
- [Pinecone Documentation](https://docs.pinecone.io/)
- [HuggingFace](https://huggingface.co/)

---

