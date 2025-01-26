# Yoga-Disha-Sendhil-Kumar-Assessment-Task
Software Engineer Assessment Task

Description
This project provides a Python script to convert markdown-formatted meeting notes into a well-structured Google Document using the Google Docs API. It automates the process of formatting the markdown content with appropriate headings, bullet points, and checkboxes while preserving the structure of the document.

The code is designed to run on Google Colab and utilizes Google Docs API to create a new document, apply markdown formatting, and insert content like attendees, agenda, action items, and next steps.

Features
Converts markdown meeting notes to a Google Doc.
Automatically applies the correct heading and paragraph styles.
Adds checkboxes to action items for task tracking.
Can be run seamlessly within a Google Colab environment.

Setup Instructions
1. Set Up Google Cloud Project
To use this script, you will need to enable the Google Docs API and create credentials in the Google Cloud Console.
Go to Google Cloud Console.
Create a new project.
Enable Google Docs API and Google Drive API for the project.
Create OAuth 2.0 credentials and download the JSON file for authentication.

2. Install Required Dependencies
Run the following command in a Google Colab cell to install the necessary libraries:
!pip install google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client

3. Authenticate and Set Up Credentials
The script will require user authentication to interact with the Google Docs API. Follow these steps:
Use auth.authenticate_user() to authenticate your Google account.
The script checks for existing credentials stored in token.pickle. If no token exists, you'll be prompted to authenticate.
If the credentials are expired, they will be refreshed automatically.

4. Run the Script in Colab
Once the authentication is complete, the script will:
Create a new Google Doc.
Convert markdown content into the Google Doc format.
Add headings, bullet points, and checkboxes.
Insert meeting notes into the document.

5. Modify the Markdown Content
You can modify the markdown_content variable with your meeting notes or any other markdown content you wish to convert into a Google Doc. Update the markdown content as necessary before running the script.

Required Dependencies-
google-auth: Authentication for Google APIs.
google-auth-oauthlib: OAuth 2.0 authentication for Google APIs.
google-auth-httplib2: HTTP handling for Google authentication.
google-api-python-client: Client library for interacting with Google Docs API.
pickle: For storing and loading authentication tokens.
google.colab: For Colab-specific integration.

How to Run in Colab-
Open the provided Google Colab notebook.
Authenticate with your Google account by running the authentication cells.
Execute the code cells in sequence
The code will first authenticate and check for existing credentials.
The markdown content will be converted and inserted into a new Google Doc.
The document will be formatted according to your markdown structure (headings, bullet points, etc.).
The Google Doc ID will be printed, confirming successful creation.
