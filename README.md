### README: Patient Risk Prediction System

#### **Overview**
The Patient Risk Prediction System leverages machine learning models to predict risks for conditions such as diabetes, hypertension, and strokes. The system uses structured datasets to train and evaluate various classification models, ensuring high accuracy and reliable predictions.

---

### **Datasets**
- **Diabetes Dataset**:
  - Predicts whether a patient is at risk of diabetes.
  - Target Variable: `Diabetes`
- **Hypertension Dataset**:
  - Predicts the likelihood of a patient having hypertension.
  - Target Variable: `target`
- **Strokes Dataset**:
  - Predicts the probability of a stroke occurrence.
  - Target Variable: `stroke`

---

### **Models Evaluated**
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. K-Nearest Neighbors (KNN)
5. Multinomial Naive Bayes (for normalized datasets)

---

### **Results Summary**

#### **Diabetes Dataset**
| Model                  | Training Accuracy | Testing Accuracy | F1 Score (Test) |
|------------------------|-------------------|------------------|-----------------|
| Logistic Regression    | 74.78%           | 74.61%          | 74.60%          |
| Decision Tree          | 97.17%           | 65.86%          | 65.85%          |
| Random Forest          | 97.17%           | 72.57%          | 72.53%          |
| KNN                    | 82.89%           | 69.48%          | 69.46%          |

#### **Hypertension Dataset**
| Model                  | Training Accuracy | Testing Accuracy | F1 Score (Test) |
|------------------------|-------------------|------------------|-----------------|
| Logistic Regression    | 85.87%           | 85.74%          | 85.62%          |
| Decision Tree          | 100%             | 100%            | 100%            |
| Random Forest          | 100%             | 100%            | 100%            |
| KNN                    | 100%             | 100%            | 100%            |
| Multinomial Naive Bayes| 78.61%           | 78.55%          | 78.30%          |

#### **Strokes Dataset**
| Model                  | Training Accuracy | Testing Accuracy | F1 Score (Test) |
|------------------------|-------------------|------------------|-----------------|
| Logistic Regression    | 68.39%           | 68.25%          | 68.10%          |
| Decision Tree          | 100%             | 99.94%          | 99.94%          |
| Random Forest          | 100%             | 99.66%          | 99.66%          |
| KNN                    | 94.42%           | 89.64%          | 89.57%          |
| Multinomial Naive Bayes| 66.31%           | 66.94%          | 66.03%          |

---

### **Key Observations**
1. **Decision Tree and Random Forest**:
   - Achieved perfect accuracy on the Hypertension and Stroke datasets, likely due to overfitting on small data variations.
   - Performed less consistently on the Diabetes dataset.

2. **Logistic Regression**:
   - Provided stable and interpretable results across all datasets.
   - Best choice for cases requiring linear separation and simplicity.

3. **KNN**:
   - Showed strong performance, especially for Stroke predictions with accuracy close to 90%.

4. **Multinomial Naive Bayes**:
   - Performed well on normalized data but struggled with complex, high-dimensional datasets.

---

### **System Features**
- **Normalization**:
  - Applied `MinMaxScaler` to scale features between 0 and 1, ensuring compatibility with all models.
- **Evaluation Metrics**:
  - Accuracy, F1 Score, Precision, and Recall are calculated for both training and testing datasets.
- **Heatmap Visualization**:
  - Correlation matrices provide insights into feature relationships and predictive power.

---

### **How to Use**
1. **Pre-requisites**:
   - Python 3.7+
   - Libraries: `pandas`, `numpy`, `sklearn`, `seaborn`, `matplotlib`
2. **Run the Code**:
   - Update the dataset paths in the `datasets` dictionary.
   - Execute the script to train models and visualize results.
3. **View Outputs**:
   - Model metrics are printed for each dataset.
   - Correlation matrices and insights are displayed as visualizations.

---

### **Conclusion**
- This system demonstrates the ability to predict patient risk effectively using machine learning models.
- Decision Tree and Random Forest are highly accurate but prone to overfitting.
- Logistic Regression is reliable for datasets with linear relationships.
- Feature normalization is essential for models like Multinomial Naive Bayes.

For further enhancements, consider hyperparameter tuning and additional data preprocessing techniques. Let me know if you need help with extensions or deployment strategies!
