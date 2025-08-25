## Fetal Health ML Analysis
Machine learning-based fetal health classification system using cardiotocography data. Compares multiple algorithms (XGBoost, Random Forest, MLP, Logistic Regression) for predicting fetal health status with 95.9% accuracy.

## About the Project
This analysis uses CTG data to classify fetal health into three categories:
- **Normal**: Healthy condition
- **Suspect**: Requires monitoring
- **Pathological**: Critical condition requiring immediate intervention

The dataset contains 2,126 samples with 21 features measuring fetal heart rate patterns, accelerations, decelerations, and uterine contractions.

## Tools and Technologies Used
- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning algorithms and preprocessing
- **TensorFlow/Keras**: Neural network implementation
- **Matplotlib & Seaborn**: Data visualization
- **Plotly**: Interactive visualizations
- **Jupyter Notebook**: Development environment

## Key Results
The **XGBoost model** achieved the best performance with **95.9% accuracy**. Most importantly, it achieved 100% precision for pathological cases, meaning no high-risk patients were missed.

### Feature Importance
The most predictive features identified were:
- Mean short-term heart rate variability
- Prolonged decelerations
- Heart rate histogram statistics
- Abnormal short-term variability patterns

## How to Use
1. Clone the repository
2. Install required packages: `pip install pandas numpy scikit-learn xgboost tensorflow matplotlib seaborn plotly`
3. Open `Fetal_health.ipynb` in Jupyter Notebook
4. Run all cells to reproduce the analysis

## Models Compared
- XGBoost: 95.9% accuracy (Best)
- Random Forest: 94.5% accuracy
- Neural Network (MLP): 90.7% accuracy
- Logistic Regression: 88.8% accuracy

## Clinical Significance
The model shows promise for clinical decision support, with zero missed pathological cases in testing. However, clinical deployment would require additional validation and should complement, not replace, professional medical judgment.

## Disclaimer
This model is designed for research and educational purposes. It should not be used as the sole basis for medical decisions without proper clinical validation and oversight by qualified healthcare professionals.
