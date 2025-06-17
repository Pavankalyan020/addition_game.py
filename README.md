# addition_game.py
Simple Game: Add Two Numbers
import random

def addition_game():
    num1 = random.randint(1, 50)
    num2 = random.randint(1, 50)
    correct_answer = num1 + num2

    print("Welcome to the Addition Game!")
    print(f"What is {num1} + {num2}?")

    try:
        user_answer = int(input("Your answer: "))
        if user_answer == correct_answer:
            print("Correct! Well done! 🎉")
        else:
            print(f"Oops! The correct answer was {correct_answer}. Try again!")
    except ValueError:
        print("Please enter a valid number.")

addition_game()

