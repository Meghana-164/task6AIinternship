#  K-Nearest Neighbors (KNN) Classification on Iris Dataset

## Objective
To understand and implement the K-Nearest Neighbors (KNN) algorithm for classification using the Iris dataset. This task focuses on evaluating the effect of different `K` values, visualizing decision boundaries, and interpreting model performance.

---

##  Dataset Overview

- **Dataset**: Iris Dataset (150 entries, 4 features + target)
- **Features Used**:
  - SepalLengthCm
  - SepalWidthCm
  - PetalLengthCm
  - PetalWidthCm
- **Target**: Species (Iris-setosa, Iris-versicolor, Iris-virginica)

---

## Tools & Libraries

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## ⚙️ Steps Followed

1. **Data Preprocessing**
   - Dropped unnecessary columns (e.g., `Id`)
   - Normalized features using `StandardScaler`

2. **Model Implementation**
   - Used `KNeighborsClassifier` from `sklearn`
   - Trained model using different values of `K` from 1 to 10

3. **Model Evaluation**
   - Accuracy score
   - Confusion matrix
   - Classification report

4. **Visualization**
   - Decision boundary plotted using two most discriminative features:
     - PetalLengthCm (scaled)
     - PetalWidthCm (scaled)

---

##  Accuracy for Different K Values

| K | Accuracy |
|---|----------|
| 1 | 0.97     |
| 2 | 1.00     |
| 3 | 1.00     |
| 4 | 1.00     |
| 5 | 1.00     |
| 6 | 1.00     |
| 7 | 1.00     |
| 8 | 1.00     |
| 9 | 1.00     |
|10 | 1.00     |

---

##  Best K Value Chosen
- **K = 3** was selected for further evaluation and visualization due to high performance and stability.

---

## 📈 Evaluation Metrics (for K=3)
### Classification Report
| Class            | Precision | Recall | F1-score | Support |
|------------------|-----------|--------|----------|---------|
| Iris-setosa      | 1.00      | 1.00   | 1.00     | 10      |
| Iris-versicolor  | 1.00      | 1.00   | 1.00     | 9       |
| Iris-virginica   | 1.00      | 1.00   | 1.00     | 11      |

- **Overall Accuracy**: 100%

- ---

##  Key Takeaways

- KNN is a simple and effective instance-based learning algorithm.
- Normalization is crucial for distance-based models.
- Lower values of K can be sensitive to noise; higher values may over-smooth decision boundaries.
- The Iris dataset is well-suited for KNN due to its clear cluster structure.

---
