Python With Yashveer 


Game name-Guess number 
```python


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
    while (x <= 9):
        number = int(input("please enter a number ->"))
        if number == y:
            print("-------------------YOU WINNER----------------------")
            print("Total no. of guesses =>", x)
            z = int(input("what you will start a new game please enter 1 ->"))
            if(z == 1):
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


my_function()



```
Pattern Printing


```python
number1 = int(input("enter a number ->"))
number2 = int(input("enter a 0 ya 1 ->"))
new = bool(number2)
print(new)
if new == True:
    for i in range(0, number1):
        for j in range(0, i+1):
            print("*", end=" ")
        print(" ")
elif new == False:

    for i in range(0, number1):
        for j in range(0, number1-i):
            print("*", end=" ")
        print(" ")
```


## Contact US-[Yashveer Soni](https://github.com/Yashveersoni123/Python-game)
