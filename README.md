# Python_Class_Project
#### Class Project summary
##### The goal for this project is to create a simple game utilizing the concepts learned in the class, like using simple coding like "inputs", "integers", and other things like random number generator. The reason that I have picked something like this for a project to to better cement the basics that was learned.
##### Usage of this game is very straight forward. You create a username to use with it then it will ask you if you want to play, this will be answered with a simple [Y/N]. Then you get to guess till your answer is correct.
#### Example of the code:
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
          
#### references and links:
[python simple game tutorial](https://www.youtube.com/watch?v=l90vKQMDHPU)
