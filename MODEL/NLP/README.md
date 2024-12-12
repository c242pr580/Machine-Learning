# Illegal Job Post Filtering Using NLP

This repository implements an NLP model to identify and filter job postings that fall into illegal or inappropriate categories. The model ensures compliance with ethical and legal standards by automatically flagging prohibited content.

---

## Table of Contents

- [Project Description](#project-description)  
- [Dataset](#dataset)  
- [Model](#model)  
- [Requirements](#requirements)    
- [Installation](#installation)  
- [Features](#features)  
- [Files](#files)  
- [Usage](#usage)  
- [Testing](#testing)  
- [Limitations](#limitations)  
- [Technical Details](#technical-details)  
- [Future Improvements](#future-improvements)  
- [License](#license)

---

## Project Description

This project involves building a Natural Language Processing (NLP) model to identify and filter job postings that fall into illegal or inappropriate categories. The primary objective is to prevent these types of jobs from being listed on a platform, ensuring compliance with ethical and legal standards.

---

## Dataset
Access the dataset from the following link:  
**[Dataset Link](https://drive.google.com/drive/folders/1joe-qILoh7lGZ0cYAKrrRAG8Le3aE6pE?usp=sharing)**

---

## Model

Model, trained weights, and configuration files are available for download:  
**[Model Link](https://drive.google.com/drive/folders/1QoycjXXtm8qTJSDlgfQhJPTRGHEF6L5G?usp=sharing)**  

The model architecture uses an embedding layer for text representation, followed by bidirectional LSTM layers to capture contextual features, and dense layers for binary classification.

---

## Requirements

The following dependencies are required:  

- Python 3.8+
- tensorflow==2.15.0
- NumPy
- Matplotlib
- Pandas
- Scikit-learn

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/c242pr580/Machine-Learning.git
   ```
2. Install the required dependencies:
   ```bash
   cd NLP
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Features
- **Job Title Prediction**: Input a job title to predict whether it is "Legal" or "Illegal."
- **Model Loading**: The TensorFlow.js model is dynamically loaded from a `model.json` file.
- **Vocabulary Handling**: A vocabulary file (`vocab.txt`) is loaded to tokenize and vectorize input text.
- **Real-time Predictions**: The model processes user input and displays predictions instantly.

---

## Files
1. `tes_model_Tfjs.html`: Main HTML file containing the code for the demo.
2. `model.json`: TensorFlow.js model configuration file.
3. `vocab.txt`: Vocabulary file used for text processing.
4. `nlp6.ipynb`: Jupyter notebook for preprocessing or training the TensorFlow.js-compatible model.

---

## Usage

### 1. Setting up the Project
1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Install the required dependencies:
   ```bash
   cd NLP
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Ensure the `model.json` and `vocab.txt` files are in the same directory as the HTML file.

### 2. Running the Demo
1. Open the `tes_model_Tfjs.html` file in a web browser.
2. Input a job title in the provided text box.
3. Click the "Prediksi" button to see the result.
4. Use the "Reset" button to clear the input and output fields.

### 3. Model and Vocabulary
- The TensorFlow.js model (`model.json`) should be exported from TensorFlow or converted using the TensorFlow.js converter.
- The vocabulary file (`vocab.txt`) should include tokens, with `[UNK]` representing unknown words.

---

## Testing
1. Ensure that `tes_model_Tfjs.html`, `model.json`, and `vocab.txt` are in the same directory.
2. Open the `tes_model_Tfjs.html` file in a browser.
3. Input a variety of job titles, including those expected to be flagged as "Illegal."
4. Verify predictions are consistent with expectations.
5. Observe the console for logs and any potential errors.

---

## Limitations
- The model's accuracy depends on the quality and coverage of the training dataset.
- Predictions may not account for nuanced contexts or phrases outside the vocabulary.
- Current implementation supports Indonesia only.

---

## Technical Details
- **Prediction Logic**:
  1. Input text is tokenized and converted into numerical vectors based on the vocabulary.
  2. The vectors are padded to a fixed length (default: 50 tokens).
  3. The TensorFlow.js model processes the vectors and outputs predictions.
  4. Predictions are classified as "Legal" or "Illegal" based on a confidence threshold (default: 0.5).

- **Error Handling**:
  - If the model or vocabulary fails to load, error messages are displayed on the webpage.
  - Invalid inputs (e.g., empty text) are rejected.

---

## Future Improvements
- Expand dataset coverage to include multiple languages and regional job-specific nuances.


---

## License
This project is open-source and available under the [MIT License](LICENSE).

