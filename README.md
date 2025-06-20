import nltk
from nltk.chat.util import Chat, reflections

# Define some pairs of patterns and responses
pairs = [
    [
        r"hi|hello|hey",
        ["Hello!", "Hi there!", "Hey! How can I help you?"]
    ],
    [
        r"what is your name?",
        ["I'm a chatbot created using NLTK.", "You can call me NLTK Bot."]
    ],
    [
        r"how are you?",
        ["I'm doing great, thank you!", "I'm just a program, but I'm functioning well!"]
    ],
    [
        r"what can you do?",
        ["I can chat with you and answer simple questions.", "I'm here to help with your queries."]
    ],
    [
        r"(.*) your name?",
        ["My name is NLTK Bot."]
    ],
    [
        r"quit|exit",
        ["Goodbye!", "See you later!"]
    ]
]

# Create and run chatbot
def start_chat():
    print("Hi! I'm your chatbot. Type 'quit' to exit.")
    chatbot = Chat(pairs, reflections)
    chatbot.converse()

if __name__ == "__main__":
    start_chat()
