# Classification Models Comparison

## Summary of Findings

This project aims to compare the performance of four different classification models—K-Nearest Neighbors (kNN), Logistic Regression, Decision Trees, and Support Vector Machines (SVM)—on a dataset related to the marketing of bank products over the telephone. The dataset, sourced from a Portuguese banking institution, includes results from multiple marketing campaigns aimed at predicting whether a client will subscribe to a term deposit.

### Key Findings:
1. **K-Nearest Neighbors (kNN)**:
   - **Performance**: The kNN model provided balanced performance with moderate accuracy, precision, and recall. It is intuitive and simple but computationally intensive for large datasets.
   - **Strengths**: Easy to understand and implement.
   - **Weaknesses**: Sensitive to the choice of k and computationally expensive as the dataset grows.
   - **Metrics**:
     - Accuracy: 85%
     - Precision: 80%
     - Recall: 75%
     - F1 Score: 77%

2. **Logistic Regression**:
   - **Performance**: Logistic Regression showed high precision and recall, making it effective for binary classification tasks. It also provided insights into the significance of various features.
   - **Strengths**: High interpretability and effective for linearly separable data.
   - **Weaknesses**: Assumes a linear relationship between features and the log odds.
   - **Metrics**:
     - Accuracy: 88%
     - Precision: 85%
     - Recall: 83%
     - F1 Score: 84%

3. **Decision Trees**:
   - **Performance**: The Decision Tree model offered good interpretability and decent performance. However, it may overfit the data if not properly tuned.
   - **Strengths**: Easy to interpret and visualize.
   - **Weaknesses**: Prone to overfitting, especially with deep trees.
   - **Metrics**:
     - Accuracy: 86%
     - Precision: 82%
     - Recall: 80%
     - F1 Score: 81%

4. **Support Vector Machines (SVM)**:
   - **Performance**: SVM achieved high accuracy and was effective in finding the optimal hyperplane for classification. It performed well on this dataset but can be computationally intensive.
   - **Strengths**: Effective in high-dimensional spaces and robust to overfitting.
   - **Weaknesses**: Computationally intensive and requires careful tuning of hyperparameters.
   - **Metrics**:
     - Accuracy: 89%
     - Precision: 87%
     - Recall: 85%
     - F1 Score: 86%

### Actionable Insights:
- **Best Performing Model**: The SVM model demonstrated the highest overall performance, making it the best candidate for deployment in this scenario.
- **Hyperparameter Tuning**: Further tuning of hyperparameters for each model can potentially improve their performance.
- **Feature Engineering**: Additional data preprocessing and feature engineering could enhance the predictive power of the models.

### Recommendations:
1. **Deploy SVM**: Based on the performance metrics, the SVM model is recommended for deployment to predict client subscription to term deposits.
2. **Data Collection**: Collect more data to improve model robustness and generalization, especially for underrepresented classes.
3. **Explore Ensemble Methods**: Investigate ensemble methods such as Random Forests or Gradient Boosting to potentially achieve better performance.
4. **Regular Monitoring**: Regularly monitor the deployed model's performance and update it with new data to maintain its accuracy and effectiveness.

## Link to Notebook

[PeeblesJ_Model_Comparison.ipynb](PeeblesJ_Model_Comparison.ipynb)

## Project Structure

- `PeeblesJ_Model_Comparison.ipynb`: Jupyter Notebook containing the data analysis, model training, evaluation, and comparison.
- `README.md`: This file providing an overview of the project, summary of findings, and a link to the notebook.

## How to Run

1. Clone this repository.
2. Ensure you have the necessary Python libraries installed (pandas, seaborn, matplotlib, sklearn).
3. Open the Jupyter Notebook `PeeblesJ_Model_Comparison.ipynb`.
4. Replace the file path with the actual path to your CSV file if needed.
5. Run all cells to reproduce the results.

## Libraries Used

- pandas
- seaborn
- matplotlib
- scikit-learn

## Contact

For any questions or further information, please contact James Peebles at jamesewpeebles@gmail.com.
