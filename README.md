# Chat with Code

This application allows you to interact with your code files by asking questions and receiving answers. It leverages language models and vector stores to create a conversational interface where you can inquire about specific aspects of your code.

## Features

- **Upload Code Files:** Upload code files in various languages (Python, JavaScript, Java, C++, C, Ruby, Go, Rust, TypeScript) and interact with them.
- **Text Chunking:** Automatically splits the uploaded code into manageable text chunks for efficient processing.
- **Vector Store Creation:** Creates a vector store from the code chunks using FAISS and embeddings.
- **Conversational Interface:** Engage in a conversation about your code, either using the Google Palm API or running offline with Ollama.

## Getting Started

### Prerequisites

- Python 3.8 or later
- An environment that supports installing Python packages

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/Sahil-Bhoite/chat-with-code
   cd chat-with-code
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up your environment variable for the Google API key:

   ```bash
   export GOOGLE_API_KEY="your-google-api-key"
   ```

### Running the App

Run the Streamlit app:

```bash
streamlit run app.py
```

### Usage

1. Open the app in your web browser.
2. Upload your code file using the file uploader.
3. Use the text input to ask questions about your code.
4. Receive answers in real-time.

### Optional: Using Ollama Offline

If you prefer to run the application offline using Ollama:

- Enable the "Use Ollama (offline) instead of Google Palm" option in the sidebar.
- Ensure you have the Ollama model `llama2` set up.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

This project uses the following libraries:

- [LangChain](https://github.com/langchain-ai/langchain)
- [FAISS](https://github.com/facebookresearch/faiss)
- [Streamlit](https://github.com/streamlit/streamlit)
- [Google Palm](https://github.com/google)
- [Ollama](https://github.com/ollama)
