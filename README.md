# Remote Keylogger in Python

## Project Overview
This project implements a remote keylogger written in Python. It captures keystrokes, takes periodic screenshots, collects basic system information (hostname, IP addresses, username, OS details), and periodically emails the data with optional screenshot attachments.

The keylogger runs silently in the background, sending reports at defined intervals.
[how it works](https://github.com/norb1x/Remote-keylogger/blob/main/screenshots/mail.png)
---

## Features

- Captures all keyboard input.
- Periodic screenshot capture.
- Collects system info: hostname, local IP, public IP, username, OS details.
- Sends data via email using Gmail SMTP.
- Automatically deletes screenshots after sending to avoid clutter.
- Runs as a background thread with configurable report intervals.
[example](https://github.com/norb1x/Remote-keylogger/blob/main/screenshots/insidemail.png)
---

## Requirements

- Python 3.x
- Packages:
  - `pynput`
  - `pyautogui`
  - `requests`

Install required packages via pip:

```bash
pip install pynput pyautogui requests
```

## Setup
Configure your email credentials in the script (EMAIL_ADDRESS, EMAIL_PASSWORD, EMAIL_RECEIVER).

Use a Gmail account with App Password enabled (recommended).

Adjust the reporting interval (INTERVAL) as needed.

Run the script.
