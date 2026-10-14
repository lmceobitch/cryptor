CRYPTOR

CRYPTOR is a Python tool that lets you encrypt and decrypt text using a password.

Features

- Encrypt and decrypt messages
- AES-256-GCM for strong security
- Custom cipher for learning and experimenting
- Choose the length of the encrypted code

Requirements

Install Python 3.9 or newer.

For AES encryption, install this library:

pip install cryptography

How to Use

1. Start the program

python cryptor.py

Follow the menu to choose the encryption mode, action, code length, message, and password.

2. Encrypt a message

python cryptor.py -e "Hello World" -l 100 --mode aes

The program will ask for a password if you don't provide one.

3. Decrypt a message

python cryptor.py -d "YOUR_ENCRYPTED_CODE" -l 100 --mode aes

Use the same password and code length you used when encrypting.

4. Choose a mode

- "aes" — recommended for real messages.
- "custom" — made for experimenting and learning(i will develop it a little more later).

Example using custom mode:

python cryptor.py -e "Hello World" -l 100 --mode custom

5. Use your own password

python cryptor.py -e "Hello World" -p "myPassword123" -l 100 --mode aes

It's safer to let the program ask for your password instead of typing it directly into the command.

Code Length

The "-l" option sets the length of the encrypted code.

For example, "-l 100" requests a code with 100 characters. Extra characters are only padding and don't make the encryption stronger.

Important

Use AES mode for real data. The custom mode is only for learning and should not be used to protect real personal stuff, but idk who would use that in a random github tool so cool , i hope it will be of use and i like it very much, and you NEED the password to decrypt a message .
