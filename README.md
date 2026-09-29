# AI Attention Visualizer

##  Project Overview

AI Attention Visualizer is a Streamlit-based application that extracts text from an uploaded image using Optical Character Recognition (OCR), creates word embeddings, calculates attention scores, and visualizes the attention given to each word.

This project demonstrates the basic workflow of an AI attention mechanism using image text, embeddings, and attention scores.

##  Live Demo

https://ai-attention-visualizer-k2rt28q4vpvcmsrt4e2abb.streamlit.app/

##  Features

* Upload JPG, JPEG, and PNG images
* Extract text from images using OCR
* Create word embeddings using Sentence Transformers
* Calculate attention scores using NumPy
* Display word-level attention scores
* Identify the word with the highest attention
* Show total number of processed words
* Simple and interactive Streamlit interface

##  Project Workflow

```text
Upload Image
     ↓
OCR Text Extraction
     ↓
Word Processing
     ↓
Word Embeddings
     ↓
Attention Calculation
     ↓
Attention Scores
     ↓
Visualization
```

##  Technologies Used

* Python
* Streamlit
* NumPy
* Pillow
* PyTesseract
* Tesseract OCR
* Sentence Transformers
* `all-MiniLM-L6-v2`

##  Project Structure

```text
AI Attention Visualizer/
│
├── app.py
├── ocr.py
├── embedding.py
├── attention.py
├── requirements.txt
├── packages.txt
└── README.md
```

##  File Description

### `app.py`

Main Streamlit application. It handles image upload, OCR output, word processing, embeddings, attention calculation, and visualization.

### `ocr.py`

Extracts text from the uploaded image using PyTesseract and Tesseract OCR.

### `embedding.py`

Creates word embeddings using the Sentence Transformer model `all-MiniLM-L6-v2`.

### `attention.py`

Calculates attention scores using Query, Key, Value (QKV), scaled dot-product attention, and softmax.

### `requirements.txt`

Contains the required Python packages.

### `packages.txt`

Contains the system-level Tesseract OCR package required for deployment.

##  Installation

Install the required Python packages:

```bash
pip install -r requirements.txt
```

##  Run the Application

Run the following command in the project folder:

```bash
streamlit run app.py
```

The application will open in the browser.

##  How to Use

1. Open the Streamlit application.
2. Upload an image containing text.
3. The application extracts the text using OCR.
4. The extracted text is divided into words.
5. Word embeddings are generated.
6. Attention scores are calculated.
7. The attention score of each word is displayed using progress bars.
8. The word with the highest attention score is displayed in the summary section.

##  Output

The application displays:

* Input Image
* Extracted Text
* Word Attention Scores
* Highest Attention Word
* Highest Attention Score
* Total Number of Words

##  Deployment

The application can be deployed using Streamlit Community Cloud.

For deployment, make sure the repository contains:

```text
app.py
ocr.py
embedding.py
attention.py
requirements.txt
packages.txt
README.md
```

##  Objective

The main objective of this project is to demonstrate how OCR, word embeddings, and an attention mechanism can be combined to visualize word-level attention in an AI application.

