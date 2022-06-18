
## 1-Guess Number



```bash
print("-------------find hidden number--------------")
print("1- Game name = guess number Anything")
print("2- total 5 chance are meet")
print("3- don't try to see the hidden number")
print("4- This code is run in the python compiler")
print("5- copy the code and paste in the following link")
print("6- https://www.programiz.com/python-programming/online-compiler/")
print("lets get start")

def my_function():
    x = 1
    y = 18
    while x <= 9:
        number = int(input("please enter a number ->"))
        if number == y:
            print("-------------------YOU WINNER----------------------")
            print("Total no. of guesses =>", x)
            z = input("what you will start a new game please enter Yes ->")
            if(z == "Yes"):
                my_function()
            break
        elif number > y and number >= 25:
            print("your guesses number is very high please reduce ")
        elif number > y and number <= 25:
            print("you are very close you number")
        elif number < y and number <= 10:
            print("your guesses number is very low please increase")
        elif number < y and number >= 10:
            print("you are very close please increase")
        else:
            print("you lose")
            print("try again later !")
            break

        x = x+1
        print(9-x, "times pending ")

    else:
        print("Try again")
        z = input("what you will start a new game please enter Yes ->")
        if (z == "Yes"):
            my_function()


my_function()

```

## 2- Stone, Paper, Scissors Games


```bash
 
print("This GAME name is Stone, Paper, Scissors")
print("you have a total of 5 chance")
print("this game is only play two-member first is you/user and second is computer")
print("enjoy this game")
print("choose (stone, paper, scissors)")

import random
s="stone"
p="paper"
sys="scissors"
def mygame():
    user_score = 0
    cpu_score = 0
    i = 1
    a = 0
    b =0
    while i<=5:
        user = input("User choosing ->")
        lst=[s,p,sys]
        cpu=random.choice(lst)
        if (user==cpu):
            print("cpu choosing->",cpu)
            print("Tie")
            print("")
        elif (user==s and cpu==p):
            print("cpu chossing->", cpu)
            print("cpu win")
            cpu_score+=1
            print("cpu score->", cpu_score)
            print("")
        elif (user==p and cpu==s):
            print("cpu chossing->", cpu)
            print("user win")
            user_score += 1
            print("user score->", user_score)
            print("")
        elif (user==p and cpu==sys):
            print("cpu chossing ->", cpu)
            print("cpu win")
            cpu_score += 1
            print("cpu score->", cpu_score)
            print("")
        elif (user==sys and cpu==p):
            print("cpu chossing->", cpu)
            print("user win")
            user_score += 1
            print("user score->", user_score)
            print("")
        elif(user==sys and cpu==s):
            print("cpu chossing->", cpu)
            print("cpu win")
            cpu_score += 1
            print("cpu score->", cpu_score)
            print("")
        elif(user==s and cpu==sys):
            print("cpu chossing ->", cpu)
            print("user win")
            user_score += 1
            print("user score->", user_score)
            print("")

        i+=1
    if user_score == cpu_score:
        print("-----------------------TIE------------------------")
    elif user_score>cpu_score:
        print("-----------------------USER WIN-------------------------")
    else:
        print("-----------------------CPU WIN--------------------------")
    print("---------user score ->",user_score)
    print("---------cpu score ->",cpu_score)
    back=input("you can retry the game please enter 'Yes' >")
    if(back=="Yes" or back=="yes" or back=="YES"):
        mygame()

mygame()


```





