# Generative AI ChatBot

## Overview
The ChatBot leverages generative AI models along with RAG techniques to interact with users and provide responses based on content retrieved from provided PDFs. The bot is capable of understanding user queries, retrieving relevant information from the documents, and generating responses that are both informative and contextually accurate. Additionally, it mentions the source of the response, specifying the PDF and the page from which the information was retrieved.

## Libraries Used
gradio
PyPDF2
faiss
numpy
sentence_transformers
google.generativeai
openai
GTTS
temp_file
speech_recognition
## Workflow
Load Model: The model is loaded using an API key.
Read PDF: The PDF content is read and processed.
Chunk Text: The extracted text from the PDF is divided into smaller chunks to accommodate model input token limitations and to handle large documents effectively.
Encode Passages: The text passages are encoded into vectors using Sentence Transformers.
Create FAISS Index: A FAISS index is created for efficient passage retrieval.
Retrieve Passages: Based on the user's query, relevant passages are retrieved from the index.
Generate Responses: The bot generates answers based on the retrieved passages.
Source Mention: The bot mentions the source of its response, including the PDF name and page number.
Host on Gradio: The application is hosted using Gradio for easy interaction.
Requirements

## Clone the Repository:
git clone https://github.com/majidhanif230/Chatbot_With_RAG

## Install Dependencies:
pip install -r requirements.txt
## Run the Notebook:
Open the Chatbot_RAG.ipynb notebook and run the cells sequentially.

## Access the ChatBot:
The ChatBot can be accessed via the Gradio interface provided in the notebook.

## Acknowledgments
This project was completed by Majid Hanif as part of an assignment given by Machine Learning 1 Pvt Ltd.
