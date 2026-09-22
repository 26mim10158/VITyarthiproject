# Number Guessing Game--

A simple **Python command-line game** where the computer randomly selects a number between **1 and 100**, and the player tries to guess it.

After every guess, the game gives a hint telling the player to **go higher** or **go lower** until the correct number is guessed.

# Features

*  Random number generated between 1 and 100
*  User enters guesses through the terminal
*  Provides hints after every incorrect guess
*  Counts the number of attempts
*  Displays the number of tries when the player wins
*  Simple and beginner-friendly Python project

# Technologies Used

* **Python 3** latest ver.
* `random` module
* Command-line/Terminal

# How to Play
note -- firstly check that you have latest python version 3 and then run this code on your computer.

1. The computer randomly selects a number from **1 to 100**.
2. Enter your guess when prompted.
3. If your guess is too high, the game tells you:
please go lower

4. If your guess is too low, the game tells you:
please go higher

5. Continue guessing until you find the correct number.
6. The game displays how many attempts you tried.

# Example

guess your number between 1 - 100 :- 50
please go higher

guess your number between 1 - 100 :- 75
please go lower

guess your number between 1 - 100 :- 63
please go higher

guess your number between 1 - 100 :- 68
congratulations you won in 4 tries

# How the Code Works
1. Import the Random Module
import random

The `random` module is used to generate a random number.
2. Generate the Computer's Number
com = random.randint(1, 100)

This generates a random integer between **1 and 100**.

3. Initialize the Attempt Counter
tries = 0

This variable keeps track of how many guesses the player has made.

4. Get the User's Guess
hum = int(input("guess your number between 1 - 100 :- "))

The user enters a number, which is converted from text to an integer using `int()`.

5. Compare the Guess

If the guess is correct:
if hum == com:
    print(f"congratulations you won in {tries} tries")
    break

The game displays the number of attempts and stops.

If the guess is too high:

elif hum > com:
    print("please go lower")

If the guess is too low:

elif hum < com:
    print("please go higher")

# Concepts Practiced
* Variables
* User input
* `if`, `elif` statements
* `while` loops
* `break`
* Random number generation
* Type conversion
* F-strings
* Basic game logic

# Author
**ROHAN PATEL (26MIM10158)**
