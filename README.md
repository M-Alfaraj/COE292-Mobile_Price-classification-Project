# COE292-Mobile_Price-classification-Project

# About the Project

This project applies machine learning techniques to classify mobile phones into four price ranges based on their technical specifications. Using a dataset of 2000 samples and 20 numerical features from Kaggle, the goal is to evaluate and compare different classification models on a structured real-world problem.

The project implements a full machine learning pipeline including data preprocessing, feature scaling, exploratory data analysis, model training, and evaluation. Three algorithms are studied: K-Nearest Neighbors (KNN), Support Vector Machine (SVM), and Multilayer Perceptron (MLP). Each model is tested using stratified 5-fold cross-validation and evaluated using multiple performance metrics.

## Team Members
1. MOHAMMAD ABUALSAUD
2. MOHAMMED ALFARAJ
3. YOUSEF ALMAZROEI
Team ID: S4_2

## Dataset
- Source: Kaggle Mobile Price Classification
- Samples: 2000
- Features: 20
- Classes: 4 (price range 0–3)
- Balanced dataset (500 samples per class)
- No missing values

## Methodology
### Data Preprocessing
- No missing values or categorical encoding required
- Feature scaling using StandardScaler
- Stratified 5-fold cross-validation for evaluation

### Data Visualization
- RAM vs Battery Power
- Pixel Width vs Pixel Height
- Internal Memory vs RAM
- Weight vs Battery Power

These visualizations help analyze feature separability and class overlap.

## Machine Learning Models
### K-Nearest Neighbors (KNN)
- Euclidean distance metric
- Best K selected through experimentation
- Performance affected by overlapping feature distributions

### Support Vector Machine (SVM)
- Kernels tested: Linear, RBF, Polynomial
- Best model: Linear kernel (C = 1)
- Strong performance due to near-linear separability

### Multilayer Perceptron (MLP)
- Fully connected neural network
- Best architecture: (64, 32)
- Captures complex non-linear relationships


## Evaluation Metrics

All models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Sensitivity & Specificity
- Confusion Matrix
- 5-Fold Stratified Cross-Validation


## Results Summary
| Model |	Accuracy | Precision |	Recall | F1-score |
| KNN |	0.5775 |	0.5874 |	0.5775 |	0.5798 |
| SVM |	0.9615 |	0.9623 |	0.9615 |	0.9614 |
| MLP |	0.9230 |	0.9245 |	0.9230 |	0.9231 |

## Conclusion
SVM achieved the best performance, indicating strong class separability in the dataset. MLP performed well by capturing non-linear patterns, while KNN showed lower performance due to sensitivity to overlapping feature distributions.

🎥 Video Demonstration
Link: [Insert Here]
