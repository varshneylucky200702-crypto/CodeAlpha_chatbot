# CodeAlpha_chatbot
print("RADHEY RADHEY! WELCOME TO YOUR CHATBOT")
print("YOU CAN ASK ME BASIC QUESTION , TYPE bye TO EXIT FROM CHATBOT")
# chatbot memory creation {dictionary of creation}
responses=  {
    "hello": "Hi ! welcome , how can i help you?",
    "how are you": "i am fine ! what about you?",
    "who are you?": "I am AI chatbot ",
    "motivate me": " always remember that real intelligence is real ....yes i am smart AI but I can also do mistake sometime as you can ...so don`t make yourself seems fool or failure bcz its only a part of life ....real is real",
    "happy":  "great to hear ! keep smiling and happy bro/sis ",
    "MAAsterG":"A SPIRITUAL MAASTER WHO INSPIRE DAILY",
    "PREMANEND JI":"RADHEY RADHEY JI PYARE"
}    
# method to get  response from chatbot
def getresponseOfBot(userquestion):
    userquestion=userquestion.lower()
    for eachkey in responses:
        if eachkey in userquestion :
            return responses[eachkey]
    return " do not now ! I learn soon"    
        
# take input from user
while(True):
    userinput=input("please ask your querry?")
    reply=getresponseOfBot(userinput)
    print("response is :",reply)
    if ("bye") in userinput.lower():
        break
    
