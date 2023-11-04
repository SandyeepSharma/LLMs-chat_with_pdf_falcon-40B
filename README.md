# PDF Chatbot with Streamlit

This is a Python LLM uses FALCON-40B model that allows you to chat with a chatbot about the content of multiple PDF documents. The chatbot is powered by Hugging Face's language models and uses a conversational retrieval chain to provide responses to your questions.

## Prerequisites

Before running the application, ensure you have the following:

1. Python installed on your system.

2. Required dependencies. You can install them using the `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
     ```
3. Hugging Face API Token:
- Sign up for a Hugging Face account if you don't have one.
- Obtain your Hugging Face API token.
- Create a `.env` file in the project directory and set your API token as follows:
  ```
  HUGGINGFACEHUB_API_TOKEN=your_api_token_here
  ```

## Usage

1. Start the application by running `app.py` using Streamlit:

```bash
streamlit run app.py 
```
2. In the Streamlit web interface, you can:

- Ask questions about the content of your PDF documents.
- Upload multiple PDF files.
- Click the "Process" button to analyze the documents.

3. The chatbot will provide responses based on the content of the PDFs.

## How It Works
- The application uses the Hugging Face API and a large pre-trained language model (tiiuae/falcon-40b-instruct) to understand and respond to your questions.

- It processes the text from the uploaded PDF files, splits it into chunks, and stores it in a vector store.

- A conversational retrieval chain is set up to enable interaction with the chatbot. Your questions are processed and matched with the content of the PDFs to generate responses.

## Support and Issues
If you encounter any issues or have questions about this application, please feel free to connect on ```sandyeepofficial@gmail.com```.