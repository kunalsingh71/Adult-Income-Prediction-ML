# 📈 Adult Income Prediction (Neural Network Project)

### 📌 Project Overview
This project was developed as the final assignment during my **AICTE & Edunet Foundation Internship** (November – December 2025). The goal is to predict whether an individual's annual income exceeds **$50,000** based on census data, using various Machine Learning classification algorithms.

---

### 🛠️ Tech Stack & Tools
* **Language:** Python 3.x
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** * `Pandas`: Data manipulation and analysis.
    * `NumPy`: Numerical computations.
    * `Scikit-Learn`: Machine Learning modeling (Preprocessing, KNN, MLP).
    * `Matplotlib` & `Seaborn`: Data visualization and outlier detection.

---

### 📊 The Machine Learning Pipeline

#### 1. Data Acquisition
* **Dataset:** Adult Census Income (UCI Machine Learning Repository).
* **Size:** 48,842 entries with 15 features (Age, Workclass, Education, Occupation, etc.).

#### 2. Data Preprocessing
* **Cleaning:** Handled missing values represented by `?` by replacing them with "Others."
* **Outlier Removal:** Used **Box Plots** to identify and remove unrealistic data points in age (e.g., Age < 17 or > 75).
* **Feature Selection:** Dropped redundant columns like `education` in favor of `educational-num` to reduce dimensionality.

#### 3. Feature Engineering
* **Encoding:** Applied **Label Encoding** to convert categorical text data into numerical format.
* **Scaling:** Utilized **MinMaxScaler** to normalize numerical features between 0 and 1, ensuring the Neural Network (MLP) converges effectively.

#### 4. Model Training & Evaluation
I implemented and compared three classification models to find the best performer:
* **K-Nearest Neighbors (KNN):** ~81.6% accuracy.
* **Logistic Regression:** ~81.9% accuracy.
* **Multi-Layer Perceptron (MLP):** **~82% accuracy** (Winner).

---

### 🏆 Key Results
The **MLP Classifier** outperformed traditional models, demonstrating the power of Neural Networks in capturing non-linear relationships within demographic data.

| Model | Accuracy (%) |
| :--- | :--- |
| KNN | 81.6% |
| Logistic Regression | 81.9% |
| **MLP (Neural Network)** | **82.1%** |

---

### 📁 Repository Structure
```text
├── Major assignment.ipynb   # Full Python implementation
├── adult.csv                # Project Dataset
├── README.md                # Project Documentation
└── images/                  # Visualizations (Boxplots, Confusion Matrix)
