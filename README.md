# Meeting Transcription and Summary Tool

This project is an AI-powered tool designed to automate the process of converting meeting audio into accurate text and generating concise summaries. It is built to assist users in tracking key points, decisions, and action items from meetings, making it a valuable tool for productivity and meeting management.

## Features

- **Real-time Transcription:** Upload audio or video files, and the tool will transcribe the content in real time using the AssemblyAI API.
- **NLP-Based Summarization:** Automatically generate summaries that extract main themes, key points, and action items using natural language processing (NLP).
- **Exportable Meeting Minutes:** Summarized notes and themes can be exported in PDF format, making it easy to share and store.

## Components
### `meeting_summary.py`
- Provides the user interface using Streamlit for uploading files and viewing transcriptions.
- Displays the main themes and summaries generated from the meeting content.
- Allows the user to export the summarized content in PDF format.

### `get_results.py`
- Handles communication with the AssemblyAI API for uploading audio files, processing them for transcription, and retrieving the meeting themes and summaries.

### `configure.py`
- This file holds your API key for AssemblyAI. Make sure to update the `auth_token` with your own API key.

## Requirements
- **Streamlit:** For building the web-based user interface.
- **AssemblyAI API:** For audio transcription and theme detection.
- **Pandas:** For handling and displaying chapter data.
- **PDFDocument:** For exporting the summarized meeting notes into a PDF format.

## How to Use
1. Upload a meeting audio or video file through the Streamlit interface.
2. View the generated main themes and summaries.
3. Export the meeting minutes in PDF format with a single click.

## Deployment Instructions
### Step 1: Install Dependencies
All the required dependencies are listed in the `requirements.txt` file. To install them, run the following command:

```bash
pip install -r requirements.txt
```

### Step 2: Get API Key from Assembly AI
- Create an account at [Assembly AI](https://www.assemblyai.com/).
- Copy your API key from the homepage.

### Step 3: Add API Key to `configure.py`
Paste the API key into the `configure.py` file as shown below:

```python
auth_token = "PASTE YOUR API KEY HERE"
 ```
 ### Step 4: Run the Application
Run the `meeting_summary.py` file using the Streamlit command

### Step 5: Open Localhost
A localhost server will automatically open in your browser. Use the interface to upload a meeting audio or video file.

### Step 6: Wait for Transcription and Summarization
After uploading the file, wait until the main themes and summaries are displayed on the screen.

### Step 7: Generate PDF
Click the "Generate PDF" button to export all the results into a PDF file named `meeting_summary.pdf`, which will be saved in the root directory.


