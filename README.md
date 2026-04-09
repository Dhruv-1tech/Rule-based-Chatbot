# 🤖 Simple Rule-Based Chatbot (NLTK)

A lightweight, rule-based chatbot built using Python and Natural Language Toolkit (NLTK). This project demonstrates basic Natural Language Processing (NLP) concepts like tokenization and stemming to match user inputs with predefined intents and generate appropriate responses.

---

## 🚀 Features

* Basic conversational chatbot
* Intent recognition using pattern matching
* Text preprocessing with tokenization and stemming
* Randomized responses for more natural interaction
* Easy to customize and extend

---

## 🛠️ Tech Stack

* Python 3
* NLTK (Natural Language Toolkit)

---

## 📂 Project Structure

```
.
├── chatbot.py       # Main chatbot logic
├── data.py          # Predefined intents and responses
└── README.md        # Project documentation
```

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/simple-chatbot.git
cd simple-chatbot
```

2. Install dependencies:

```bash
pip install nltk
```

3. Run the chatbot:

```bash
python chatbot.py
```

---

## 📌 How It Works

1. **User Input Processing**

   * Converts input to lowercase
   * Tokenizes the sentence
   * Applies stemming using Porter Stemmer

2. **Intent Matching**

   * Matches processed input with predefined patterns
   * Uses simple keyword-based matching

3. **Response Generation**

   * Selects a random response from the matched category
   * Falls back to a default response if no match is found

---

## 🧠 Code Overview

### `preprocess(sentence)`

* Tokenizes and stems user input for better matching.

### `get_response(user_input)`

* Matches user input against intent patterns and returns a response.

### `chat()`

* Runs the chatbot in a loop until the user types `exit`.

---

## 📊 Sample Intents

| Category   | Example Inputs   |
| ---------- | ---------------- |
| Greetings  | hello, hi, hey   |
| Farewells  | bye, goodbye     |
| Questions  | what's your name |
| Small Talk | tell me a joke   |

---

## 💡 Example Interaction

```
Chatbot: Hello! I'm your friendly chatbot. type 'exit' to end the conversation.
You: hi
Chatbot: Hello!

You: tell me a joke
Chatbot: Why don't scientists trust atoms? Because they make up everything!

You: bye
Chatbot: Goodbye!
```

---

## 🧩 Customization

You can easily extend the chatbot by modifying the `data.py` file:

* Add new intent categories
* Add more patterns
* Add more responses

Example:

```python
"food": ["what is your favorite food", "do you like pizza"],
"food_responses": ["I don't eat, but pizza sounds great!", "I'm a bot, I don't have taste buds!"]
```

Then update the `INTENT_RESPONSE_MAP` in `chatbot.py`.

---

## ⚠️ Limitations

* Uses simple keyword matching (no machine learning)
* Cannot understand complex or unseen sentences
* Limited conversational memory (stateless)

---

## 🔮 Future Improvements

* Implement machine learning-based intent classification
* Add context awareness
* Integrate with APIs (weather, news, etc.)
* Build a GUI or web interface

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 🙌 Acknowledgements

* NLTK library for NLP utilities
* Python community for support and resources

---

## 👨‍💻 Author

Your Name
GitHub: https://github.com/Dhruv-1tech

---

⭐ If you like this project, feel free to star the repo!
