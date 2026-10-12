# Final Project

## Project Name

Final Project - Emotion Detection Application

## Project Overview

This Final Project implements an emotion detection application using
Python and the IBM Watson Natural Language Processing (NLP) library.

The application analyzes a user-provided text statement and identifies
five emotions: anger, disgust, fear, joy, and sadness. It returns a
score for each emotion and determines the dominant emotion based on
the highest score.

## Project Features

- Emotion detection using the Watson NLP EmotionPredict service.
- A Python function named emotion_detector.
- A Python package named EmotionDetection.
- Formatted emotion scores and dominant emotion results.
- Error handling for blank or invalid text input.
- Unit tests that validate the expected dominant emotions.
- A Flask web application that allows users to submit text through a
  browser and view the emotion detection results.
- Static code analysis using Pylint.

## Technologies Used

- Python 3
- IBM Watson NLP EmotionPredict service
- Requests library
- Flask web framework
- Python unittest framework
- Pylint
- HTML, CSS, and JavaScript for the web interface
- Git and GitHub for version control

## Project Structure

    oaqjp-final-project-emb-ai/
    ├── EmotionDetection/
    │   ├── __init__.py
    │   └── emotion_detection.py
    ├── templates/
    │   └── index.html
    ├── static/
    │   └── mywebscript.js
    ├── server.py
    ├── test_emotion_detection.py
    └── README.md

## How It Works

The emotion_detector function sends the input text to the Watson NLP
EmotionPredict endpoint. It processes the JSON response, extracts the
five emotion scores, and identifies the dominant emotion.

The Flask application provides a web interface through which users can
submit statements for analysis. The application displays the resulting
emotion scores and the dominant emotion. Blank input is handled with
an error message.

## Running the Application

Install the required Python dependencies if they are not already
available in the development environment:

    python3 -m pip install requests flask

Run the Flask application from the project directory:

    python3 server.py

The application listens on port 5000. Open the application using
http://localhost:5000/ or the appropriate port preview provided by
the Cloud IDE.

## Running the Unit Tests

Run the unit tests from the project directory:

    python3 -m unittest -v test_emotion_detection.py

The tests check the expected dominant emotion for statements expressing
joy, anger, disgust, sadness, and fear.

## Error Handling

The application handles blank input and can return an appropriate
error message when the text cannot be analyzed.

## Project Objective

The objective of this Final Project is to demonstrate how a natural
language processing service can be integrated into a Python
application, tested using unit tests, and deployed through a Flask
web interface.
