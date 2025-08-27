# Number-guessing-game
import random

n = random.randint(1, 100)
a = -1
guesses = 0

print("PEOGGRAMER SUMAN \u2764")
print(" Welcome to the Number Guessing Game!")
print("Guess a number between 1 and 100\n")

while a != n:
    try:
        a = int(input("Enter your guess: "))
        guesses += 1

        if a < n:
            print(" 》Higher number please\n")
        elif a > n:
            print("《Lower number please\n")
    except ValueError:
        print(" Invalid input! Please enter a number.\n")

print(f"₩ You guessed the number {n} correctly in {guesses} attempts!")