# Fun-Games

```python
import random

def guessing_game():
    print("Welcome to the Guessing Game!")
    secret_number = random.randint(1, 10)
    attempts = 0

    while True:
        guess = int(input("Enter your guess (between 1 and 10): "))
        attempts += 1

        if guess == secret_number:
            print(f"Congratulations! You guessed the correct number in {attempts} attempts.")
            break
        elif guess < secret_number:
            print("Too low! Try again.")
        else:
            print("Too high! Try again.")

if __name__ == "__main__":
    guessing_game()
```
