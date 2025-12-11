# 🎙️ Distributed Speech Emotion Recognition using PySpark

## 📌 Overview
This project implements a scalable **Big Data analytics pipeline** for Speech Emotion Recognition (SER). Utilizing **Apache Spark (PySpark)** for distributed processing and **Deep Learning (Multilayer Perceptron)** for classification, the system detects 7 distinct emotions (Neutral, Happy, Sad, Angry, Fear, Disgust, Surprise) from raw audio files.

## 🚀 Key Features
* **Distributed Processing:** Uses PySpark for data ingestion and parallel feature extraction.
* **Feature Engineering:** Extracts MFCCs, RMS Energy, Zero Crossing Rate, and Chroma features using Librosa.
* **Deep Learning Model:** Implements a Multilayer Perceptron (MLP) classifier using Spark MLlib.
* **Interactive Demo:** Integrated **Gradio** web interface for real-time microphone testing.

## 🛠️ Technologies Used
* **Big Data:** Apache Spark, PySpark, Hadoop (Simulated)
* **Machine Learning:** Spark MLlib (Random Forest & MLP)
* **Audio Processing:** Librosa
* **Visualization:** Seaborn, Matplotlib

## 📊 Performance
The Multilayer Perceptron (MLP) model significantly outperformed traditional methods:

| Model | Accuracy | F1-Score |
| :--- | :--- | :--- |
| **Multilayer Perceptron (MLP)** | **97.85%** | **0.97** |
| Random Forest (Baseline) | 32.28% | 0.25 |

## 📂 Dataset
* **Source:** RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
* **Size:** ~1,440 Audio Files
* *Note: The code automatically downloads and processes the dataset.*

## 💻 How to Run
1. Open the `.ipynb` file in **Google Colab**.
2. Run the "Environment Setup" cell to install Java 11 and Spark.
3. Run all cells to download data, train the model, and launch the Gradio app.

---
*Inspired by the Big Data Analytics Lab Mini Project (2025)*
