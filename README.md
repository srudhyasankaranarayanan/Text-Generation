# 🤖 AI Text Generator

A simple web-based **AI Text Generator** built using **Streamlit** and **Hugging Face Transformers**. The application allows users to enter a sentence or short prompt and generates a continuation using the pretrained **Qwen/Qwen2.5-0.5B-Instruct** language model.

## About the Project

This project demonstrates how a pretrained **Transformer language model** can be integrated with a simple interactive Streamlit web interface.

Instead of training a language model from scratch, the application uses the **Qwen/Qwen2.5-0.5B-Instruct** model from Hugging Face. Streamlit provides the user interface for entering prompts and displaying the generated text.

## Features

* Simple text input area
* AI-generated text completion
* Generate Text button
* Loading message while generating
* Separate generated-text output section
* Pretrained Transformer model
* Model caching for faster interaction
* User-friendly Streamlit interface
* Warning message when no input is provided

## Technologies Used

* Python
* Streamlit
* Hugging Face Transformers
* PyTorch
* Qwen/Qwen2.5-0.5B-Instruct

## How It Works

<img width="1086" height="1448" alt="AI Text Generator Workflow" src="https://github.com/user-attachments/assets/1afcb1dc-3561-402d-9cc9-e48fa4cb7e58" />

## Model

The application uses:

```text
Qwen/Qwen2.5-0.5B-Instruct
```

The model is loaded using the Hugging Face Transformers pipeline:

```python
from transformers import pipeline

generator = pipeline(
    "text-generation",
    model="Qwen/Qwen2.5-0.5B-Instruct"
)
```

## Installation

Make sure Python is installed on your system.

Install the required packages:

```bash
pip install streamlit transformers torch
```

## Running the Application

Save the Python program as:

```text
app.py
```

Open a terminal in the project folder and run:

```bash
streamlit run app.py
```

The application will normally open at:

```text
http://localhost:8501
```

## Project Structure

```text
AI-Text-Generator/
│
├── app.py
├── README.md
├── requirements.txt
└── .gitignore
```

## Example

Enter a prompt such as:

```text
Artificial Intelligence is
```

Click **✨ Generate Text** to generate the continuation.

## What This Project Demonstrates

This project provides a practical introduction to:

* Transformer-based language models
* Hugging Face Transformers
* Text generation
* Pretrained AI models
* Streamlit application development
* Model caching
* Connecting an AI model to a web interface
