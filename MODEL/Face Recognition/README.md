# Face Recognition Using Siamese Network

This repository implements a face recognition system using a Siamese network for one-shot learning. The model is designed to verify if two images belong to the same individual, making it ideal for applications like authentication systems and personalized identification.

---

## Table of Contents

- [Project Description](#project-description)  
- [Dataset](#dataset)  
- [Model](#model)  
- [Requirements](#requirements)    

---

## Project Description

Siamese networks are a type of neural network architecture used for comparing two inputs. In this project, the network is trained to minimize the distance between embeddings of the same person while maximizing the distance between embeddings of different people. This one-shot learning approach allows for face verification with minimal training data for each individual.

---

## Dataset
Access the dataset from the following link:  
**[Dataset Link](https://drive.google.com/drive/folders/1EFTR64jY3QG6-EsGIOFo4DqNNR5d6FN_?usp=sharing)**  
---

## Model

The Siamese network model, trained weights, and configuration files are available for download:  
**[Model Link](https://drive.google.com/drive/folders/1ErdRRtFBbMts9hsJTAf8K5auyrjyqEt0?usp=sharing)**  

The model architecture uses convolutional layers to extract features, followed by a contrastive loss function to optimize similarity between embeddings.

---

## Requirements

The following dependencies are required:  

- Python 3.8+
- TensorFlow/Keras
- NumPy
- OpenCV
- Matplotlib
- Pandas
- Scikit-learn  
