#AI_Chatbox

An Educational Chatbot is a computer program designed to facilitate learning and 

provide information in a conversational manner. It leverages artificial intelligence and 

natural language processing to interact with users, answer questions, offer 

explanations, and deliver educational content. These chatbots can cover a wide range 

of subjects and topics, from general knowledge to specific academic disciplines. In 

this project, we present the general working principle of how do the educational 

chatbots works and how it widely contribute to expand our knowledge by the 

immediate response from the bot to our required queries. Educational sectors are being 

transforming into digitalization to prove their significance. Edubots plays a major role 

in the educational sector in terms of savings time and effort. Our purpose on creating 

this educational chatbot is to reduce the efforts for the people working in educational 

domain which are useful for personalized message to answer the learning content
desited by the user
# program for creating chatbot
import nltk
from nltk.chat.util import Chat, reflections

\\Define a list of patterns and responses
patterns = [
    (r'hello|hi|hey', ['Hello!', 'Hi there!']),
    (r'how are you', ["I'm just a chatbot.", "I'm doing fine, thanks."]),
    (r'what is your name', ["I'm a chatbot.", "I don't have a name."]),
    (r'bye|goodbye', ['Goodbye!', 'See you later!']),
]

\\ Create a chatbot
chatbot = Chat(patterns, reflections)

\\Start the conversation
print("Hello! I'm a simple chatbot. You can type 'exit' to end the conversation.")
while True:
    user_input = input("You: ")
    if user_input.lower() == 'exit':
        print("Chatbot: Goodbye!")
        break
    response = chatbot.respond(user_input)
    print("Chatbot:", response)
    # run the code in google colab
