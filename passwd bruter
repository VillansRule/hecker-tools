import itertools
import string

def generate_passwords(length):
    characters = string.ascii_letters + string.digits + string.punctuation
    return (''.join(password) for password in itertools.product(characters, repeat=length))

def check_password(username, password):
    # Code to connect to the target system and check the password
    # Return True if the password is correct, False otherwise
    return False

username = input("Enter the username: ")

for length in range(1, 10):
    passwords = generate_passwords(length)
    for password in passwords:
        if check_password(username, password):
            print(f"Password found: {password}")
            break


