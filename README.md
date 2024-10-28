# ChatBot
An AI-powered chatbot for precise Q&amp;A over local documents, supporting PDF files with accurate, context-aware responses.

# Chat with Multiple PDFs :books:

This project is a Streamlit-based application that allows users to chat with content extracted from multiple PDF documents. It uses OpenAI's GPT model or HuggingFace language models, FAISS for vector storage, and LangChain for managing conversational retrieval.

## Features
- Upload multiple PDF files
- Extract text and split into manageable chunks
- Embed text and perform conversational retrieval with either OpenAI or HuggingFace language models
- Maintain a chat history within the same session

## Requirements
- [OpenAI API Key](https://platform.openai.com/signup) or [HuggingFace API Key](https://huggingface.co/join)
- Python packages listed in `requirements.txt`

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   cd your-repository-name
   ```

2. **Install the required packages**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the OpenAI API key**:
   - Go to [OpenAI](https://platform.openai.com/account/api-keys) and create an API key.
   - Create a new file named `.env` in the project directory and add your OpenAI API key:
     ```bash
     OPENAI_API_KEY=your_openai_api_key_here
     ```
   - (Optional) If you want to use HuggingFace models instead, include your HuggingFace API key and configure the model accordingly in the code.

4. **Run the Streamlit app**:
   ```bash
   streamlit run chatbot.py
   ```

## Usage

- **Upload PDF Files**: Use the sidebar to upload one or multiple PDF documents.
- **Ask Questions**: Type a question related to your documents in the text box, and the bot will respond based on the content of your uploaded PDFs.
  
## Customization

You can choose between OpenAI and HuggingFace models by commenting/uncommenting the respective lines in the code for embeddings and language models.

---