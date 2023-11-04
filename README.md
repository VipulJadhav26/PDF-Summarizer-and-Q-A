# Data Analyst Portfolio
by Vipul Jadhav

# [Project 1: PDF Summarizer powered by OpenAI LLM](https://github.com/VipulJadhav26/PDF-Summarizer-Q-A)
This is an app built using Streamlit web application that allows users to interact with a chatbot powered by the OpenAI LLM (Language Model) model.

1. It imports necessary Python libraries and modules, including Streamlit, dotenv, PyPDF2, LangChain, and OpenAI, to create the web application and perform various tasks.
2. In the sidebar of the web application, it provides some information about the app and its components, such as Streamlit, LangChain, and the OpenAI LLM model.
3. The main() function is defined, which is the main part of the application.
4. Inside the main() function, it loads environment variables from a .env file using load_dotenv().
5. It allows users to upload a PDF file using the Streamlit file_uploader widget and extracts text from the uploaded PDF.
6. It splits the extracted text into smaller "chunks" for processing.
7. It checks if embeddings (vector representations of text) have been precomputed and stored as a file. If not, it computes embeddings for the text chunks and saves them to a file.
8. Users can input questions about the content of the PDF using a text input field.
9. When a user submits a query, the code performs the following steps:
    * It searches for similar text chunks in the PDF based on the user's query using vector embeddings.
    * It sets up a language model chain using LangChain and the OpenAI LLM model.
    * It uses the chain to answer the user's question based on the retrieved text chunks.
    * It displays the response from the chatbot in the Streamlit app.

Overall, the code creates a web application for interacting with a chatbot that can answer questions about the content of a PDF document, and it leverages LangChain and OpenAI's LLM model for this purpose.
