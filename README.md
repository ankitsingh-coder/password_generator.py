# password_generator.py
A simple Python password generator for creating secure random passwords.
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

