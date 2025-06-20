
# -AI-chatbot-with-NLP

#COMPANY:CODETECH IT SOLUTIONS

#NAME:VENKATA SRINIVASA RAO KILLADI

#INTERN ID:CT04DF812

#DOMAIN:PYTHON PROGRAMMING

#DURATION:4 WEEKS

#MENTOR:NEEELA SANTOSH

problem statement: 

This project demonstrates a simple rule-based chatbot built using Python and Natural Language Processing (NLP) with NLTK. The chatbot can engage in basic conversations and respond to user queries with predefined answers.

## 📌Objective

To create an interactive chatbot using NLP techniques capable of understanding and responding to simple text-based user queries.

## 🧰 Tools and Libraries Used

- **Python** – Core programming language
- **NLTK** – Natural Language Toolkit for basic NLP processing

## 📂 Files Included

- `chatbot.py` – Main Python script for running the chatbot
- `requirements.txt` – Python dependencies
- `README.md` – Project documentation

📌STEP BY STEP CODE EXPLANATION:

1. Importing Required Modules:
   
    import nltk
   
    from nltk.chat.util import Chat, reflections
   
Chat: A utility in nltk for creating chatbots using predefined pattern-response pairs.

reflections: A dictionary that maps first-person to second-person pronouns (e.g., “I” ↔ “you”), which helps in mirroring user inputs for better responses.

2. Defining Pattern-Response Pairs:
   
        pairs = [
     
               [r"hi|hello|hey", ["Hello!", "Hi there!", "Hey! How can I help you?"]],
   
               ...
   
        ]
-Each item in pairs is a list where:

-The first element is a regex pattern to match user input.

-The second is a list of possible responses (one will be chosen randomly).

3. Chatbot Logic:

       def start_chat():
   
       print("Hi! I'm your chatbot. Type 'quit' to exit.")
   
       chatbot = Chat(pairs, reflections)
   
       chatbot.converse()
   
-Chat(pairs, reflections): Creates a chatbot using the patterns and reflection logic.

-.converse(): Starts an interactive chat loop where user can type and get responses.

-Typing "quit" or "exit" ends the conversation.

4. Program Entry Point:

       if __name__ == "__main__":
   
        start_chat()

-This ensures the chatbot starts only when the script is run directly, not when imported as a module.

📌SAMPLE OUTPUT:

Hi! I'm your chatbot. Type 'quit' to exit.

> hello

Hi there!

> what is your name?

I'm a chatbot created using NLTK.

> how are you?

I'm doing great, thank you!

> exit

Goodbye!

📌SUMMARY:

-This is a simple NLTK-based chatbot that uses regex patterns to reply to user inputs. 

-It matches user messages with predefined responses and runs in a loop until the user types "quit" or "exit".

📌OUTPUT:

![Image](https://github.com/user-attachments/assets/011f0f2d-b41c-45ca-8268-8c4758a67e8d)
