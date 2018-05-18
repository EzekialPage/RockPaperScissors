#Ezekial Page
#simulates a game of rock paper scissors with an ai

from random import seed, randint

def convert(s):
    choice = s.upper()
    if choice == "ROCK":
        return 1
    elif choice == "PAPER":
        return 2
    elif choice == "SCISSORS":
        return 3
    
def shoot(user, ai):
    if(ai == 1) and (user == 1):
        return "ai threw rock\nround resulted in a draw."
    elif(ai == 2) and (user == 2):
        return "ai threw paper\nround resulted in a draw."
    elif(ai == 3) and (user == 3):
        return "ai threw scissors\nround resulted in a draw."
    elif(ai == 1) and (user == 2):
        return "ai threw rock\nround goes to you."
    elif(ai == 1) and (user == 3):
        return "ai threw rock\nround goes to the ai."
    elif(ai == 2) and (user == 1):
        return "ai threw paper\nround goes to the ai."
    elif(ai == 2) and (user == 3):
        return "ai threw paper\nround goes to you."
    elif(ai == 3) and (user == 1):
        return "ai threw scissors\nround goes to you."
    elif(ai == 3) and (user == 2):
        return "ai threw scissors\nround goes to the ai."

def wins(user, ai):
    if(ai == user):
        return 0
    elif(ai == 1) and (user == 2):
        return 1
    elif(ai == 1) and (user == 3):
        return 2
    elif(ai == 2) and (user == 1):
        return 2
    elif(ai == 2) and (user == 3):
        return 1
    elif(ai == 3) and (user == 1):
        return 1
    elif(ai == 3) and (user == 2):
        return 2


print("Welcome to rock, paper, scissors.\nCompete against the ai in a best of 5 series.\n")
aiw = 0
userw = 0
while aiw < 3 and userw < 3:
    userIn = input("Enter Rock, Paper, or Scissors: ")
    ai = randint(1,3)
    user = convert(userIn)
    print(shoot(user, ai))
    if(wins(user, ai) == 1):
        userw+=1
    elif(wins(user, ai) == 2):
        aiw+=1
    if(userw == 3):
        print("you win!!!")
    elif(aiw == 3):
        print("you lose.")
    else:
        print("Current score is ai", aiw, "user", userw)
        print()
    
    
    
