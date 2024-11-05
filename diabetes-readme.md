# Diabetes Prediction using Logistic Regression

This project implements a machine learning model to predict diabetes using logistic regression. The model analyzes various health metrics to determine whether a patient is likely to have diabetes.

## Overview

The project uses a dataset containing various health parameters to predict diabetes. The model achieves approximately 76% accuracy in predictions, with particular attention paid to recall metrics given the healthcare domain context.

## Dataset Features

The dataset includes the following parameters:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI (Body Mass Index)
- Diabetes Pedigree Function
- Age
- Outcome (Target Variable)

## Technical Implementation

### Data Preprocessing
- Handled missing values and zero values using median/mean imputation
- Removed outliers using IQR approach
- Standardized features using StandardScaler
- Addressed class imbalance using SMOTE

### Model Development
- Used Logistic Regression for classification
- Split data into 80% training and 20% testing sets
- Implemented SMOTE for handling imbalanced classes

## Model Performance

- Accuracy: 76.47%
- Detailed metrics:
  - Non-Diabetic:
    - Precision: 0.85
    - Recall: 0.78
    - F1-score: 0.81
  - Diabetic:
    - Precision: 0.64
    - Recall: 0.73
    - F1-score: 0.68

## Dependencies

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- imbalanced-learn

## Installation

```bash
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn
```

## Usage

1. Clone the repository:
```bash
git clone [repository-url]
```

2. Navigate to the project directory:
```bash
cd diabetes-prediction
```

3. Run the Jupyter notebook:
```bash
jupyter notebook Project_2_Predictive_Analysis_in_diabetes.ipynb
```

## Project Structure

```
├── Project_2_Predictive_Analysis_in_diabetes.ipynb
├── diabetes.csv
├── classification_model.pkl
├── README.md
└── images/
    ├── Correlation-coefficient.jpg
    └── Boxplot.jpg
```

## Key Findings

- The model shows good performance in identifying non-diabetic cases (85% precision)
- Recall for diabetic cases (73%) indicates reasonable effectiveness in identifying positive cases
- Feature correlation analysis revealed important relationships between health metrics

## Future Improvements

1. Experiment with different machine learning algorithms
2. Collect more data to improve model performance
3. Implement cross-validation for more robust evaluation
4. Consider feature engineering to create more predictive variables

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Contact

Your Name - [your-email@example.com]

Project Link: [https://github.com/yourusername/diabetes-prediction]
