# PRODIGY-INFOTECH-TASK-2-
lggh 

import random #Generate a random number between 1 and 100
number_to_guess = random.randint(1, 10)

# Initialize the number of attempts
attempts = 0

while True:
    # Prompt the user to input their guess
    user_guess = int(input("Guess a number between 1 and 10: "))

    # Increment the number of attempts
    attempts += 1

    # Check if the user's guess is correct
    if user_guess == number_to_guess:
        print(f"Congratulations! You guessed the number in {attempts} attempts.")
        break
    # Check if the user's guess is too high
    elif user_guess > number_to_guess:
        print("Your guess is too high. Try again!")
    # Check if the user's guess is too low
    else:
        print("Your guess is too low. Try again!")
