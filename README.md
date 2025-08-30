
# Q&A System with Gemini and LlamaIndex

This is a Question Answering (Q&A) system based on documents using **Google Gemini** and **LlamaIndex**. It allows users to upload documents and ask questions related to the content of the uploaded document. The system uses Gemini's natural language processing capabilities and LlamaIndex for efficient document querying and vector embeddings.

## Features

- **Document Upload**: Upload PDF documents for processing.
- **Ask Questions**: Users can ask questions related to the uploaded document.
- **Document Querying**: Uses Gemini for NLP and LlamaIndex for querying documents based on vector embeddings.
- **Error Handling**: Custom error handling and logging are included to track and manage exceptions.

## Tech Stack

- **LlamaIndex**: A Python library for indexing and querying documents using vector embeddings.
- **Gemini**: Google's NLP model used for embedding and processing the document's content.
- **Streamlit**: Used for building the web app interface for uploading documents and interacting with the system.
- **Python**: Main programming language for building the system.
- **dotenv**: For managing API keys securely.

## Installation

### Requirements

1. Python 3.x
2. Install the necessary libraries using pip:

```bash
pip install llama_index google-generativeai streamlit python-dotenv
```

### Setting up API Key

1. Create a `.env` file in the root directory of the project.
2. Add your **Google Gemini API Key** to the `.env` file:

```
GOOGLE_API_KEY=your_google_api_key
```

## Running the Application

1. Run the Streamlit app using the following command:

```bash
streamlit run App.py
```

2. Once the app is running, navigate to the provided URL in your browser.
3. Upload a PDF document using the file uploader.
4. Ask a question related to the document, and the system will respond based on the content of the document.

## File Structure

```plaintext
QASystem/
│
├── App.py                # Main Streamlit app file
├── data_ingestion.py     # Loads documents from the directory
├── embedding.py          # Handles embedding and querying documents
├── exception.py          # Custom exception handling
├── logger.py             # Logging setup
├── model_api.py          # Loads the Gemini model for NLP
├── .env                  # Environment file for API keys
└── requirements.txt      # Python dependencies
```

## Contributing

Feel free to fork this repository, make changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [LlamaIndex](https://llamaindex.ai/)
- [Google Gemini](https://cloud.google.com/generative-ai/)
- [Streamlit](https://streamlit.io/)
