# 🚦 Traffic Crash Severity Prediction using Machine Learning

## 📌 Project Overview

Road traffic accidents cause millions of injuries and fatalities worldwide every year. Predicting accident severity can help governments, traffic authorities, and emergency responders improve road safety and response planning.

This project builds a **Machine Learning-based system to predict crash severity** using environmental, roadway, and temporal factors. Multiple machine learning algorithms were tested and compared to determine the most accurate model.

The project was also documented in a **research paper analyzing machine learning approaches for traffic crash prediction.**

---

# 🎯 Objectives

* Predict whether a crash will result in **injury or no injury**
* Analyze the impact of **weather, road, and time conditions**
* Compare performance of multiple **machine learning algorithms**
* Discover accident patterns using **clustering techniques**
* Predict the **number of injuries using regression models**

---

# 📊 Dataset

The dataset contains historical traffic crash records including environmental, temporal, and roadway factors.

### Key Features

**Environmental**

* Weather Condition
* Lighting Condition

**Temporal**

* Crash Hour
* Day of Week

**Roadway**

* Road Surface Condition
* Trafficway Type

**Target Variables**

* Total Injuries
* Crash Damage Estimate

---

# ⚙️ Data Preprocessing

The following preprocessing steps were applied:

* Removed features with more than **50% missing values**
* Filled categorical missing values with **"Unknown"**
* Filled numerical missing values with **median values**
* Applied **Label Encoding** to convert categorical data into numerical form
* Standardized features using **Z-score normalization**

---

# 🔧 Feature Engineering

A binary classification variable was created.

```
Yclass = 1 if INJURIES_TOTAL > 0
Yclass = 0 if INJURIES_TOTAL = 0
```

This converts the problem into **injury vs no injury prediction**.

---

# 🤖 Machine Learning Models

## Regression Models

Used to predict the **exact number of injuries**

* Linear Regression
* Polynomial Regression

---

## Classification Models

Used to predict **injury occurrence**

* Decision Tree
* K-Nearest Neighbors (KNN)
* Naïve Bayes
* Support Vector Machine (SVM)
* Random Forest
* Gradient Boosting
* AdaBoost
* Neural Network (MLP)

---

## Unsupervised Learning

To identify hidden accident patterns:

* K-Means Clustering
* Hierarchical Clustering

Clusters revealed patterns such as:

* Late-night severe crashes
* Rush-hour accident frequency
* Weekend accident patterns

---

# 📈 Results

| Model             | Accuracy   |
| ----------------- | ---------- |
| Decision Tree     | ~80.7%     |
| KNN               | ~82.0%     |
| SVM               | ~83.7%     |
| **Random Forest** | **~84.5%** |

The **Random Forest classifier achieved the best performance**, demonstrating the effectiveness of ensemble learning methods for crash severity prediction.

---

# 📊 Model Evaluation

The models were evaluated using:

* Accuracy Score
* Confusion Matrix
* Bias-Variance Analysis

The confusion matrix showed strong prediction performance for **non-injury crashes while maintaining reasonable detection of injury cases.**

---

# 📉 Clustering Insights

Using **K-Means clustering (k=3)** the dataset was segmented into:

1. Late-night accidents (high severity)
2. Rush-hour accidents (high frequency)
3. Weekend accidents

These patterns can help traffic authorities design targeted safety measures.

---

# 🛠 Technologies Used

### Programming Language

Python

### Libraries

* Pandas
* NumPy
* Scikit-learn
* Matplotlib

### Machine Learning Techniques

* Classification
* Regression
* Clustering
* Principal Component Analysis (PCA)

---

# 📂 Project Structure

```
ml-project-traffic-crash-severity-prediction
│
├── data
│   └── traffic_crash_dataset.csv
│
├── notebooks
│   └── crash_severity_prediction.ipynb
│
├── research
│   └── traffic_crash_research_paper.pdf
│
├── README.md
```

---

# 🚀 Applications

* Traffic safety analysis
* Accident risk prediction
* Smart city transportation planning
* Emergency response optimization

---

# 🔮 Future Improvements

* Integrating **Deep Learning models such as LSTM**
* Handling class imbalance using **SMOTE**
* Using **real-time traffic and IoT sensor data**
* Building a **web dashboard for real-time accident monitoring**

---

# 👩‍💻 Author

**Tanvi**
B.Tech Computer Science & Engineering
Lovely Professional University

---

# ⭐ If you found this project useful

Consider giving this repository a **star ⭐**
