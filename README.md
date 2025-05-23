# 🧠 Automated Neural Architecture Search for Chest X-ray Classification

This project implements an **Automated Neural Architecture Search (NAS)** system using **Genetic Algorithms** and **Reinforcement Learning (Q-Learning)** to automatically design and optimize **Convolutional Neural Network (CNN)** architectures for **chest X-ray image classification**.

## 📌 Objective

The primary goal is to classify chest X-ray images for medical diagnosis (e.g., detecting pneumonia) by **automatically generating the best CNN architecture**, removing the need for manual trial-and-error in model design.

---

## ⚙️ Features

- ✅ Chest X-ray classification using deep learning.
- 🤖 Automated CNN architecture design via:
  - Genetic Algorithms (GA)
  - Q-Learning (Reinforcement Learning)
- 📊 Evaluation metrics: Accuracy, F1-score, ROC-AUC, Confusion Matrix.
- 📁 Image preprocessing and augmentation for better generalization.
- 📈 Logging and visualization of model performance.

---

## 🏗️ Architecture Overview

Data Loader ➝ Preprocessing ➝ CNN Generation (GA / Q-Learning) ➝ Model Training ➝ Evaluation ➝ Best Model


### 🧪 Two Types of CNN Models:
- **Baseline CNN**: Fixed architecture for comparison.
- **Dynamic CNN**: Flexible structure generated by AI algorithms.

---

## 🧬 Genetic Algorithm (GA)

- Initializes a population of random CNNs.
- Selects top-performing architectures based on accuracy.
- Applies crossover and mutation to evolve better models.
- Repeats over several generations to find the best solution.

---

## 🤖 Q-Learning (RL-based NAS)

- Uses Q-Learning to select CNN hyperparameters based on reward signals.
- Learns which architecture actions (e.g., changing filters or layers) lead to improved model performance.
- Stores experience in a Q-table to guide future decisions.

---

## 🗂️ Dataset Structure
dataset/ │ ├── train/ │ ├── NORMAL/ │ └── PNEUMONIA/ │ ├── val/ │ ├── NORMAL/ │ └── PNEUMONIA/ │ └── test/ ├── NORMAL/ └── PNEUMONIA/


- All images are resized to 128x128 and normalized.
- Augmentation includes horizontal flipping.

---

## 📊 Evaluation Metrics

- **Accuracy**
- **Precision, Recall, F1-Score**
- **AUC-ROC Curve**
- **Confusion Matrix**

---


