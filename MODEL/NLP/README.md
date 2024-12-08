# Illegal Job Post Filtering Using NLP

This repository implements an NLP model to identify and filter job postings that fall into illegal or inappropriate categories. The model ensures compliance with ethical and legal standards by automatically flagging prohibited content.

---

## Table of Contents

- [Project Description](#project-description)  
- [Dataset](#dataset)  
- [Model](#model)  
- [Requirements](#requirements)    
- [Installation](#Installation) 
---

## Project Description

This project involves building a Natural Language Processing (NLP) model to identify and filter job postings that fall into illegal or inappropriate categories. The primary objective is to prevent these types of jobs from being listed on a platform, ensuring compliance with ethical and legal standards.

---

## Dataset
Access the dataset from the following link:  
**[Dataset Link](https://drive.google.com/drive/folders/1joe-qILoh7lGZ0cYAKrrRAG8Le3aE6pE?usp=sharing)**

---

## Model

model, trained weights, and configuration files are available for download:  
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

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository.git
