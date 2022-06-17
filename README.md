
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

