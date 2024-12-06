# Import Libraries
import re

def language_chatbot(user_input):
    user_input = user_input.lower()
    
    # ----***ENGLISH SECTION***--------------------------------------------------------------------------------------
    if "hello" in user_input or "hi" in user_input:
        if "how are you" in user_input:
            return "I'm just a bot, but I'm doing great! How about you?"
        elif re.search(r"bye|goodbye|see you", user_input):
            return "Goodbye! Have a great day!"
        else:
            return "Hello! How can I assist you today?"

    # ----***FRENCH SECTION***--------------------------------------------------------------------------------------
    elif "bonjour" in user_input or "salut" in user_input:
        if "comment ça va" in user_input:
            return "Je suis juste un bot, mais je vais très bien! Et vous?"
        elif re.search(r"au revoir|adieu|à bientôt", user_input):
            return "Au revoir! Passez une excellente journée!"
        else:
            return "Bonjour! Comment puis-je vous aider aujourd'hui?"

    # ----***SPANISH SECTION***--------------------------------------------------------------------------------------
    elif "hola" in user_input or "buenos días" in user_input:
        if "cómo estás" in user_input:
            return "Soy solo un bot, ¡pero estoy muy bien! ¿Y tú?"
        elif re.search(r"adiós|hasta luego|nos vemos", user_input):
            return "¡Adiós! ¡Que tengas un gran día!"
        else:
            return "¡Hola! ¿Cómo puedo asistirte hoy?"

    # ----***GERMAN SECTION***--------------------------------------------------------------------------------------
    elif "hallo" in user_input or "hi" in user_input:
        if re.search(r"wie gehts dir|wie gehts dir?|wie gehts|wie gehts?|wie gehts ihnen|wie gehts ihnen?|wie geht's dir ?|wie geht's dir", user_input):
            return "Ich bin ein Bot, aber ich bin gut! Und Sie?"
        elif re.search(r"tschüß|tschüss|auf wiedersehen|bis bald|guten abend", user_input):
            return "Tschüß! Bis bald!"
        else:
            return "Hallo! Wie kann ich Ihnen heute helfen?"

    # ----***DEFAULT RESPONSE***-------------------------------------------------------------------------------------
    else:
        return "Sorry, I didn't understand that. Can you please rephrase? Make sure to write 'hello' in your own language for a customized experience."
def chatbot_homepage():
    print("="*50)
    print("🌟 Welcome to the Multilingual Chatbot! 🌟")
    print("="*50)
    print("Chatbot 🤖: Hello! 🙋‍♂️ Type 'bye' to exit 🏃‍♂️.")
    print(" --> Write 'hello' for English 🍔")
    print(" --> Write 'hallo' for German 🥨")
    print(" --> Write 'bonjour' for French 🥐")
    print(" --> Write 'hola' for Spanish 🍕")
    print("="*50)



# Chatbot interaction loop
chatbot_homepage()
while True:
    user_message = input("You: ")
    if "bye" in user_message.lower():
        print("Chatbot: Goodbye!")
        break
    response = language_chatbot(user_message)
    print("Chatbot 🤖:", response)
