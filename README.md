
# Real-Time Chat Application

This project is a real-time chat application that leverages Natural Language Processing (NLP) to understand and respond to user queries instantly. Built with Streamlit, the application provides an interactive web interface to ensure seamless and dynamic communication.

## Features

- **Real-Time Processing**: Utilizes NLP to handle and respond to user queries instantly.
- **Interactive Interface**: Built with Streamlit for a user-friendly and engaging chat experience.
- **Conversation History**: Stores and displays past conversations.
- **Modular Design**: Easy to extend and customize.

## Requirements

- Python 3.x
- Required Libraries: Listed in `requirements.txt`

## Installation

1. **Clone the repository**:
   ```sh
   git clone (https://github.com/BADUGU-SRICHETAN/real-time-chat-application)
   cd real-time-chat-application
Create and activate a virtual environment:

sh
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required libraries:

sh
pip install -r requirements.txt
Download NLTK data:

sh
python -c "import nltk; nltk.download('punkt')"
Running the Application
Start the Streamlit application:

sh
streamlit run app.py
Open your browser and navigate to:

http://192.168.0.13:8501
Project Structure
app.py: Main application file containing the Streamlit app logic.

intents.json: JSON file containing the intents and patterns for the chatbot.

requirements.txt: File listing all required libraries.

Dataset
The dataset used in this project consists of labeled intents and entities, stored in a structured list:

Intents: Represents the user's real-time query or goal (e.g., "greeting", "goodbye", "ask for help").

Entities: Key details extracted from the user’s input (e.g., "What is the current weather?", "Tell me a joke", "Recommend a book").

Text: The user’s input text seeking information or interaction in the real-time chat application.

How It Works
Load Intents: The intents are loaded from a JSON file.

Preprocess Data: The data is preprocessed using TF-IDF vectorization.

Train Model: A Logistic Regression model is trained on the intents and patterns.

Chatbot Function: The chatbot function predicts the intent and returns a relevant response.

Streamlit Interface: Provides an interactive web interface for user interaction.

Usage
Home Menu
Type your query in the input box to start chatting with the chatbot.

The chatbot will respond to your query in real-time.

Conversation History
View the history of all past conversations in a collapsible expander.

About
Learn about the project, its structure, and future enhancements.

Future Work
Expand the dataset with more intents and patterns.

Incorporate advanced NLP and deep learning techniques to enhance capabilities.

Add more interactive and user-friendly features to the Streamlit interface.
