# Loan Approval Prediction Model

## Objective
This project aims to develop a prediction model for automating loan approval decisions at a large regional bank. The focus is on interpreting and critically evaluating various classification performance measures and understanding their implications for different business contexts.

## Repository Structure
The repository is organized into three main parts, each corresponding to a separate Jupyter Notebook:

- **Part 1 - k-Nearest Neighbors (kNN) Model**
- **Part 2 - Logistic Regression Model**
- **Part 3 - Model Evaluation and Business Implications**

Each notebook follows the same high-level outline:

### High-Level Outline

#### Brief Background Section
- **Problem Statement**: What is the problem? Why is it important? Who are the key stakeholders?
- **Importance**: Discuss the significance of accurate loan approval predictions.
- **Stakeholders**: Identify key stakeholders (e.g., bank management, loan officers, customers).

#### Data Section
- **Dataset**: Description of the dataset (loan_approval.csv).
- **Preprocessing**: Note that the data has already been cleaned with no missing values and categorical encoding done.
- **Train/Test Split**: Perform a train/test split.
- **Normalization**: Optionally normalize numerical variables if there are significant scaling issues.

#### Classification Modeling

- **k-Nearest Neighbors (kNN)**
  - **Hyperparameter Tuning**: Find the best "k" value by looping through a list of odd numbers and choosing the one that produces the most accurate model.
  - **Final Model Training**: Train the final kNN model using the selected "k".
  - **Performance Measures**: Create a table of performance measures (TN, TP, FN, FP, Precision, Recall, F1, Accuracy) over a range of probability thresholds.

- **Logistic Regression**
  - **Model Training**: Train a Logistic Regression model.
  - **Performance Measures**: Create a table of performance measures as described above for the Logistic Regression model.

- **Model Comparison and Selection**
  - **Choose Winning Model**: Decide which model (kNN or Logistic Regression) to move forward with based on performance measures.
  - **Justification**: Justify the choice of the winning model.

#### Careful Evaluation of Winning Model Performance Measures
- **Threshold Evaluation**: Evaluate performance measures at different probability thresholds (e.g., 0 to 0.4).
- **Business Implications**: Discuss the potential business ramifications of False Positives and False Negatives at each threshold.
- **Cost Analysis**: Speculate on the costs of prediction mistakes and which are more costly.
- **Recommended Threshold**: Recommend a probability threshold based on the evaluation and analysis.

## Dataset
The dataset used in this project is `loan_approval.csv`, with the target variable being `approved`. The dataset includes various features related to loan applicants. Note: Some features (e.g., ethnicity, age) may pose ethical concerns if used in practice. Consider these issues when developing and interpreting your models.

## Learning Outcomes
By the end of this project, readers will:
- Understand the process of building and evaluating classification models.
- Gain experience in hyperparameter tuning for kNN and Logistic Regression models.
- Learn to interpret various performance measures and their business implications.
- Develop a critical approach to selecting and justifying the best model for a given problem.
- Understand the ethical considerations of using sensitive features in predictive modeling.

## Getting Started
1. **Clone the Repository**: `git clone <repository_url>`
2. **Install Dependencies**: Ensure you have the necessary Python libraries installed (e.g., pandas, scikit-learn, matplotlib, seaborn).
3. **Open Jupyter Notebooks**: Navigate to each part of the project and follow the steps outlined in the Jupyter Notebooks.
