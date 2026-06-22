# Emotion Detection System

A final project submission for the IBM Backend Development course. This application analyzes text blocks to determine individual emotion scores ('anger', 'disgust', 'fear', 'joy', and 'sadness') alongside the 'dominant_emotion' utilizing the Watson NLP Emotion Predict API through a cleanly designed Flask web server.

---

## Project Structure & Task Files

This repository contains the complete execution history organized by specific project tasks and deliverables:

### 1. Emotion Detection Package (`EmotionDetection/`)
* **`__init__.py`** (Task 4: Activity 1) -> Initializes the `EmotionDetection` directory as a structured Python package and exposes the detector interface.
* **`2a_emotion_detection`** (Task 2: Activity 1) -> The raw initial module function creating the API POST request to Watson NLP.
* **`3a_output_formatting`** (Task 3: Activity 1) -> Updated module script that extracts the key metrics and returns the structured response dictionary.
* **`7a_error_handling_function`** (Task 7: Activity 1) -> Final version of the function that cleanly intercepts `400` status codes for empty inputs and returns dictionary values set to `None`.

### 2. Validation & Terminal Outputs
* **`2b_application_creation`** (Task 2: Activity 2) -> Terminal snapshot proving successful application import and baseline function check.
* **`3b_formatted_output_test`** (Task 3: Activity 2) -> Terminal output recording the validation of the correctly structured response dictionary containing the metrics and the dominant emotion.
* **`4b_packaging_test`** (Task 4: Activity 2) -> Terminal validation log confirming that `EmotionDetection` functions correctly as an imported package module.

### 3. Automated Unit Testing
* **`5a_unit_testing`** (`test_emotion_detection.py`) (Task 5: Activity 1) -> Comprehensive Python unit testing file checking joy, anger, disgust, fear, and sadness edge cases via standard assertions.
* **`5b_unit_testing_result`** (Task 5: Activity 2) -> Validation output confirming all 5 unit tests ran and passed cleanly using `pytest`.

### 4. Flask Server Implementation (`server.py`)
* **`6a_server`** (Task 6: Activity 1) -> Initial implementation setup of the Flask engine, incorporating routing for `/` and `/emotionDetector`.
* **`7b_error_handling_server`** (Task 7: Activity 2) -> Enhanced web code returning `"Invalid text! Please try again."` if user interface strings evaluate to an empty condition.
* **`8a_server_modified`** (Task 8: Activity 1) -> The final clean execution server script containing explicit, PEP-257 compliant docstrings designed to satisfy static analyzers.
* **`8b_static_code_analysis`** (Task 8: Activity 2) -> Terminal analysis output proving a perfect static script score code metric of `10.00/10` when parsed with `pylint`.

---

## Technical Specifications
* **Language:** Python 3.11
* **Framework:** Flask
* **API Platform:** Watson NLP Runtime Services (EmotionPredict Engine)
