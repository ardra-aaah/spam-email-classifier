# SpamMorph — AI-Powered Spam Email Classifier

**SpamMorph** is a hybrid spam email classifier that combines a machine learning model trained on the UCI Spambase dataset with OpenAI's GPT-4 to assess whether a message is spam or not.

## Features

- Accepts pasted text or uploaded `.txt` email files
- Predicts using both a machine learning model and GPT-4
- Displays model confidence and reasoning
- Web interface built with Streamlit

## File Overview

- `spam_app.py`: Main Streamlit application
- `spam_model.pkl`: Trained Random Forest model
- `requirements.txt`: Python dependencies
- `notebook.ipynb`: Optional notebook used to train and prepare the model

## How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/spam-morph.git
    cd spam-morph
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Launch the application:
    ```bash
    streamlit run spam_app.py
    ```

## OpenAI API Key

To use GPT-based predictions, set your OpenAI API key in your Python script:

```python
openai.api_key = "your-api-key-here"
