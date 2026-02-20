🤖 Smart AI Chatbot (Python Basic Project)
A simple AI Chatbot built using basic Python concepts, including:
datetime module (24-hour clock greeting system)
time module
os module (file handling)
Dictionaries
Functions
Loops
File read/write operations
This chatbot can:
Greet users based on current time
Respond to predefined questions
Learn new responses
Save chat history
Store learned knowledge permanently

📌 Features
1️⃣ Time-Based Greeting

The chatbot uses the datetime module to greet users according to the current hour:

🌅 Good Morning (5 AM – 12 PM)
☀️ Good Afternoon (12 PM – 5 PM)
🌆 Good Evening (5 PM – 9 PM)
🌙 Good Night (9 PM – 5 AM)

Example:

presenthour = datetime.datetime.now().hour
2️⃣ Predefined Responses

The chatbot contains some built-in responses stored inside a Python dictionary:

responses = {
    "hello": "Hii welcome. how can I help you?",
    "how are you": "I am very fine. thank you",
}

It matches user input with keywords and replies accordingly.

3️⃣ Learning New Things 🧠

If the chatbot does not know an answer:
It asks the user to teach it
Saves the new question and answer in brain.txt
Loads the saved data automatically next time the program runs
Format inside brain.txt:
question::answer
4️⃣ Chat History 📜

All conversations are saved in history.txt.

Example format:

User: hello
Bot: Hii welcome. how can I help you?

This is handled using file append mode:

with open(HISTORY_FILE, "a", encoding="utf-8") as f:
📂 Project Structure
📁 Chatbot Project
│
├── chatbot.py
├── brain.txt        # Stores learned responses
├── history.txt      # Stores conversation history
└── README.md
🛠️ Technologies Used

Python 3
datetime module
os module
File Handling
Dictionaries
Functions
While Loop
Conditional Statements

▶️ How to Run

Make sure Python is installed.
Save the file as chatbot.py
Open terminal or command prompt.

Run:

python chatbot.py
💡 How It Works

User enters their name.
Bot greets based on time.
User starts chatting.

Bot:

Replies if it knows the answer.

Learns if it doesn’t know.

Type bye to exit.

🎯 Learning Concepts Covered

This project is great for beginners because it teaches:

Variables
Dictionaries
String methods (lower(), strip())
Functions
Loops
File handling
Working with date and time
Basic AI logic (keyword matching)
Data persistence

🚀 Future Improvements

You can improve this chatbot by adding:

NLP using nltk

GUI using tkinter

Voice support using speech_recognition

Better matching using similarity algorithms

Removing repeated keywords problem

Using JSON instead of text files

👨‍💻 Author

Created as a beginner-friendly Python AI Chatbot project.
