Emotion Classification of Natural Language

This repository contains the implementation of a natural language emotion classification project. This project was developed as part of the CS 3780/5780 Creative Project, showcasing the application of machine learning techniques to classify emotions from textual data.

Project Overview

Emotion classification is a crucial aspect of natural language processing (NLP) that enables machines to understand and respond to human emotions. This project:
Implements emotion classification using advanced machine learning frameworks.
Explores techniques like data preprocessing, feature extraction, and model training.
Leverages popular Python libraries, such as TensorFlow, PyTorch, and scikit-learn, for efficient computation and experimentation.

Problem Formulation

This problem is a multi-class text classification task, where the objective is to classify a piece of text into one of 28 predefined emotion classes. The goal was to design a model that could predict the emotion expressed in a given text based on its content.

Learning Methods Used

Two learning methods were chosen for this project:

Convolutional Neural Networks (CNN):

CNN is a type of deep learning and supervised learning method. Since we are working with labeled data where each piece of text is associated with an emotion class (label), the learning method chosen is supervised learning.
Within the code, Bag of Words (BoW) extraction was used for feature extraction. BoW counts the frequency of each word in a document, providing a direct representation of text that the CNN can process. While BoW does not account for word order, it is simple and often works well for text classification tasks.

Transformer Model - DistilBERT:

DistilBERT, a lightweight version of BERT, was selected for its ability to effectively classify texts into 28 emotion labels. Like the CNN model, DistilBERT uses supervised learning.
Unlike BoW, DistilBERT leverages attention mechanisms to capture the relationships between words, making it particularly suited for tasks involving nuanced text like emotion classification. This approach improves the accuracy of predictions by considering word context and order.

Model Selection

For the CNN model, we prioritized simplicity and efficiency in handling labeled datasets, choosing BoW for its straightforward implementation.
For the Transformer model, DistilBERT was selected due to its balance between performance and computational efficiency, offering robust contextual understanding essential for emotion classification.

Performance Evaluation

The test performance of both models was evaluated against the baseline "Tiny Piney."
CNN Model: Scored a 0.66, which does not reach the first baseline "Tiny Piney."
DistilBERT Model: Scored a 0.77, successfully reaching the baseline "Tiny Piney."
