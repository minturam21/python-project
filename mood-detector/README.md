# 🎭 Mood Detector

A simple Python program that analyzes a user's text input and detects their mood based on emotional keywords.  
It then returns an encouraging or empathetic quote that matches the detected emotion.

---

## 🧠 How It Works

1. You type how you’re feeling (for example: “I feel so happy today!”).
2. The program converts your text to lowercase.
3. It checks for emotion-related keywords in the text.
4. The mood with the most matches is selected.
5. A motivational or comforting quote for that mood is displayed.

---

## 🚀 Features

- Detects eight moods:  
  `happy`, `sad`, `angry`, `anxious`, `tired`, `motivated`, `confused`, and `grateful`.
- Returns a **random quote** that fits the detected mood.
- Handles neutral input gracefully (no emotion detected).
- Interactive loop: keeps running until the user types `quit` or `exit`.

---

flowchart TD
A[Start Program] --> B[User types mood statement]
B --> C[convert input to lowercase]
C --> D[Check for keywords across all mood categories]
D --> E[Count matches for each mood]
E --> F[Find mood with highest score]
F --> G{Any matches found?}
G -->|Yes| H[Select matching mood]
G -->|No| I[Set mood = neutral]
H --> J[Pick a random quote from mood_quotes]
I --> J
J --> K[Display Detected Mood + Quote]
K --> L[Ask for next input or exit]
L --> M[End]


# 📚 Project Structure

mood-detector/
│        
├── MoodDetector.ipynb                      
└── README.md 