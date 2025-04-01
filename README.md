# E-commerce Shopping Analysis and Purchase Prediction

This project analyzes online shopping behavior and predicts purchase intentions using machine learning techniques. The goal is to determine whether a visitor will complete a purchase during their browsing session by analyzing various behavioral metrics.

## Project Overview

The project uses the Online Shoppers Purchasing Intention Dataset from the UCI Machine Learning Repository, containing 12,330 sessions collected over one year. It implements a machine learning pipeline to predict purchase likelihood based on session characteristics.

### Key Features
- Comprehensive exploratory data analysis (EDA)
- Handling of imbalanced data using SMOTE
- Implementation of multiple machine learning models
- Detailed performance evaluation and comparison

## Dataset Description

The dataset includes various features capturing visitor behavior:

### Numerical Features:
- Page visit counts (Administrative, Informational, Product Related)
- Time duration metrics
- Bounce rates and exit rates
- Page values
- Special day indicator
- Operating system, browser, and region information

### Categorical Features:
- Month of the year
- Visitor type (New, Returning, Other)
- Weekend indicator
- Revenue (target variable)

## Implementation Details

### Data Preprocessing
- Robust scaling for numerical features
- One-hot encoding for categorical variables
- SMOTE for handling class imbalance

### Models Implemented
1. Logistic Regression
   - Baseline model
   - ROC AUC Score: 0.898
   - Overall accuracy: 85%

2. Random Forest Classifier
   - Advanced model
   - ROC AUC Score: 0.917
   - Overall accuracy: 89%

## Key Findings

- Significant class imbalance (15.5% purchase vs 84.5% no purchase)
- Strong correlation between page values and purchase likelihood
- Seasonal patterns in shopping behavior
- Random Forest outperforms Logistic Regression in overall metrics

## Project Structure

```
.
├── app.ipynb          # Main notebook with analysis and modeling
├── README.md         # Project documentation
└── .gitignore        # Git ignore file
```

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- imbalanced-learn

## Installation

`pip install` is included in the app.ipynb file.

## Usage

1. Clone the repository
2. Run the Jupyter notebook `app.ipynb`

## Results

The Random Forest model achieved the best performance with:
- 89% overall accuracy
- 66% precision for purchase prediction
- 65% recall for purchase prediction
- 0.917 ROC AUC score

## Business Applications

This model can be used to:
- Trigger personalized offers for likely purchasers
- Optimize marketing resource allocation
- Improve customer experience through targeted interventions
- Increase conversion rates and revenue

## Future Improvements

- Feature engineering for temporal patterns
- Implementation of deep learning models
- Real-time prediction capabilities
- A/B testing framework for interventions

## License

This project is open source and available under the MIT License.

## Contact

For questions or feedback, please open an issue in the repository. 