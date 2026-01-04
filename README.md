# Password Generator (Python)

A simple Python password generator for creating secure random passwords.

## Features
- User-defined password length
- Uses letters, digits, and special characters
- Generates secure random passwords

## Code
```python
import random
import string

print("PASSWORD GENERATOR")

length = int(input("Enter password length: "))

characters = string.ascii_letters + string.digits + string.punctuation
password = ""

for i in range(length):
    password += random.choice(characters)

print("Generated Password:", password)



