def chatbot():
    print("Chatbot: Hi! I'm Chatbot. Type 'bye' to end the conversation.")
    while True:
        user_input = input("You: ").lower()
        if user_input in ["hi", "hello", "hey"]:
            print("Chatbot: Hello there! How can I assist you today?")
        elif user_input in ["how are you", "how are you doing"]:
            print("Chatbot: I'm doing well, thanks for asking! And you?")
        elif user_input in ["what is your name", "who are you"]:
            print("Chatbot: I'm a friendly chatbot made in Python.")
        elif user_input in ["what can you do", "what do you do"]:
            print("Chatbot: I can chat with you and answer simple questions!")
        elif user_input in ["who made you", "who created you"]:
            print("Chatbot: I was created by a curious programmer.")
        elif user_input in ["what is the time", "tell me the time"]:
            from datetime import datetime
            now = datetime.now().strftime("%H:%M:%S")
            print(f"Chatbot: The current time is {now}.")
        elif user_input in ["what is the date", "tell me the date"]:
            from datetime import date
            today = date.today().strftime("%B %d, %Y")
            print(f"Chatbot: Today is {today}.")
        elif user_input in ["bye", "exit", "quit"]:
            print("Chatbot: Goodbye! Talk to you later.")
            break
        else:
            print("Chatbot: I'm not sure how to respond to that. Try asking something else.")

chatbot()
