# Streamlit Chatbot Application with Groq API Integration

This project demonstrates a chatbot application built using **Streamlit** and integrated with the **Groq API** for generating chat completions.

## Features

- Accepts user input through a text field.
- Sends the input to the Groq API to generate a response using the `mixtral-8x7b-32768` model.
- Displays the chatbot's response in the app.
- Styled UI with CSS for enhanced user experience, including a background image and custom element alignments.

## Prerequisites

1. Python 3.7 or higher
2. Streamlit library
3. Groq API key

## Installation

1. Clone the repository:
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate # On Windows use `venv\Scripts\activate`
    ```

3. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Add your **Groq API Key** in the script:
    Replace the placeholder API key in the script with your actual Groq API key.
    ```python
    api_key=("your_actual_api_key")
    ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Access the app in your browser at `http://localhost:8501`.

3. Enter a message in the text input field and click the "Send" button to receive a chatbot response.

## File Structure

- `app.py`: Main script containing the Streamlit application.
- `requirements.txt`: List of dependencies for the project.

## Example Response

When you enter a message, the chatbot responds based on the input using the Groq API's `mixtral-8x7b-32768` model.

## Customization

### Background Image

To change the background image, replace the URL in the CSS section:
```css
background-image: url("your_image_url");
```

### Chatbot Model

To use a different model, update the `model` parameter in the `get_chat_completion` function:
```python
model="your_preferred_model"
```

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgements

- [Streamlit Documentation](https://docs.streamlit.io/)
- [Groq API Documentation](https://groq.com/docs)
