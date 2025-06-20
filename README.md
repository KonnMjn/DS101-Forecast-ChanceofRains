# 🌧️ Rainfall Prediction Project

This project aims to predict the probability of rainfall the next day using multiple approaches including Naive Bayes, Markov Chains, and Monte Carlo simulation with Logistic Regression. 

---

## 📌 Table of Contents

- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [How to Run](#how-to-run)
- [License](#license)
- [Credits](#credits)

---

## 📁 Project Structure

```
rain-prediction-project/
├── cleaned_weatherAUS.csv # Weather dataset
├── main.ipynb # Jupyter notebook with full implementation
├── Project Report.pdf 
├── Project Presentation.pptx
├── .gitignore 
├── requirements.txt 
├── README.md 
```

---

## 📦 Dataset

- **Source**: The dataset was originally obtained from [Rain in Australia - Cleaned Dataset](https://www.kaggle.com/datasets/caillemaxence/rain-in-australia-cleaned-dataset) and cleaned to `cleaned_weatherAUS.csv`.
- **Description**: Contains weather observations from various locations in Australia, including temperature, humidity, wind, and rainfall.
- **Target variable**: `RainTomorrow` – a binary label indicating whether it will rain the next day.
- Missing values and irrelevant columns were removed in the preprocessing step.

---

## 🧠 Methodology

This project applies three statistical and machine learning methods to predict rainfall:

### 1. Naive Bayes Classifier
- Uses Gaussian Naive Bayes to model continuous weather features.
- Applies log-probabilities and Laplace smoothing.
- Softmax is used to compute class probabilities.

### 2. Markov Chains
- Models rain as a two-state Markov process: "Rain" and "No Rain".
- Computes transition probabilities and uses matrix powers to forecast future states.

### 3. Monte Carlo Simulation + Logistic Regression
- Simulates data distributions for `Rain` and `No Rain` from Gaussian assumptions.
- Trains Logistic Regression repeatedly on simulated data.
- Evaluates and averages results over 100 simulations for performance stability.

**Metrics used**: Accuracy, Precision, Recall, and Confusion Matrix.

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/KonnMjn/DS101-Rain-Prediction.git
cd DS101-Rain-Prediction
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```
### 3. Open the Jupyter notebook
```bash
jupyter notebook notebook/main.ipynb
```
You can run each section step by step and modify parameters to test different settings.

---

## 📄 License
📌 Code components are licensed under the MIT License, allowing reuse, modification, and distribution with attribution and no warranty.

📎 Non-code contents are shared under the Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0), allowing reuse with attribution for non-commercial purposes.

---

## 👨‍🏫 Credits

Phạm Đông Hưng – 22520521

Lương Anh Huy - 22520550

Phan Công Minh - 22520884

Hồng Khải Nguyên - 22520967

Instructor: TS. Dương Ngọc Hảo

---
