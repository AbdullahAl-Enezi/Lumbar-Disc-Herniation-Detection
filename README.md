# 🧠 Lumbar MRI Disc Classification using Classical Machine Learning

## 📌 Overview

This project presents a complete machine learning pipeline for classifying lumbar spine MRI images into two categories:

* **Normal**
* **Herniated Disc**

The system is built using **classical machine learning algorithms** combined with **feature engineering, PCA dimensionality reduction, and image preprocessing techniques**.

---

## 🎯 Objectives

* Build a robust ML pipeline for MRI classification
* Compare multiple classical algorithms
* Analyze the impact of:

  * PCA (dimensionality reduction)
  * Image smoothing (bilateral filtering)
* Achieve strong performance using lightweight models (no deep learning)

---

## 🗂️ Dataset

* Source: MRI lumbar spine images
* Classes:

  * `Normal`
  * `Abnormal`
* Images are:

  * Converted to grayscale
  * Resized (224×224)
  * Flattened into feature vectors

---

## ⚙️ Methodology

### 1️⃣ Preprocessing

* Grayscale conversion
* Image resizing
* Bilateral smoothing (optional)
* Normalization (0–1 scaling)

---

### 2️⃣ Feature Representation

* Flattened pixel features (~50,176 features per image)

---

### 3️⃣ Dimensionality Reduction

* **PCA (Principal Component Analysis)**
* Extensive sweep over multiple components

---

### 4️⃣ Models Used

The following algorithms were evaluated:

* K-Nearest Neighbors (KNN)
* Support Vector Machine (RBF)
* Logistic Regression
* Decision Tree
* Random Forest
* Extra Trees
* Gradient Boosting
* AdaBoost
* XGBoost *(optional)*
* LightGBM *(best performing)*

---

## 🧪 Experimental Setup

* Train/Test split: **85% / 15%**
* Stratified sampling
* Evaluation metrics:

  * Accuracy
  * Precision
  * Recall
  * F1-score

---

## 📊 Results

### 🥇 Best Model

- **LightGBM**
- Best PCA: **80**
- Accuracy: **0.8879**
- F1-score: **0.8974**

### 📈 Key Findings

* PCA significantly reduces dimensionality with minimal information loss
* Bilateral smoothing improves model performance
* Classical ML models can compete with deep learning in this task

---

## 📉 Visualizations

The project includes:

* Class distribution plots
* Feature distributions (mean/std)
* Image sharpness analysis
* PCA explained variance curves
* Confusion matrices
* Model comparison charts
* Before vs after smoothing analysis

---

## 🧾 Outputs

* Best model performance summary
* Confusion matrices for each model
* PCA performance plots


---

## 🚀 How to Run

### 1. Clone the repository:

```bash
git clone https://github.com/AbdullahAl-Enezi/Lumbar-Disc-Herniation-Detection.git
cd Lumbar-Disc-Herniation-Detection
```

---

### 2. Install dependencies:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn opencv-python lightgbm
```

---

### 3. Run the project:

#### 🟢 Option 1: Using Jupyter Notebook (Recommended)

```bash
jupyter notebook
```

Then open:

```
Disc_Classifier.ipynb
```

---

#### 🟢 Option 2: Using Python script (if available)

```bash
python disc_classifier.py
```


---

## 📦 Requirements

* Python 3.8+
* numpy
* pandas
* opencv-python
* scikit-learn
* matplotlib
* seaborn
* xgboost *(optional)*
* lightgbm *(recommended)*

---

## 📌 Project Structure

```
├── data/
├── notebooks/
├── disc_classifier.py
├── best_pca_smoothing_comparison.csv
├── README.md
```

---

## 🧠 Key Contribution

This work demonstrates that:

> Carefully designed classical machine learning pipelines can achieve high performance on medical imaging tasks without requiring deep learning.

---

## 📬 Contact

Developed by: **Abdullah Al-Enezi**
Field: Artificial Intelligence

---

## ⭐ If you found this useful

Give the repo a star ⭐ and share it!
