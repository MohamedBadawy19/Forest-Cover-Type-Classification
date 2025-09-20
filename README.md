# 🌲 Forest Cover Type Classification

This project predicts the *type of forest cover* from cartographic variables using machine learning classification models.  
It uses the *UCI Covertype dataset*, which is one of the largest and most popular datasets for environmental classification.

---

## 📂 Dataset

- *Source*: [UCI Covertype Dataset](https://archive.ics.uci.edu/ml/datasets/covertype)  
- *Size: **581,012 rows × 54 features*  
- *Target Variable*: Cover_Type (7 forest cover classes)  

### Features:
- *Elevation, Aspect, Slope*  
- *Hydrology distances (horizontal/vertical)*  
- *Distances to roadways & fire points*  
- *Hillshade indices (9am, Noon, 3pm)*  
- *40 Soil Types (binary)*  
- *4 Wilderness Areas (binary)*  

✔ No missing values  
✔ No duplicates  

---

## 🛠 Tools & Libraries

Implemented in *Python 3* using:

- *pandas, numpy* → Data processing  
- *matplotlib, seaborn* → Data visualization  
- *scikit-learn* → Preprocessing, train-test split, Random Forest  
- *imbalanced-learn (SMOTE)* → Handling class imbalance  
- *XGBoost* → Gradient boosting model for classification  

---

## 🔎 Project Workflow

1. *Data Preprocessing*
   - Converted categorical soil/wilderness columns into boolean type.
   - Standardized continuous features with *StandardScaler*.
   - Addressed class imbalance using *SMOTE*.

2. *Dimensionality Reduction*
   - Applied *PCA* for feature exploration and visualization.

3. *Model Training*
   - *Random Forest Classifier*  
   - *XGBoost Classifier*

4. *Model Evaluation*
   - Confusion Matrix visualization  
   - Classification Report (Precision, Recall, F1-score)  
   - Accuracy comparison  

---

## 📊 Results & Accuracy

- *Random Forest Classifier*  
  - Accuracy: *~93%*  
  - Strong performance with balanced precision/recall.  

- *XGBoost Classifier*  
  - Accuracy: *~95%*  
  - Outperformed Random Forest, particularly in distinguishing minority cover types.  

✅ *Best Model: XGBoost (95% Accuracy)*  

---

## ▶ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/forest-cover-classification.git
   cd forest-cover-classification

2. Install dependencies:

pip install -r requirements.txt


3. Run the Jupyter Notebook:

jupyter notebook forest-cover-type-classification.ipynb




---

📌 Future Work

Try deep learning models (Neural Networks, CNNs) for improved performance.

Experiment with feature engineering for soil and elevation interactions.

Deploy the best model as an API/Streamlit app for environmental monitoring.

