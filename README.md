# Mushroom Classification Via Random Forrest Gradient Boosting And Stacking Ensemble Methods

This project explores the use of ensemble learning techniques, including **Random Forest, Gradient Boosting, and Stacking**, to classify mushrooms as **edible or poisonous**. The dataset contains **61,069 instances** with **21 features**, making it well-suited for advanced classification tasks.

## Dataset & Files Overview

The **Secondary Mushroom Dataset** consists of:
- **primary_data.csv**
- **secondary_data.csv**
- **primary_data_meta.txt**
- **secondary_data_meta.txt**

Files:
- **Mushroom Classification Via Random Forrest Gradient Boosting And Stacking Ensemble Methods.docx**
- **Mushroom Classification Via Random Forrest Gradient Boosting And Stacking Ensemble Methods.ipynb**

These files contain bioinformatics data about mushrooms, with 21 nominal and metrical features, such as **cap diameter, gill color, stem root, habitat, and bruising properties**.

## Objective

The goal of this project is to implement **ensemble learning** to improve **classification accuracy** in distinguishing edible vs. poisonous mushrooms. The methods used include:
- **Random Forest (Bagging)** to reduce variance.
- **Gradient Boosting (Boosting)** to improve precision.
- **Stacking** to aggregate multiple model predictions for optimal performance.

## Ensemble Learning Methods

The project utilizes the following techniques:

1. **Random Forest (Bagging)**
   - Creates multiple decision trees and outputs the class mode.
   - Reduces variance and improves feature importance analysis.

2. **Gradient Boosting**
   - Builds weak learners sequentially to correct previous errors.
   - Enhances model precision by reducing bias.

3. **Stacking**
   - Uses Random Forest and Gradient Boosting as base models.
   - A final meta-estimator refines predictions for improved accuracy.

## Data Preprocessing

### Missing Values
- Found in **9 features**, filled with "uk" to maintain data integrity.

### Outliers
- Identified but **not removed**, as variability in biological data is expected.

### Feature Encoding
- **One-hot encoding** applied to categorical variables.
- **Binary encoding** applied to boolean features.

### Normalization
- **MinMaxScaler** was used to normalize numerical features (`cap-diameter`, `stem-height`, `stem-width`).

## Model Implementation

The dataset was split into **80% training and 20% testing**. The following models were implemented:

1. **Random Forest Classifier**
2. **Gradient Boosting Classifier**
3. **Stacking Classifier** (Combining Random Forest and Gradient Boosting)

## Usage
1. Clone the repository and navigate to the project directory:
git clone https://github.com/jovanthompsonmds/Mushroom-Classification-Via-Random-Forrest-Gradient-Boosting-And-Stacking-Ensemble-Methods.git

2. Run the Jupyter Notebook:
- Load and preprocess the data.
- Train the Random Forest, Gradient Boosting, and Stacking ensemble models.
- Evaluate classification performance using confusion matrices, accuracy scores, and ROC-AUC curves.

3. Analyze the model evaluation metrics and visualizations:
- Review feature distributions, outlier analysis, and normalized feature scaling.
- Compare ensemble method results to understand their impact on classification accuracy.
- Examine prediction probabilities for edible and poisonous mushrooms.

4. (Optional) Modify hyperparameters and test different ensemble learning configurations to observe performance variations.

### Model Evaluation

- **Confusion Matrix**: **100% classification accuracy**
- **Accuracy Score**: **100.00%**
- **ROC-AUC Curve**: **Perfect score of 1.00**
- **k-Fold Cross-Validation (k=10)**: **100.00% average score**

## Key Insights

- The model perfectly classified mushrooms as **edible or poisonous**.
- **No false positives or false negatives**, making it highly reliable.
- Stacking **enhanced prediction accuracy** by combining diverse models.
- **Model validation confirmed high generalizability** with **no overfitting**.

## Conclusion

This project demonstrates the power of **ensemble learning** in **binary classification tasks**. The combination of **bagging, boosting, and stacking** resulted in a **100% accurate model**, making it a **highly effective and practical solution** for mushroom classification.

## Contributing
Contributions are welcome! If you'd like to improve the project, add features, or provide feedback, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Author
Developed by Jovan Thompson as part of a data science portfolio project.
