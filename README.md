# My Chatbot

### Description
This is an AI-powered chatbot built using Streamlit, FAISS, and Google's Gemini model. The chatbot acts as a replica of Me, answering questions based on a provided dataset and refining responses using the Gemini AI model.

### Features
- Mimics My responses based on a dataset.

- Uses FAISS for efficient semantic search.

- Integrates Google Gemini for enhanced response generation.

- Provides a chat interface with a customized UI.

- Retrieves answers from a CSV dataset containing questions and answers.

- Supports embeddings using the SentenceTransformer model.

### Installation
### Prerequisites

Ensure you have Python 3.8 or later installed on your system. You also need to install the required Python packages.
### Setup Instructions

1. Clone this repository or download the source code.

2. Install the required dependencies by running:
   ```sh
   pip install streamlit pandas google-generativeai sentence-transformers faiss-cpu numpy
3. Place your dataset file (my_data.csv) in an accessible location.

4. Update the file path in the load_data() function if needed.

### Usage

1. Run the chatbot application using:
   ```sh
   streamlit run my_chatbot.py
2. The chatbot will load and allow users to ask questions.

3. The system searches for the most relevant answer in the dataset and refines it using the Gemini AI model.
4. Responses are displayed in a friendly and engaging format.

### File Structure
    ```sh
    .
    ├── my_chatbot.py          # Main script for running the chatbot
    ├── my_data.csv         # Dataset containing questions and answers
    ├── README.md           # Project documentation
### Configuration

- Modify the dataset path inside load_data() to match your file location.

- Replace the api_key in genai.configure(api_key="YOUR_API_KEY") with your Google Gemini API key.

### Troubleshooting

1. If the chatbot fails to load, ensure that my_data.csv exists and contains question and answer columns.

2. If Streamlit fails to start, verify that all dependencies are correctly installed.

### Future Enhancements

- Add support for multiple answer retrieval.

- Improve UI with additional customization options.

- Implement memory for contextual conversations.
   
   
