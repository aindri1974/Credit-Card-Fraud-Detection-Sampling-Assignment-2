# Credit-Card-Fraud-Detection-Sampling-Assignment-2

### Analysis of Results:

From the `accuracy_table`, we can observe the performance of each model with different sampling techniques. To identify the best combination, we look for the highest accuracy scores.

*   **M1 (Logistic Regression):** Shows consistent accuracy around 91-92% across most sampling methods, with slightly higher performance for Random Over-sampling, SMOTE, and TomekLinks. The convergence warning suggests that `max_iter` might need to be increased or the data scaled for this model.
*   **M2 (Decision Tree Classifier):** Achieves very high accuracy, with 100% using Random Under-sampling, and consistently above 98% for others. This indicates it performs exceptionally well, especially with `RandomUnderSampler` in this specific setup.
*   **M3 (Random Forest Classifier):** Demonstrates excellent performance, achieving 100% accuracy with NearMiss, and nearly 100% (99.78%) with all other sampling methods. This is the most robust model in this comparison.
*   **M4 (K-Neighbors Classifier):** Performs well, with accuracy ranging from 97.60% to 98.47%. Random Over-sampling, SMOTE, and TomekLinks yield slightly better results for this model.
*   **M5 (Gaussian Naive Bayes):** Shows the lowest accuracy among the models, ranging from 65.94% to 78.17%. Random Over-sampling, SMOTE, and TomekLinks provide a notable improvement compared to Random Under-sampling and NearMiss.

**Overall Best Performance:**

*   **Random Forest Classifier (M3)** achieved 100% accuracy with **NearMiss (Sampling4)**.
*   **Decision Tree Classifier (M2)** also achieved 100% accuracy with **Random Under-sampling (Sampling1)**.

These results suggest that for this specific dataset and experimental setup, ensemble methods like Random Forest and tree-based models like Decision Trees, when combined with appropriate sampling techniques, yield the highest accuracy. The choice of sampling technique significantly impacts the performance, particularly for simpler models like Gaussian Naive Bayes and Logistic Regression.
