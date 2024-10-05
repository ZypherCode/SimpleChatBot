# ZypherBot

ZypherBot is a simple conversational chatbot built using Python and the NLTK (Natural Language Toolkit) library. This bot can respond to basic questions and engage in casual conversation. It is a great starting point for anyone interested in learning about natural language processing (NLP) and creating simple bots.

## Features
- Responds to basic greetings and common questions.
- Uses pattern matching and predefined responses.
- Easily customizable with new conversation patterns.
- A great educational project for learning chatbot basics and NLP with Python.

## Requirements
Before running ZypherBot, you need to install the required dependencies:

- Python 3.x
- NLTK

To install NLTK, run:
```bash
pip install nltk
```

You also need to download the required NLTK resources:
```python
import nltk
nltk.download('punkt')
```

## Getting Started
To get started with ZypherBot, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ZypherBot.git
   cd ZypherBot
   ```

2. Run the bot:
   ```bash
   python main.py
   ```

3. Start chatting with ZypherBot! For example:
   - User: `Привет, бот!`
   - Bot: `Привет, пользователь! Как дела?`

## Customization
You can easily customize ZypherBot by adding new conversation patterns. The responses are defined using a list of pattern-response pairs, where the pattern is a regular expression and the response can include placeholders.

Example of a simple pair:
```python
pairs = [
    ['Привет (.*)', ['Привет, %1!', 'Здравствуйте, %1! Как дела?']],
]
```
- `Привет (.*)` matches any greeting that starts with "Привет", and the `(.*)` captures the rest of the input.
- `%1` is replaced with the captured group from the user's input.

Feel free to add more pairs to extend the bot’s capabilities.

## File Structure
- **main.py**: The main file where the bot's logic is implemented.
- **README.md**: This file, explaining how to use the bot.
- **requirements.txt**: A list of required Python libraries for easy installation.
  
## Example Conversation
```
User: Привет, бот!
Bot: Привет, пользователь! Как дела?

User: Как тебя зовут?
Bot: Меня зовут ZypherBot.

User: Пока!
Bot: До свидания!
```

## Contributions
Contributions are welcome! If you'd like to improve the bot or add new features, feel free to fork the repository and submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
