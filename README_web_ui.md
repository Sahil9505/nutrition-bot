# AI Culture Guide Chatbot - Web UI

This is a web-based interface for the Culture Guide Chatbot powered by Google's Gemini AI. The web interface allows you to interact with the chatbot through a modern, responsive UI.

## Features

- Modern, responsive chat interface
- Dark/light mode toggle
- Syntax highlighting for code snippets
- Markdown formatting support
- Typing indicators
- Chat history within the session

## Requirements

- Python 3.8 or higher
- Flask
- Google Generative AI Python SDK
- python-dotenv

## Installation

1. Make sure you have all the required packages installed:

```bash
pip install -r requirements.txt
```

2. Set up your environment variables by creating a `.env` file with your Google API key:

```
GOOGLE_API_KEY=your_google_api_key_here
```

## Running the Web UI

To start the web interface, run:

```bash
python web_chatbot_ui.py
```

Then open your browser and navigate to:

```
http://127.0.0.1:5000
```

## Usage

1. Type your culture-related question in the input field
2. Press Enter or click the Send button
3. The chatbot will process your question and provide a response
4. You can toggle between dark and light mode using the switch in the top right
5. Click "Clear Chat" to start a new conversation

## Limitations

- The chatbot is specifically focused on cultural topics
- Responses are generated using the Gemini 1.5 Flash model
- Internet connection is required

## Integration

This web UI is designed as a standalone component that can be integrated into other projects. The core functionality is separated from any existing desktop UI implementation.

# Using the Nutrition Facts Chatbot Web UI

This README provides instructions on how to use the web interface for the Nutrition Facts Chatbot.

## Getting Started

1. Make sure you have installed all the required dependencies:
   ```
   pip install -r requirements.txt
   ```

2. Ensure you have set up your API keys in the `.env` file:
   ```
   GOOGLE_API_KEY=your_google_api_key_here
   SPOONACULAR_API_KEY=your_spoonacular_api_key_here
   ```

## Setting Up Spoonacular API Key

1. Go to [Spoonacular API](https://spoonacular.com/food-api) and create a free account
2. After signing up and verifying your email, navigate to the Dashboard
3. Generate an API key from the dashboard
4. Copy the API key and paste it in your `.env` file:
   ```
   SPOONACULAR_API_KEY=your_spoonacular_api_key_here
   ```
5. The free plan includes 150 API calls per day which should be sufficient for testing

## Starting the Web Interface

1. Run the Flask application:
   ```
   python web_chatbot_ui.py
   ```

2. Open your web browser and navigate to:
   ```
   http://127.0.0.1:5002
   ```

## Using the Chatbot

1. The chat interface will appear with a welcome message
2. Type your nutrition or food-related questions in the input box
3. Press Enter or click the Send button to submit your question
4. The AI will respond with relevant nutritional information
5. Type "byee" to end the conversation

## Example Questions

You can ask questions like:

- "What are the nutritional benefits of kale?"
- "How many calories are in a cup of coffee?"
- "What's the protein content of quinoa?"
- "Is dark chocolate healthy?"
- "How much vitamin C is in an orange?"
- "What are the health benefits of avocados?"
- "Is oatmeal good for breakfast?"
- "How much sugar is in a banana?"
- "What nutrients are in almonds?"
- "What's the difference between white and brown rice nutritionally?"

## Troubleshooting

1. **API Key Issues**: If you see warnings about missing API keys, check that your `.env` file is correctly set up and that you've added the right keys.
2. **Connection Issues**: The Spoonacular API requires an internet connection to retrieve food nutrition data. 
3. **Rate Limiting**: The free tier of Spoonacular API has a limit on daily requests. If you exceed this limit, the API will return errors.

## Features

- **Enhanced Food Database**: With the Spoonacular API integration, the chatbot can now provide nutrition information on thousands of food items
- **Detailed Nutrition Facts**: Get comprehensive nutrition information about various foods
- **AI-Powered Responses**: The Google Gemini AI provides natural language understanding for a conversational experience
- **Responsive Design**: Works well on both desktop and mobile devices

## Need Help?

If you encounter any issues or have questions, please refer to the main README.md file or open an issue on the project's repository. 