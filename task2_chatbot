import nltk
from nltk.chat.util import Chat, reflections


patterns = [
    (r"hi|hello|hey", ["Hello! How can I help you today?", "Hi there! What can I do for you?"]),
    (r"what is your name?", ["I'm a simple chatbot created using Python."]),
    (r"how are you?", ["I'm just a bot, but I'm doing great! How about you?"]),
    (r"my name is (.*)", ["Hello, %1! Nice to meet you."]),
    (r"quit", ["Goodbye! Have a great day!"]),
]


chatbot = Chat(patterns, reflections)


def chat():
    print("Hello! I am your chatbot.")
    print("Type 'quit' to exit.")
    
    while True:
       
        user_input = input("You: ")
        
       
        if user_input.lower() == "quit":
            print("Chatbot: Goodbye!")
            break
        
        
        response = chatbot.respond(user_input)
        
        if response:
            print(f"Chatbot: {response}")
        else:
            print("Chatbot: Sorry, I don't understand that.")


if __name__ == "__main__":
    chat()
