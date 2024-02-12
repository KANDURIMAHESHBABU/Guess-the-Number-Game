# Guess-the-Number-Game
import random

def guess_the_number():
   
    secret_number = random.randint(1, 10000)
    
    
    attempts = 0
    
    print("Welcome to Guess the Number game ")
    #guess tha number game between the 1 to 10000.
    print("I have picked a number between the 1 and 10000. Try to guess it!")
    
    while True:
        guess = int(input("Enter your guess: "))
        attempts =attempts + 1
        
        if guess < secret_number:
            print("Too low! Try again.")
        elif guess > secret_number:
            print("Too high! Try again.")
        else:
            print(f"Congratulations! You have guessed the number is {secret_number} correctly in {attempts} attempts!")
            break

if __name__ == "__main__":
    guess_the_number()

