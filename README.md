Email Agent Python Script

This project contains Python scripts to automatically read emails from a Gmail inbox and send emails using Gmail SMTP. It is designed as a simple email agent for automation purposes.

Features
1. Email Reader

Connects to Gmail via IMAP.

Searches for unread emails from a specific sender (e.g., a lecturer).

Displays:

Sender’s email address

Email subject

Message body (plain text)

Logs out automatically after reading emails.

2. Email Sender

Sends emails via Gmail SMTP.

Supports:

Specifying recipient email

Custom subject and body

Uses Google App Passwords for authentication.

Requirements

Python 3.x

Libraries:

pip install email
pip install imaplib
pip install smtplib


Gmail account with App Password enabled for IMAP/SMTP access.

Note: Standard Gmail passwords may not work due to security restrictions. Use a Google App Password.

Setup Instructions

Clone the repository (or copy your scripts) to your local machine:

git clone <your-repo-url>


Update email credentials in both scripts:

your_email = "your-email@gmail.com"
your_password = "your-app-password"


Update recipient or sender info as needed:

# Email Reader
'(UNSEEN FROM "sender-email@gmail.com")'

# Email Sender
to_email = "recipient-email@gmail.com"


Run the scripts:

python read_email.py
python send_email.py

Usage Examples
Read unread emails from lecturer
✅ New email from: dantetrevordrex@gmail.com
Subject: Assignment Update

📩 Message body:
Hello, please review the attached assignment before Friday.

Send a test email
Email sent successfully!
