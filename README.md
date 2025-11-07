# Simple Chatbot Example

def chatbot():
    print("Chatbot: Hi there! I'm a simple chatbot. Type 'bye' to exit.\n")

    while True:
        user_input = input("You: ").lower()

        # Exit condition
        if "bye" in user_input:
            print("Chatbot: Goodbye! Have a great day!")
            break

        # Greetings
        elif any(word in user_input for word in ["hi", "hello", "hey"]):
            print("Chatbot: Hello! How can I help you today?")

        # Asking how the bot is
        elif "how are you" in user_input:
            print("Chatbot: I'm just a bunch of code, but I'm doing great! Thanks for asking.")

        # Asking for the bot's name
        elif "your name" in user_input:
            print("Chatbot: I'm ChatBot 1.0, your friendly virtual assistant!")

        # Asking about the weather
        elif "weather" in user_input:
            print("Chatbot: I'm not sure, but you can check your local forecast online!")

        # Default response
        else:
            print("Chatbot: I'm not sure I understand. Could you rephrase that?")

