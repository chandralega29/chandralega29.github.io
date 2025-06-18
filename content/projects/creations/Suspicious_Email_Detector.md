
```json
{
  "title": "Suspicious Email Detector using ML",
  "date": "2025-06-18T12:00:00+05:30",
  "image": "/img/emaildetector.jpg",
  "link": "https://github.com/YourUsername/Suspicious_Email_Detector",
  "description": "An ML-based system that uses NLP to detect suspicious emails by analyzing content using Naive Bayes, SVM, and vectorization techniques such as TF-IDF.",
  "tags": ["Python", "Machine Learning", "NLP", "Email Security", "Streamlit", "Django"],
  "fact": "",
  "featured": true
}
```

# Overview
A **Suspicious Email Detection System** built using **Machine Learning** and **Natural Language Processing (NLP)** to automatically classify emails as *Suspicious* or *Non-Suspicious*. The system uses classifiers like **Naive Bayes** and **SVM**, with vectorization techniques such as **CountVectorizer** and **TF-IDF**.

# Features
- Detects harmful or threatening email content.
- Uses NLP techniques like stemming, lemmatization, and stopword removal.
- Integrates a web interface using **Streamlit** and **Django**.
- Supports **SQLite** for email storage and management.
- Real-time suspicious keyword detection.

# Dependencies
Install the required libraries:
```sh
pip install streamlit sqlite3 scikit-learn pandas numpy nltk
```

# Code Structure

## Core Functions
- `speak(text)`: Converts text to speech.
- `recognize_speech()`: Captures voice input and converts it into text.
- `match_command(command, options)`: Matches spoken commands to predefined options using fuzzy string matching.

## Main Modules
- **Data Gathering**: Loads email data from CSV.
- **Text Preprocessing**: Cleans the email content.
- **Vectorization**: Converts text to numerical data.
- **Classification**: Uses ML models like SVM, Naive Bayes.
- **Prediction**: Predicts whether the email is suspicious or not.

# Usage
1. Run the script with Streamlit.
2. Use the web interface to input email content.
3. System returns Suspicious or Non-Suspicious status.
4. All emails are stored with metadata in SQLite database.

# Sample Code Snippet
```python
def is_suspicious(content):
    suspicious_keywords = ['bomb', 'scam', 'murder', 'kill', 'fraud']
    return any(word in content.lower() for word in suspicious_keywords)
```

# Conclusion
This project offers a scalable, efficient way to filter out suspicious or harmful emails. It combines classic machine learning with robust NLP techniques to analyze email content with high accuracy. Future enhancements may include multilingual detection and deeper context analysis using LLMs or transformer-based models.
