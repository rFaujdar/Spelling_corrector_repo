Deep Learning-Based Spelling Corrector

Project Title

A robust spelling corrector powered by deep learning, capable of identifying and correcting various types of spelling errors with high accuracy.

Description

The Spelling Corrector leverages deep learning approaches to identify and correct misspelled words. It ensures that even within the context of surrounding words, the most appropriate corrections are made. This system goes beyond pointing out errors by suggesting or automatically selecting the correct alternative while retaining already correct words.

Types of Errors Addressed:
	1.	Non-Word Errors: Common typos, e.g., “langage” instead of “language.”
	2.	Real-Word Errors: Incorrect yet valid words, e.g., “three” instead of “there.”
	3.	Cognitive Errors: Mistakes due to confusion or homophones, e.g., “peace” vs. “piece.”
	4.	Short Forms/Slang: Informal or abbreviated text, e.g., “u r kewl.”

The implementation is backed by a sequence-to-sequence model built using the Keras framework with TensorFlow GPU backend.

Table of Contents
	1.	Installation
	2.	How to Use
	3.	Technologies Used
	4.	Workflow
	5.	Features
	6.	Future Enhancements

Installation

Prerequisites
	•	Python: Version 3.6
	•	Anaconda (Recommended)
	•	GPU-compatible environment with CUDA 10 and CuDNN 10 for TensorFlow GPU.

Steps

Using PyCharm:
	1.	Create a new project in PyCharm.
	2.	Navigate to the project directory.
	3.	Set up a virtual environment using Conda with Python 3.6.
	4.	Install dependencies:

pip install -r requirements.txt



Using Conda CLI:
	1.	Create a virtual environment:

conda create -n spell_corrector_env python=3.6


	2.	Activate the environment:

conda activate spell_corrector_env


	3.	Navigate to the project directory and install dependencies:

pip install -r requirements.txt

How to Use
	1.	Start the Flask Server:
	    •	Run clientApp.py to start the web server.
	    •	The server will be hosted at: http://0.0.0.0:5000/.
	2.	Input Misspelled Text:
	    •  	Enter a sentence with misspelled words in the input box.
	    •	Click “Predict” to get corrected suggestions.
	3.	View Results:
	    •	The corrected sentence will be displayed in the results box.

Technologies Used
	•	Programming Language: Python
	•	Deep Learning Framework: Keras (2.2.4) with TensorFlow GPU backend (1.14.0)
	•	Web Framework: Flask
	•	Additional Libraries:
	    •	SymSpellPy: For efficient spelling correction.
	    •	NumPy: For numerical computations.
	    •  	Flask-Cors: For handling cross-origin requests.
	    •	requests: For making API requests.
	    •	pytest and pytest-cov: For testing and coverage reporting.
	    •	cryptography: For secure communications.
	    •	idna and urllib3: For handling HTTP requests.
	    •  	Jinja2 and Werkzeug: For templating and utility functions.
	    •	NumPy, Flask-Cors, requests, pytest, and more (see requirements.txt).

Workflow
	1.	Input Preprocessing:
	    •	Tokenize input sentences.
	    •	Identify errors based on predefined rules or sequence models.
	2.	Sequence-to-Sequence Model:
	    •	Corrects spelling using context from surrounding words.
	    •	Retains correctly spelled words.
	3.	Output Generation:
	    •	Returns corrected text.
	4.	Web Application:
	    •	Flask-based interface for real-time input and output.

Features
	•	Identifies and corrects four types of spelling errors.
	•	Retains correctly spelled words without modification.
	•	User-friendly web interface for testing and predictions.
	•	Scalable deployment using a virtual environment.

Future Enhancements
	•	Integrate pretrained models like BERT or GPT-2 for higher accuracy.
	•	Expand the training dataset to improve model generalization.
	•	Implement a live API for real-time spell-checking in external applications.

Conclusion

This project demonstrates a powerful deep learning-based spelling corrector capable of handling diverse error types effectively. With future enhancements, the system can achieve even greater accuracy and become a critical tool for text processing applications.
