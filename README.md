# Bard-api-for-everyone-Hello this is a free Bard api key ofr everyone
I have provided everything
just run 'pip install GoogleBard' in your command line
and paste the given code and hit the run button.
code:



from Bard import Chatbot

token = 'YwjINDGxf536sZ-cBs-jTIHvG1w4wC718LWZJivc8IsjAWjxtbwzg_agx51044O4DfNO-Q.'
secure_1psidts = 'YwjINDGxf536sZ-cBs-jTIHvG1w4wC718LWZJivc8IsjAWjxtbwzg_agx51044O4DfNO-Q.'

chatbot = Chatbot(token, secure_1psidts)

def prompt_bard(prompt):
    response = chatbot.ask(prompt)
    return response['content']

while True:
    message = input("Ask me anything: ")
    print(prompt_bard(message))
