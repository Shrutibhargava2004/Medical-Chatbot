# MediTrain - Medical Chatbot

## Overview

MediTrain is an AI-powered medical assistant designed to provide users with accurate, empathetic, and clear answers to medical queries. Built using open-source AI models and Flask, MediTrain emphasizes user-friendly interactions while ensuring that users are reminded to seek professional healthcare advice for proper diagnosis and treatment.

## Features

* **Simulated Patient for Trainee Doctors**: Interacts as a virtual patient, describing symptoms and responding dynamically to follow-up questions from users acting as doctors.
* **Store Conversation History**: Stores the conversations of every session for future use.
* **Medical Focus**: Tailored to assist with general medical questions while avoiding direct diagnoses.
* **Flask-Based UI**: Intuitive and interactive web-based interface for seamless user interaction.
* **Empathetic Responses**: Ensures responses are clear, considerate, and accurate.
* **Text-to-Speech Functionality**: Allows users to listen to chatbot responses for a more accessible experience.
* **Disease Prediction**: Supports prediction of diseases like diabetes, Alzheimer's disease, and heart disease.

## Prerequisites

To run MediTrain locally, ensure you have the following:

* Python 3.8+
* Libraries specified in `requirements.txt`
* A medical book in PDF format (used for chatbot training)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Shrutibhargava2004/MediTrain-AI.git
   cd MediTrain-AI
   ```
2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Place your `medical_book.pdf` and any related data files (e.g., JSON) in the `data` folder.

## Usage

1. Run the Flask application:
   ```bash
   python app.py
   ```
2. Open the application in your browser (default: [http://localhost:5000](http://localhost:5000/)).
3. Create an account and log in to access the chat.
4. Choose between:
   - **General Medical Chatbot**: Ask medical queries.
   - **Simulated Patient Mode**: Act as a virtual patient.
5. Use the text-to-speech button to listen to chatbot responses.

## Project Structure

* **`app.py`**: Main Flask application script.
* **`data/`**: Contains training data, including `medical_book.pdf` and JSON files.
* **`requirements.txt`**: List of required Python packages.
* **`static/`**: Contains static assets like CSS and JavaScript files.
* **`templates/`**: HTML templates for the Flask application.
* **`model/`**: Trained models for various disease predictions.
* **`sample/`**: Contains the code for text preprocessing and storing data.

## Key Libraries

* **Flask**: For building the user interface.
* **PyPDF2**: For extracting data from the medical book in PDF format.
* **NLTK**: For natural language processing.
* **gTTS**: For text-to-speech functionality.
* **Mistral-7B-Instruct-v0.3**: For generating response in medical queries asked by patient.
* **LLaMA API from Groq**: For generating responses in simulated patient mode.
* **Python-dotenv**: For managing environment variables.

## Important Notes

* MediTrain is designed as a medical assistant but does not provide medical diagnoses or treatment plans.
* The simulated patient feature is meant for educational purposes and should not replace real patient interactions.
* Always consult a certified healthcare professional for medical concerns.

## Future Enhancements

* Add support for multilingual queries.
* Enhance conversation memory to retain context over extended sessions.
* Introduce additional models for region-specific medical advice.
* Implement real-time voice-based interaction.
* Expand the simulated patient feature to include different case complexities and medical histories.

## License

This project is licensed under the MIT License.

---

Enjoy using MediTrain and let us know if you have suggestions or encounter issues!
