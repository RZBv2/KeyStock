## KeyStock - an Keylogger


# KeyStock (Windows Only) - For Learning Purposes


## Purpose of This Project

This is a fully functional but **intentionally simple** keylogger designed to teach students and beginners how real-world infostealer malware works under the hood.


It demonstrates the following real attack techniques used by actual malware in 2025:

- Keystroke logging via `pynput`
- Exfiltration over Telegram C2 (Command & Control)
- Fileless-like persistence via `%APPDATA%` + hidden attribute
- Windows Registry Run key persistence (`HKCU\...\Run`)
- Self-replication and silent execution
- Background threading and timed beaconing

Perfect for:
- Cybersecurity / Ethical Hacking courses
- Malware Analysis classes
- CTF challenges
- Red Team training
- Defensive security (Blue Team) labs

## THIS IS NOT MALWARE FOR ILLEGAL USE

 I fully understand and declare that:
- This tool must **never** be used on any computer without explicit written permission
- Using this on someone else's device without consent is a serious crime in most countries
- I take no responsibility for misuse of this code
- This repository is for **educational and defensive learning only**

## Features Demonstrated

- Real-time keystroke capture using `pynput`
- Sending logs every 60 seconds via Telegram Bot
- Self-copying to `%APPDATA%` with hidden attribute
- Adding itself to Windows startup via Registry (`HKCU\...\Run`)
- Running silently in background
- Clean threading implementation


## Warning: Ethical & Legal Notice

> **DO NOT RUN THIS ON ANY SYSTEM YOU DO NOT OWN OR HAVE EXPLICIT WRITTEN PERMISSION TO TEST.**

Using this script against any person or organization without consent is **illegal** in virtually every country (Computer Misuse Act, CFAA, GDPR, etc.).

By using this repository, you agree:
- You will only execute it on your own machines or authorized lab environments
- You accept full responsibility for any misuse
- The author is not liable for any illegal actions



## How to Use (Educational Environment Only)

1. Create a Telegram bot via @BotFather and get your `bot_token`
2. Get your own `chat_id` (you can use @userinfobot)
3. Replace the values in the script:
   ```python
   bot_token = 'YOUR_BOT_TOKEN'
   chat_id = 'YOUR_CHAT_ID'


