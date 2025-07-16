# README for Credit Card Fraud Detection Model

## Project Overview
This project implements machine learning models to detect fraudulent credit card transactions using a highly imbalanced dataset. We compare Random Forest and Logistic Regression approaches to identify fraudulent activity with high precision while minimizing false positives.

## Objective
- Develop binary classification models to distinguish fraudulent (positive class) from legitimate (negative class) transactions
- Handle extreme class imbalance (only 0.17% fraud cases)
- Optimize models to maximize fraud detection while minimizing false positives
- Provide interpretable results for business decision-making

## Dataset
The dataset contains credit card transactions with:
- Time-normalized numerical features (V1-V28) from PCA transformation
- Transaction amount (normalized)
- Class label (0 = legitimate, 1 = fraudulent)

## Key Features
✅ **Binary Classification**: Distinguishes fraudulent vs legitimate transactions  
✅ **Imbalance Handling**: Special techniques for 0.17% fraud case distribution  
✅ **Model Comparison**: Random Forest vs Logistic Regression performance  
✅ **Comprehensive Metrics**: Precision, recall, F1-score, and ROC analysis  
✅ **Feature Importance**: Identifies most predictive transaction characteristics  
✅ **Visual Analytics**: Confusion matrices and ROC curves for model evaluation  

## Methodology
1. **Data Preprocessing**:
   - Feature scaling and normalization
   - Stratified sampling for model evaluation

2. **Imbalance Handling**:
   - Class weighting
   - Strategic metric selection (prioritizing precision and recall)

3. **Model Development**:
   - Logistic Regression (baseline interpretable model)
   - Random Forest (ensemble method for complex patterns)
   - Hyperparameter tuning with GridSearchCV

4. **Evaluation**:
   - Precision-Recall tradeoff analysis
   - ROC curve comparison
   - Feature importance interpretation

## Technical Implementation
- **Python 3.x** with scikit-learn
- **Pandas/NumPy** for data manipulation
- **Matplotlib/Seaborn** for visualization
- **GridSearchCV** for hyperparameter optimization
- **Imbalanced-learn** for handling class imbalance (optional)

## Business Value
💳 **Financial Protection**: Reduces losses from fraudulent transactions  
👥 **Customer Experience**: Minimizes false positives to avoid blocking legitimate transactions  
🛡️ **Real-time Framework**: Provides foundation for production fraud detection systems  
📈 **Risk Management**: Helps financial institutions optimize fraud prevention strategies  

## Repository Structure
```
├── data/                   # Dataset files
├── notebooks/              # Jupyter notebooks with full analysis
│   ├── EDA.ipynb          # Exploratory data analysis
│   ├── Modeling.ipynb     # Model development and evaluation
├── src/                    # Python modules (if applicable)
├── outputs/                # Saved models and visualizations
│   ├── models/            # Serialized model files
│   ├── figures/           # Evaluation plots
└── README.md
```

## Key Results
- Achieved high precision (>90%) to minimize false positives
- Maintained strong recall to catch majority of fraudulent cases
- Identified most predictive transaction features
- Provided clear performance comparison between models

## How to Use
1. Clone repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run Jupyter notebooks in sequence:
   - `EDA.ipynb` for data exploration
   - `Modeling.ipynb` for model development

## Dependencies
- Python 3.7+
- scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter

## Future Improvements
- Experiment with additional models (XGBoost, Neural Networks)
- Implement anomaly detection approaches
- Develop API for real-time predictions
- Create synthetic fraud cases for better training

## Author
[Harshraj Chavda] 
[harshchavda439@gmail.com]  
[@HarshSanatani]

## License
This project is available under the MIT License.
