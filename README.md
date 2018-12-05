# Python_Class_Project
#### Class Project Summary
##### The goal for this project is to create a simple game utilizing the concepts learned in the class, like using simple coding like "inputs", "integers", and other things like random number generator. The reason that I have picked something like this for a project to to better cement the basics that was learned.
##### Usage of this game is very straight forward. You create a username to use with it then it will ask you if you want to play, this will be answered with a simple [Y/N]. Then you get to guess till your answer is correct.
#### Example of the code:
```python
uname = input("Hello, What is your username?")

print("Hello", uname + ".", )

question = input("Would you like to play a game? [Y/N] ")

if question == "n":

    print("Oh...okay maybe next time")

if question == "y":

    print ("I'm thinking of a number between 1 & 10")
    guess = int(input("Have a guess: "))
    if guess > number:
        print("Guess lower...")
        
if guess < number:

    print("Guess Higher...")
    
while guess != number:

    tries += 1
    guess = int(input("Try again: "))
    if guess < number:
        print ("Guess Higher")
        
if guess == number:
    print("Congrats! you guessed the right number! you win! the number was", number, \
          "and it only took", tries, "tries!")
```

##### This was the start of the code that was created with the help from python tutorials. After fiddling around with the code it was moddifed to create a repeating loop as well as fix some issues with dialouge prompts. With help from proffessor Miller a new and improved version of the game was made to even futher help develope python basics.

```python
import random

number = random.randint(1, 10)
tries = 1


uname = raw_input("Hello, What is your username?")

print("Hello", uname + ".", )

end = False
question =raw_input("Would you like to play a game? [Y/N] ")
if question.upper() == "N":
    print("Oh...okay maybe next time")
if question.upper() == "Y":
    while not end:
        print ("I'm thinking of a number between 1 & 10")
        number = random.randint(1, 10)
        tries = 1
        guess = int(raw_input("Have a guess: "))
        while guess != number:
            tries += 1
            guess = int(raw_input("Try again: "))
            if guess > number:
                print("Guess Lower...")
            elif guess < number:
                print ("Guess Higher...")
        if guess == number:
            print("Congrats! you guessed the right number! you win! the number was", number, \
                  "and it only took", tries, "tries!")
        question =raw_input("Would you like to play again? [Y/N] ")
        if question.upper() == 'N':
            end = True
```
            
##### This is the final product for this simple game.
          
#### References and Links:
[python simple game tutorial](https://www.youtube.com/watch?v=l90vKQMDHPU)
