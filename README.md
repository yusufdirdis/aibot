# AI Document Assistant – AI Integration Mini Lab
## Overview

This project is a Streamlit-based AI chatbot that allows users to upload a document and ask questions about its contents. The application uses the Google Gemini API to analyze the uploaded file and generate answers based on the information contained in the document.

The chatbot is designed to only answer questions using the uploaded document. If the answer is not found in the document, the system responds that it does not know.

This project demonstrates how AI models can be integrated into a simple application using APIs, while also highlighting responsible AI practices.

## Features

Upload PDF or TXT documents

Ask questions about the document

AI generates responses using document context

Interactive chat interface

Built with Streamlit and the Google Gemini API

## Technologies Used

Python

Streamlit

Google Gemini API

python-dotenv

Google GenAI SDK

## Model Name and Source

This application uses Google Gemini 2.0 Flash, a large language model developed by Google.

The model is accessed through the Google Gemini API using the google-genai Python SDK.

Gemini models are capable of understanding natural language and analyzing documents, making them well suited for building conversational AI applications.

## Rationale for Model Selection

Gemini 2.0 Flash was selected because it is optimized for speed and efficiency while still providing strong natural language understanding. It supports document-based reasoning and conversational interactions, which makes it ideal for building a simple AI document assistant.

Using the Gemini API also allows developers to integrate powerful AI capabilities without needing to train their own models.

How the Application Works

The user uploads a document (PDF or TXT).

The document is sent to the Gemini Files API.

The system creates a chat session with the Gemini model.

The user enters a question in the chat interface.

The question and document reference are sent to the AI model.

Gemini generates a response using the document as context.

If the answer cannot be found in the document, the chatbot responds that it does not know.

# Installation
1. Clone the Repository
git clone https://github.com/yourusername/ai-document-assistant.git
cd ai-document-assistant
2. Install Dependencies
pip install streamlit
pip install google-genai
pip install python-dotenv

Or install everything with:

pip install -r requirements.txt
Environment Variables

Create a .env file in the project directory and add your Google Gemini API key:

GOOGLE_API_KEY=your_api_key_here

You can obtain a Gemini API key from:

https://ai.google.dev/

## Running the Application

Run the Streamlit application with the following command:

streamlit run aibot.py

Once the application starts, it will open in your browser.

## Steps to use the app:

Upload a PDF or TXT document.

Wait for the document to upload.

Ask questions about the document in the chat box.

The AI will generate answers based on the uploaded file.
