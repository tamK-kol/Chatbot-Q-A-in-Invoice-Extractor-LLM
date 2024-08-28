## Documentation for Chatbot Q&A in Invoice Extractor
=====================================

### Overview
This project is a Streamlit application that uses Google's Gemini Pro Vision model to extract and analyze information from invoice images. The application allows users to upload an invoice image and enter a text prompt to receive responses based on the content of the invoice.

### Features
1. Upload an invoice image (JPG, JPEG, PNG formats).
2. Input a prompt related to the invoice.
3. Receive responses from the Gemini Pro Vision model based on the image and prompt.

### Requirements
1. Python 3.x
2. Streamlit
3. Pillow (PIL)
4. google.generativeai (for Gemini Pro Vision)

### Installation
1. Install the required packages:

pip install streamlit pillow google-generativeai python-dotenv

2. Set up environment variables
Create a .env file in the project root directory and add your Google API key:
GOOGLE_API_KEY=your_google_api_key

### Usage
1. Run the Streamlit app:
streamlit run app.py

2. Interact with the app:
* Upload an Invoice Image: Click on "Choose an image of the invoice" and select an image file.
* Enter a Prompt: Provide a text prompt for querying the invoice content.
* Submit: Click the "Tell me about the invoice" button to receive a response.

### Code Overview
* from dotenv import load_dotenv: Loads environment variables from a .env file.
* import streamlit as st: Imports the Streamlit library for creating the web app interface.
* import os: Imports the os module for environment variable management.
* from PIL import Image: Imports the PIL library for image handling.
* import google.generativeai as genai: Imports the Google Generative AI library for accessing the gemini-1.5-flash model.

### Key Functions
1. get_gemini_response(input, image, prompt): Generates a response from the Gemini-1.5-flash model based on the input prompt and uploaded image.

2. input_image_setup(uploaded_file): Processes the uploaded image file and prepares it for analysis.

### Streamlit App Initialization
1. st.set_page_config(page_title = "Tamal's Invoice Extractor"): Configures the Streamlit app's page title.
2. st.header("Tamal's Invoice Extractor"): Displays the main header of the app.
3. st.text_input("Input Prompt: ", key="input"): Provides a text input for the user to enter a prompt.
4. st.file_uploader("Choose an image of the invoice", type=["jpg", "jpeg", "png"]): Allows users to upload an invoice image.
5. st.button("Tell me about the invoice"): A button to submit the prompt and image for processing.

### Error Handling
* File Upload Error: If no file is uploaded, a 'FileNotFoundError' will be raised.

### Acknowledgements
* Google Generative AI for providing the Gemini Pro Vision model.
* Streamlit for the app development framework.

### License
This project is licensed under the GNU License. See the LICENSE file for details.

=====================================
Feel free to customize the details according to your needs!