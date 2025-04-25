# Emotion Classification of Natural Language

This repository contains the implementation of a Natural Language Processing (NLP) project focused on **emotion classification**. Developed as part of the **CS 3780/5780 Creative Project**, the goal was to explore the application of modern machine learning techniques to detect emotions in textual data.

---

## 📌 Project Overview

Emotion classification is a vital subdomain of NLP, enabling machines to interpret and respond to human emotions embedded in text. This project demonstrates:

- Implementation of multi-class emotion classification using supervised learning.
- Utilization of key NLP techniques including data preprocessing, feature extraction, and model training.
- Experimentation with cutting-edge Python libraries such as **TensorFlow**, **PyTorch**, and **scikit-learn**.

---

## 🧠 Problem Formulation

The task is formulated as a **multi-class text classification problem**, where each input sentence must be categorized into one of **28 predefined emotion classes**.

Given a sentence, the objective is to predict the dominant emotion expressed based on its semantic and syntactic features.

---

## 🛠️ Methods Used

### 1. Convolutional Neural Network (CNN)

- A **supervised learning** approach was employed using a CNN architecture.
- Feature extraction was handled through the **Bag of Words (BoW)** model, which captures word frequency to generate input features.
- Although BoW does not preserve word order, it offers simplicity and effectiveness in text classification tasks.

### 2. Transformer-Based Model: DistilBERT

- A compact and efficient version of BERT, **DistilBERT** leverages attention mechanisms to understand word context and relationships.
- It was chosen for its high accuracy and relatively low computational cost.
- DistilBERT processes the text holistically, capturing nuanced emotional expressions that traditional models might overlook.

---

## 🔍 Model Selection Rationale

- **CNN with BoW** was selected for its ease of implementation and suitability for structured, labeled datasets.
- **DistilBERT** was preferred for its deep contextual understanding and strong performance in capturing emotion-rich expressions in natural language.

---

## 📊 Performance Evaluation

Model performance was assessed against the baseline model **"Tiny Piney"**.

| Model         | Accuracy | Baseline Reached     |
|---------------|----------|----------------------|
| CNN (BoW)     | 0.66     | ❌ Below baseline     |
| DistilBERT    | 0.77     | ✅ Above baseline     |

DistilBERT successfully surpassed the performance threshold set by the baseline, showcasing the benefits of transformer-based models in emotion classification tasks.

---

## 📂 Tech Stack

- Python 3.x  
- TensorFlow / Keras  
- PyTorch / HuggingFace Transformers  
- scikit-learn  
- Pandas / NumPy  

---

## 🚀 Getting Started

To reproduce the results:

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# Install dependencies
pip install -r requirements.txt
