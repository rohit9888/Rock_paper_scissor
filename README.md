# Rock_paper_scissor
import random
computer_score = 0
user_score = 0
listt = ['r','p','s']


def rule_set():
    global computer_score,user_score,computer_input
    if user_input == computer_input[0]:
        pass
    elif (user_input == 'r' and computer_input == 'paper') or (user_input =='p' and computer_input =='scissor') or (user_input == 's' and computer_input == 'rock') :
        computer_score+=1
    else:
        user_score+=1
while True:
    user_input = input("press 'r' for rock, 'p' for paper and 's' for scissor" )
    if user_input in listt:
        computer_input = random.choice(['rock', 'paper', 'scissor'])
        print(computer_input)
        rule_set()
        print(f"user score : {user_score}")
        print(f"Computer score : {computer_score}")
    else:
        pass





