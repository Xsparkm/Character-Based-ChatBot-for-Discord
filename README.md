# Character-Based Discord Chatbot

This is a character-based chatbot designed for Discord. It leverages a JSON file as a knowledge base to provide responses to user queries, making it highly customizable for different characters.

## Features

- Responds to user queries based on a predefined knowledge base.
- Uses the `difflib` library to find the closest match for user questions.
- Asynchronous file operations with `aiofiles` for efficient file handling.
- Simple to set up and customize.

## Prerequisites

- Python 3.8+
- `discord.py` library
- `aiofiles` library
- `python-dotenv` library

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Xsparkm/Character-Based-ChatBot-for-Discord.git
    cd character-based-chatbot
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the project directory and add your Discord bot token:
    ```env
    TOKEN=your_discord_bot_token
    ```

5. Create a JSON knowledge base file (`knowledge_base.json`) with the following structure:
    ```json
    {
        "questions": [
            {
                "question": "How are you?",
                "answer": "I'm just a bot, but I'm here to help you."
            },
            {
                "question": "What's your name?",
                "answer": "I am your friendly character-based bot!"
            }
            // Add more questions and answers as needed
        ]
    }
    ```

## Usage

Run the bot with the following command:
```bash
python bot.py
