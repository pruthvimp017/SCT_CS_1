Caesar Cipher CLI Tool (Windows)

A lightweight Command Line Interface (CLI) tool for encrypting and decrypting text using the Caesar Cipher.
Built in Python, designed for Windows, and suitable for academic submissions and beginner cryptography demos.

📌 Project Highlights

✅ Encrypt & decrypt text using Caesar Cipher

✅ Preserves uppercase, lowercase, numbers, spaces, and symbols

✅ User-defined shift value (auto-normalized)

✅ Windows-compatible CLI (Command Prompt / PowerShell)

✅ Clean argument parsing with --help support

🛠️ Tech Stack

Language: Python 3.8+

Platform: Windows

Libraries: argparse (standard library)


⚙️ Installation & Setup
1️⃣ Install Python

Download from: https://www.python.org

✔ Ensure “Add Python to PATH” is checked during installation.

Verify:

python --version

🚀 Usage
Encrypt
python caesar.py -t "Hello World!" -s 3


Output

Khoor Zruog!

Decrypt
python caesar.py -t "Khoor Zruog!" -s 3 -d


Output

Hello World!

Help Menu
python caesar.py --help

🧾 Command-Line Arguments
Flag	Description
-t, --text	Input text
-s, --shift	Shift value (integer)
-d, --decrypt	Enable decryption mode
🖥️ Run as a Windows Command (Optional)

Create caesar.bat:

@echo off
python "%~dp0caesar.py" %*


Add the folder to Environment Variables → Path

Now run from anywhere:

caesar -t "Attack at dawn!" -s 4

🧠 Algorithm (High-Level)

Read command-line arguments

Normalize shift using modulo 26

Reverse shift if decrypt mode

For each character:

Shift alphabetic characters

Preserve others

Print output

📚 Use Cases

Cryptography fundamentals

CLI tool development practice

Academic assignments

Interview / internship demonstrations

⚠️ Limitations

❌ Not cryptographically secure

❌ Easily breakable via brute force

❌ Educational use only

📄 Report

A detailed project report with algorithm and flowchart is included:

📎 Caesar_Cipher_CLI_Report.pdf

🏁 Conclusion

This project demonstrates a clean and functional implementation of the Caesar Cipher using a Windows-based CLI approach. While unsuitable for real-world security, it effectively showcases command-line design, character manipulation, and basic cryptographic concepts.
