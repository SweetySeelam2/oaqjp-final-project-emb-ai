# Final project

## AI-Based Emotion Detection Web Application

This project is a Flask-based AI web application developed using the IBM Watson NLP Emotion Prediction API. The application analyzes user-entered text and detects emotions such as joy, anger, sadness, fear, and disgust.

The project was developed as part of the IBM Skills Network Final Project: *AI-Based Web Application Development and Deployment*.

---

## Features

- Emotion detection using Watson NLP API
- Detects:
  - Joy
  - Anger
  - Fear
  - Sadness
  - Disgust
- Returns dominant emotion
- Flask web deployment
- Error handling for blank inputs
- Unit testing included
- Pylint score: **10/10**

---

## Technologies Used

- Python 3
- Flask
- Requests
- Watson NLP API
- Pylint

---

## Project Structure

```text
final_project/
│
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
│
├── static/
│   └── mywebscript.js
│
├── templates/
│   └── index.html
│
├── server.py
├── test_emotion_detection.py
├── README.md
└── LICENSE
```

---

## Emotion Detection API

The application uses the IBM Watson NLP Emotion Prediction API.

**API Endpoint**
```
https://sn-watson-emotion.labs.skills.network/v1/watson.runtime.nlp.v1/NlpService/EmotionPredict
```

**Request Format**
```
{
  "raw_document": {
    "text": text_to_analyze
  }
}
```

---

## Installation

Clone the repository:
```
git clone https://github.com/SweetySeelam2/oaqjp-final-project-emb-ai.git
```

Navigate into the project folder:
```
cd oaqjp-final-project-emb-ai
```

Install dependencies:
```
pip install flask requests pylint
```

---

## Run the Application

Start Flask server:
```
python3 server.py
```

Application runs on:
```
http://127.0.0.1:5000
```

---

## Example Output

Input:
```
I think I am having fun
```

Output:
```
For the given statement, the system response is 'anger': 0.029103195, 'disgust': 0.0067921067, 'fear': 0.027528232, 'joy': 0.876574 and 'sadness': 0.06151191. The dominant emotion is joy.
```

---

## Error Handling

Blank input handling has been implemented.

Example:
```
Invalid text! Please try again!
```

---

## Unit Testing

Run tests using:
```
python3 test_emotion_detection.py
```

*Expected output:*
```
All tests passed!
```

---

## Static Code Analysis

**Run pylint:**
```
pylint server.py
```

**Pylint Score:**
```
10.00/10
```

---

## Author

Sweety Seelam

GitHub:
https://github.com/SweetySeelam2

---

## License

This project is licensed under the Apache 2.0 License.
