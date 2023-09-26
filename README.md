# Intro-To-ML-and-AI-Tokenization-and-NLP-Lab
 
# NLP Exploration Lab: Dive into `transformers`!

Hello, Developers! 🎉 After our dive into tokenization and Natural Language Processing (NLP) models, it's time to get hands-on!

## 🚀 **Objective:**

- Familiarize with the `transformers` library by Hugging Face.
- Set up a simple Flask application integrated with a model from the library.

## 🛠 **Setup**:

### 1. **Installation**

Begin by installing the `transformers` library:
```bash
pip install transformers
```

### 2. Exploring `transformers`

Navigate to the [official documentation of `transformers`](https://huggingface.co/docs/transformers/index). Familiarize yourself with the models, tools, and various features available.

### 3. Model Selection

Choose a model from the `transformers` library that interests you, such as BERT, GPT-2, T5, or any other. Consider its potential applications, like sentiment analysis, text completion, or translation.

## 🔍 **Your Main Task**

### 1. Flask Application Setup

Begin by setting up a basic Flask application structure. You'll be creating a simple Flask server where users can access:

```python
from flask import Flask
app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, NLP Explorer!"

if __name__ == "__main__":
    app.run(debug=True)
```
### 2. Integrating the Model

With your Flask application initialized, it's time to integrate a model from Hugging Face's `transformers` library. Here's how:

1. **Import the Necessary Modules**

  - Begin by ensuring you've imported the essential libraries.
    1. Load your chosen model using the Hugging Face's pipeline
    2. Replace `task_name` with the task you want (e.g., 'sentiment-analysis', 'translation', etc.)
    3. Replace `model_name_from_hugging_face` with the model you selected.

   ```python
   from transformers import pipeline
   model = pipeline("task_name",model='model_name_from_higging_face')
   text = ["input"]
   predictions = model(text)
```
### 3. Linking Flask with Transformers and Adding a User Interface

1. **Extend the Flask route to get user input from a simple HTML form and process it using the loaded NLP model.**
  
2. **Design a simple HTML file in to render the predictions' results**
  
3. **Update your Flask route to handle the requests, process the text using the model, and render the results on the HTML page**
   
 ****Great job!****
  ****Call an Instructor/TA to check your completed tasks****

## Challenge 🌟
 - Extend your Flask application with additional functionalities or routes.
 - Add frontend and style for better user interactivity.

Remember, the journey is more important than the destination. Don't hesitate to ask if you're stuck. Happy coding! 🎉
