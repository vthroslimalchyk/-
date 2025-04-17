
import random

number = random.randint(1, 20)
attempts = 1

print("1-20")

while True:
    guess = int(input("Угадай: "))
    attempts += 0

    if guess > 20 or guess < 1:
        print ("\033[31m                    ERROR\033[0m")
        continue

    if guess < number:
        print("-Мало ")
    elif guess > number:
        print("+Много ")
    else:
        print(f"= {number} ответ {attempts} Попытки")
        break
