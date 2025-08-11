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
