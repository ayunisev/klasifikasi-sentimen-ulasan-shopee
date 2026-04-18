# Shopee Review Sentiment Classification

This project aims to perform **sentiment classification** on **Indonesian-language reviews** of the **Shopee** application on the **App Store**.  
The analysis is conducted to classify user reviews into **positive**, **neutral**, and **negative** sentiments using several machine learning and deep learning algorithms.

## Background

User reviews on digital platforms are very important for understanding service quality and user satisfaction. Through sentiment analysis, a collection of reviews can be transformed into more structured information, which can help evaluate an application.

In this project, Shopee review data is processed through several stages, including scraping, cleaning, preprocessing, and classification model training.

## Project Objectives

- Collect Shopee application review data
- Clean and preprocess the review text
- Perform sentiment classification into 3 classes
- Compare the performance of several algorithms
- Determine the best-performing model

## Sentiment Categories

This project uses **3 sentiment classes**, namely:

- **Positive**
- **Neutral**
- **Negative**

## Workflow

1. **Data Scraping**  
   Collecting Indonesian-language Shopee application reviews from the App Store.

2. **Cleaning and Preprocessing**  
   The preprocessing steps include:
   - case folding
   - text cleaning
   - tokenization
   - stopword removal
   - stemming

3. **Data Labeling**  
   The review data is labeled into three sentiment categories: positive, neutral, and negative.

4. **Model Training**  
   The models used are:
   - **SVM (Support Vector Machine)**
   - **Dense Neural Network**
   - **BiLSTM**

5. **Model Evaluation**  
   The evaluation is carried out by comparing the performance of the models in 3-class sentiment classification.

## Algorithms Used

### 1. Support Vector Machine (SVM)

SVM is used as a classification model based on transformed text features.

### 2. Dense Neural Network

The Dense Neural Network model is used to learn sentiment patterns from text feature representations in a more complex way.

### 3. BiLSTM

BiLSTM is used to capture the contextual sequence of words in review texts, enabling it to better understand language patterns.

## Accuracy Results

Based on the test results, the model performances are as follows:

| Model | Training Accuracy | Testing Accuracy |
|------|------------------:|----------------:|
| SVM | 96.9% | 88.93% |
| Dense Neural Network | 99.29% | 92.10% |
| BiLSTM | 98.34% | 93.4% |

## Conclusion

Based on the evaluation results, the **BiLSTM** model achieved the best performance on the testing data compared to the other models.  
This model reached a testing accuracy of approximately **93.4%**, making it the best model for classifying **Indonesian-language Shopee application reviews** into three sentiment classes.
