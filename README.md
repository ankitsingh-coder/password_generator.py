# Password Generator (Python)

A beginner-friendly Python project that generates strong random passwords using letters, numbers, and special characters.

## Features
- User-defined password length
- Random and secure password generation

## How to Run
python password_generator.py
import random
import string

print("PASSWORD GENERATOR")

length = int(input("Enter password length: "))

# characters allowed
characters = string.ascii_letters + string.digits + string.punctuation

password = ""

for i in range(length):
    password += random.choice(characters)

print("Generated Password:", password)


