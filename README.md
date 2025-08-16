# 🗣 Smart Voice Assistant
A Python-based voice-controlled assistant that can respond to greetings, tell the time/date, search Google/Wikipedia, open selected websites, send emails, and more — all through simple voice commands.

## 📌 Features
- Responds to greetings like *"Hello"* 👋
- Tells you the *current time* ⏰
- Tells you the *current date* 📅
- Performs *Google/Wikipedia searches* 🔍
- Opens selected websites (*Google, YouTube, LinkedIn*) 🌐
- Sends emails through voice commands ✉
- Ends session when you say *"Goodbye"* or *"No Thanks"* 🚪

---

## 📦 Modules Used and Their Purpose

| Module | Purpose |
|--------|---------|
| pyttsx3 | Converts text to speech for audio responses |
| speech_recognition | Captures and recognizes voice input |
| wikipedia | Fetches quick summaries from Wikipedia |
| webbrowser | Opens websites in the default browser |
| datetime | Gets the current date and time |
| time | Adds delays between operations |
| smtplib | Sends emails using SMTP protocol |
| email.message | Creates and formats email messages |

---

## ⚙ Functions in the Project

| Function | Description |
|----------|-------------|
| speak(audio) | Speaks the given text aloud |
| pns(text) | Prints and speaks text together |
| WishMe() | Greets the user based on the current time |
| listen() | Listens to the user's voice and converts it to text |
| WikiSearch() | Searches Wikipedia and speaks a brief summary |
| Website() | Opens user-specified websites |
| actual_time() | Tells the current time |
| actual_date() | Tells the current date |
| sendMail() | Sends an email to a specified recipient |
| Menu() | Lists all available commands |
| main() | Main loop that listens and executes commands |

---

## 🚀 How to Run

1. *Install Python* (v3.8 or above recommended)
2. *Install the required modules* using pip:
   ```
   pip install pyttsx3 SpeechRecognition wikipedia
   ```
3. Save the project code as voice_assistant.py
4. Run the script:
   ```
   python voice_assistant.py
   ```
5. Start speaking commands like:
- "Hello"
- "What is the time?"
- "What is the date?"
- "Wikipedia search"
- "Open website"
- "Send mail"
- "Goodbye"

---

## 💡 Example Usage

```
User: Hello
Assistant: Hello Sir, I'm your Personal Voice Assistant! How would you like me to help you?

User: What is the date
Assistant: The date is 11th of August of year 2025

User: Open website
Assistant: Which website would you like me to open?
```
---
---
---
# BMI Calculator 🧮

A Python program to calculate **Body Mass Index (BMI)** with **realistic input limits** and robust **exception handling**.

---

## 📌 Features
- Takes **weight (kg)** and **height (m)** from the user
- Validates:
  - ✅ Non-numeric inputs
  - ✅ Blank or whitespace inputs
  - ✅ Negative or zero values
  - ✅ Unrealistic values (Weight: 5–200 kg, Height: 0.2–2.5 m)
- Categorizes BMI into:
  - Underweight
  - Healthy (Normal Weight)
  - Overweight
  - Obese (with Obesity Classes I, II, and III)
- Keeps prompting until valid values are entered

## 🧠 BMI Categories Reference

| BMI Value     | Category                       |
|---------------|--------------------------------|
| < 18.5        | Underweight                    |
| 18.5 – 24.9   | Healthy (Normal Weight)        |
| 25 – 29.9     | Overweight                     |
| 30 – 34.9     | Obesity Class I                |
| 35 – 39.9     | Obesity Class II               |
| ≥ 40          | Obesity Class III (Severe)     |

## 📂 Code Overview
- Main function: Handles the whole process
- take_input() → Handles user input with:
  - try-except blocks for exception handling
  - Validation for positive numeric values
  - Range checks for realistic data
- BMI Calculation:
```
bmi = w / (h ** 2)
```
- BMI Categorization: Uses conditional statements to determine BMI category.

---

## 🖥️ How to Run
1. **Clone this repository** or download the Python file:
   ```
   git clone https://github.com/yourusername/bmi-calculator.git
   cd bmi-calculator
   ```
2. Run the program in your terminal:
   ```
   python bmi_calculator.py
   ```

##📜 Example Output
```
Enter your weight (in kg): 72
Enter your height (in m): 1.78

Your Body Mass Index is: 22.72
Your BMI Category is:
You are Healthy (Normal Weight)!
```
---
---
---
# 🔐 Random Password Generator

A simple Python program to generate **random secure passwords** based on user preferences for letters, numbers, and symbols.  
The program includes **basic exception handling** to avoid crashes when users enter invalid inputs.

---

## 📌 Features
- User specifies:
  - Password length
  - Whether to include **letters**
  - Whether to include **numbers**
  - Whether to include **symbols**
- Validates inputs:
  - Ensures only integers are entered
  - Ensures options are `1 (Yes)` or `0 (No)`
  - At least one character type must be selected
- Generates a password of the requested length using the selected character sets

## 📂 Code Overview
- Main function: Handles the whole process
- pw_specs() → Handles user input with try-except for invalid integers.
  - Validates only 0/1 for choices
  - Ensures at least one option is selected
- Password Generation:
```
for i in range(length):
    password += random.choice(choices)
```
---

## 🖥️ How to Run
1. Clone this repository or download the Python file:
   ```
   git clone https://github.com/yourusername/password-generator.git
   cd password-generator
   ```
2. Run the script:
   ```
   python password_generator.py
   ```

## 📜 Example Output
   ```
   Enter the length of your password: 10
   Do you want letters in your password? (1 for Yes, 0 for No): 1
   Do you want numbers in your password? (1 for Yes, 0 for No): 1
   Do you want symbols in your password? (1 for Yes, 0 for No): 0

   Your random generated password of length 10 is: kF2hT8wLpQ
   ```
