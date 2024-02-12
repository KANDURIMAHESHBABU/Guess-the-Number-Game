# Guess-the-Number-Game
import random

def guess_the_number():
   
    secret_number = random.randint(1, 1000)
    
    
    attempts = 0
    
    print("Welcome to Guess the Number game!")
    print("I've picked a number between 1 and 1000. Try to guess it!")
    
    while True:
        guess = int(input("Enter your guess: "))
        attempts += 1
        
        if guess < secret_number:
            print("Too low! Try again.")
        elif guess > secret_number:
            print("Too high! Try again.")
        else:
            print(f"Congratulations! You've guessed the number {secret_number} correctly in {attempts} attempts!")
            break

if __name__ == "__main__":
    guess_the_number()
