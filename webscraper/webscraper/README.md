# Dynamic Document Generator

This web application uses Gemini AI to dynamically format text based on an existing document template. It allows users to paste text content, which is then processed by Gemini AI to generate a formatted document in both DOCX and PDF formats.

## Features

- Web interface for inputting text content
- Integration with Google's Gemini AI for document formatting
- Automatic generation of formatted DOCX and PDF documents
- Download options for the generated documents
- Display of the generated Python code

## Setup

1. Clone this repository
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Set up your Google API key:
   ```
   # On Windows
   set GOOGLE_API_KEY=your_api_key_here
   
   # On Linux/Mac
   export GOOGLE_API_KEY=your_api_key_here
   ```
4. Run the application:
   ```
   python app.py
   ```
5. Open your browser and navigate to `http://localhost:5000`

## Requirements

- Python 3.7+
- Flask
- Google Generative AI Python SDK
- python-docx
- docx2pdf (requires Microsoft Word or LibreOffice to be installed)

## How It Works

1. The user pastes text content into the web interface
2. The application sends the text and the original document template to Gemini AI
3. Gemini AI generates an updated version of the document code with the new content
4. The application executes the updated code to generate formatted documents
5. The user can download the generated documents in DOCX and PDF formats

## Note

This application requires a valid Google API key with access to the Gemini API. You can obtain one from the [Google AI Studio](https://makersuite.google.com/app/apikey).
