# AI Email Classification Using Deep Learning (BERT)

## Project Overview

This project aims to automate the classification of email inquiries into three categories using **deep learning** techniques, specifically leveraging the **BERT (Bidirectional Encoder Representations from Transformers)** model. BERT is a pre-trained natural language processing (NLP) model based on transformers, known for its ability to capture both local and global context within text sequences.

The model is fine-tuned on a custom dataset of email inquiries related to **Product A**, **Product B**, and **Product C**, and is trained to classify these emails into their corresponding categories.

## Problem Statement

Classifying emails into predefined categories is a common task in automating customer support and streamlining communication. This project demonstrates the use of deep learning models (BERT) to automatically categorize emails based on their content, improving the efficiency of handling product inquiries.

## Approach

1. **Data Preprocessing**: 
   - **Tokenization**: Emails are tokenized into smaller units (tokens) using the BERT tokenizer.
   - **Padding**: Sequences are padded to ensure they are of uniform length, making them compatible with the BERT model.
   
2. **Model Architecture**:
   - The project uses a pre-trained **BERT** model (`bert-base-uncased`).
   - A **classification layer** is added on top of BERT to map the output to one of three categories: Product A Inquiry, Product B Inquiry, and Product C Inquiry.

3. **Fine-Tuning**:
   - The BERT model is fine-tuned on the labeled dataset, adjusting its weights to optimize for email classification.
   
4. **Evaluation**: 
   - The model is evaluated on a test set, and key metrics such as **accuracy**, **precision**, **recall**, and **F1-score** are calculated to assess the model's performance.

## Results

The model achieved **100% accuracy** on the test set, demonstrating its effectiveness in classifying email inquiries into the correct categories.

- **Precision, Recall, and F1-score** for all classes (Product A, Product B, Product C) are **1.00**, indicating excellent performance across all categories.

## Model Details

- **Model Used**: BERT (`bert-base-uncased`), a pre-trained transformer model.
- **Classification Layer**: A dense layer added to BERT for sequence classification, outputting three classes.
- **Fine-Tuning**: The model was fine-tuned using the provided dataset of email texts and their labels.

## Files Included

- **Email_Classification.ipynb**: The Python script that defines the BERT model and fine-tunes it on the email dataset.
A sample dataset containing email texts and their corresponding labels (Product A, Product B, Product C).
A Python script to run the trained model on new email texts and classify them.
A file listing the necessary dependencies for running the project, such as `torch`, `transformers`, and `sklearn`.

## How to Run

1. Clone this repository or download the files.
   ```bash
   git clone https://github.com/yourusername/AI-Email-Classification-Assignment.git
