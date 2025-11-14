# 🏋️‍♂️ Gym Management System

*A lightweight and efficient Gym Management System to handle members, attendance, subscriptions, and reports.*

# ⭐ Features:-

*1. Member Registration & Management*

*2. Attendance Tracking*

*3. Subscription Plans & Payments*

*4. CSV Export*

*5. Simple & Fast UI*

*6. Secure Authentication*

# Libraries Used :-
# *1. Standard Python Libraries*

*These come built-in with Python and require no installation.*

✔ ***os*** = Used to handle file paths and create folders.Example: creating the gym_data directory.

✔ ***csv*** = Used to store and read data from CSV files.Handles members.csv and attendance.csv.

✔ ***hashlib*** = Used for secure password hashing using PBKDF2.Ensures passwords are stored safely.

✔ ***hmac*** = Performs secure hash comparison to prevent attacks.

✔ ***re (Regular Expressions)*** = Used to clean phone numbers (keeping only digits).Used for validating date and extracting digits.

✔ ***datetime*** = Used to generate timestamps in Indian Standard Time (IST).Used for reading/storing dates (DOB, joined-on, entry/exit log).

✔ ***typing*** = Provides type hints like Optional, improving code clarity.

✔ ***threading*** = Used to run Flask server in a background thread while Colab continues running.

✔ ***time*** = Used for small delays when initializing Flask + ngrok.

# *2. External Libraries (Installed Using pip)*

*These are installed using pip install inside Google Colab.*

**⭐ 1. Flask = Used to build the web-based frontend.**

Handles:
1. routing (/login, /register)

2. HTML forms

3. displaying members/attendance in tables

4. running a web server

**⭐ 2. pyngrok =**

1. Used to expose the Flask web app to the internet from Google Colab.

2. Creates a public URL using ngrok.

3. Google Colab Environment Tools
