**Introduction:** 

In this assignment, the primary objective is to build a binary classifier that predicts the "has_disease" column using the dataset named "synthetic_data_training.csv." The central focus of this task is to maximize the F1 score, which plays a pivotal role in assessing the performance of binary classification models.

The assignment entails a comprehensive data preprocessing process, encompassing various critical steps. These include the careful handling of missing data through the application of appropriate imputation techniques, the identification and treatment of outliers, the standardization of numeric features to ensure consistency, and the effective encoding of categorical features for model training. An essential consideration throughout this process is the strict adherence to applying all data preprocessing steps, such as imputation and feature scaling, exclusively to the training dataset to prevent any potential data leakage.

Upon the completion of model development, the best-performing classifier will be applied to the "synthetic_data_test.csv" dataset, and the resulting predictions will be saved in a file named "answers.csv."

**Methodology**

I initiated the analysis by importing the "synthetic_data_training.csv" dataset. To gain a comprehensive understanding of the data, I generated histograms and scatter plots to visualize the relationships between various data points.

Subsequently, I conducted a thorough examination for missing values within the dataset. For numeric features, I implemented imputation using the mean, while for categorical features, I utilized the mode as the imputation strategy.

To ensure the effectiveness of the data preprocessing steps, I selected a representative row from the dataset and verified that the missing values had been accurately filled. Following this, I proceeded to define the feature columns (X) and the target variable (Y). The dataset was then split into training and validation sets, and preprocessing steps were applied to both numeric and categorical features.

For model construction, I created a logistic regression classifier and designed a pipeline that encompassed both preprocessing and classification stages. Subsequently, I trained the model using the training data and assessed its performance on the validation set. Remarkably, the model achieved an F1 score of ***84.37%*** on the training data.

To gain deeper insights into the model's performance, I constructed a confusion matrix, which provided valuable metrics such as True Negatives (TN), False Positives (FP), False Negatives (FN), and True Positives (TP). Additionally, the model achieved an impressive average precision score of 0.94 in the precision-recall curve analysis. This score underscores the model's accuracy and effectiveness in identifying positive cases, with a balanced approach that minimizes false positives while capturing a high proportion of true positives.

Finally, in the last step, I loaded the testing data, applied the trained model to make predictions, and saved the predictions to an "answers.csv" file for submission.

**Results:**
I was able to have the F1 score of 84.37%


**Acknowledgements:** I recognize that I actively pursued additional resources, such as external platforms like Stack Overflow and ChatGPT, to expand my knowledge and understanding while working on this assignment.

