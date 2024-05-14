# AI PDF CHAT

## Description

This is a chat application in which you can upload a PDF document and the AI will scan it so that you can then ask questions related to the document. The model used in the analysis of the information is Google's Gemini 1.0 Pro.

### Stack

- Python
- Langchain
- Streamlit

## Setup

First of all you must clone the repository:

```sh
git clone https://github.com/jezbravo/pdf-chat.git
cd django-chatbot
```

Create a virtual environment to install dependencies in and activate it:

```python
python.exe -m venv venv
.\venv\Scripts\activate
```

Then install the dependencies:

```python
(venv)pip install -r requirements.txt
```

Note the `(venv)` in front of the prompt. This indicates that this terminal session operates in a virtual environment set up by "venv".

### Environment Variables

In order for the program to work correctly, it is necessary to configure the following environment variable in an .env file at the root of the project:

```python
GOOGLE_API_KEY=
```

This key is provided by the Google Gemini API service.

Once everything is ready:

```python
(venv)streamlit run .\app.py
```

## Demo

A PDF file can be uploaded by pressing the "Browse files" button in the sidebar. It is worth mentioning that the maximum size that the file can have is 200 MB. Then press the "Submit & Process" button and wait a few seconds for the application to scan the document. Once the "Done" notice appears, the form on the main screen will be ready to begin receiving questions related to the recently uploaded file.

You can test a deployed version at the following link: https://jezbravo-pdf-chat.streamlit.app
