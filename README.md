🔐 Python Password Manager (CLI Based)
A secure command-line password manager written in Python that allows users to store, retrieve, and manage website passwords safely using modern cryptographic techniques.
This project demonstrates the implementation of encryption, hashing, and secure password handling using Python libraries. The stored passwords are encrypted using Fernet symmetric encryption, and the master password is protected using SHA-256 hashing.
The program runs entirely in the terminal and stores all credentials in an encrypted vault file, ensuring sensitive data remains protected.

🚀 Features

🔑 Master Password Authentication
A master password is required to access the vault. It is securely stored using SHA-256 hashing.

🔐 AES-Based Encryption (Fernet)
All saved credentials are encrypted using the Fernet encryption mechanism from the cryptography library.

🌐 Add Website Credentials
Store a website name and its corresponding password securely.

🔍 Retrieve Passwords
Fetch stored passwords for any saved website.

🗑 Delete Credentials
Remove saved website passwords from the vault.

📋 Display Stored Entries
View all saved websites and passwords.

🙈 Hidden Password Input
Password input is hidden using getpass for improved security.

💾 Encrypted Storage
All credentials are stored in an encrypted file to prevent unauthorized access.

🛠 Technologies Used
Python
Cryptography (Fernet)
SHA-256 Hashing
JSON Data Storage
OS File Handling
Getpass (Secure Input)


📁 Project Structure

password-manager/
│
├── password_manager.py   # Main program
├── key                   # Encryption key
├── master.key            # Hashed master password
└── lock                  # Encrypted password vault

⚙️ How It Works
1. The user sets a master password on first launch.

2. The password is hashed using SHA-256 and stored securely.

3. An encryption key is generated for the vault stored in key file.

4. Passwords are stored in a JSON structure.

5. The JSON data is encrypted using Fernet before being written to disk.

▶️ How to Run
Install the required library:
pip install cryptography
Run the program:
python password_manager.py

📌 Learning Purpose
This project was built to understand:
Cryptography fundamentals
Secure password storage
Python file handling
CLI tool development
Basic cybersecurity concept
