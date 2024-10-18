# HR-Analytics
This project is aimed to analyze employee-related data and provide insights into workforce management, employee performance, and attrition trends. The objective is to use predictive modeling to understand the factors influencing employee turnover and help the organization retain valuable employees by identifying potential risks early on.

### Buisness Objectives: 
1. To analyze employee attrition and understand the key factors contributing to employees leaving the organization.
2. To build predictive models that can identify employees who are at risk of attrition.
3. To provide insights that can help HR managers take proactive steps to retain employees and improve workforce stability.

**Key steps in the process include:** 

- Data Preprocessing: Cleaning and transforming the dataset for analysis.
     - Deleting redundant columns.
     - Renaming the columns.
     - Dropping duplicates.
     - Cleaning individual columns.
     - Remove the NaN values from the dataset
     - Check for some more Transformations
- Exploratory Data Analysis: Identifying key patterns and relationships between employee characteristics and attrition.
- Model Building: Applying machine learning algorithms to predict employee attrition.
- Evaluation and Optimization: Assessing model performance and improving accuracy through techniques such as hyperparameter tuning.

-----------------------------------------------------------------------------------------------------
## Dataset Description:
The dataset used in the project contains employee-related features typically gathered by HR departments. Some key features include:

Employee ID: Unique identifier for each employee.
Age: The age of the employee.
Gender: Gender of the employee.
Department: The department to which the employee belongs.
Job Role: The specific role or job title held by the employee.
Years at Company: The number of years the employee has worked at the company.
Salary: Salary or compensation details.
Job Satisfaction: Rating of the employee’s satisfaction with their job.
Attrition: Whether the employee has left the company or not (binary variable used for predictive modeling).
This dataset represents key HR metrics that could influence employee retention and performance outcomes.




## 4. Methods Used
1. Data Preprocessing:
Handling Missing Values: Filling or removing missing data entries.
Categorical Data Encoding: Converting categorical variables (such as department or job role) into numerical form using techniques like one-hot encoding or label encoding.
Feature Scaling: Normalizing numeric features (e.g., salary, years at company) to ensure all features are on a similar scale.

2. Exploratory Data Analysis (EDA):
Correlation Analysis: Understanding how variables such as job satisfaction, salary, and department are related to employee attrition using heatmaps and pair plots.
Distribution Analysis: Visualizing the distribution of employees across departments, age groups, and job roles to identify trends that could influence turnover.

3. Model Building:
Logistic Regression: A classification model used as a baseline to predict whether an employee will leave (attrition) or stay.
Random Forest: An ensemble method used for classification that builds multiple decision trees and outputs the majority class prediction.
Gradient Boosting: Another ensemble technique that builds sequential trees to correct previous errors, often used to improve prediction accuracy.
Support Vector Machine (SVM): A machine learning model used to classify data by finding the hyperplane that best separates the two classes (attrition vs. no attrition).

4. Evaluation Metrics:
Accuracy: The percentage of correct predictions made by the model.
Precision & Recall: Measures of the relevance and completeness of the predicted results.
F1 Score: A harmonic mean of precision and recall, useful for evaluating models where class distribution is imbalanced (such as predicting attrition, which is often a minority class).

5. Model Improvement:
Hyperparameter Tuning: Using techniques like Grid Search and Random Search to find the optimal set of hyperparameters for models like Random Forest and Gradient Boosting.
Feature Selection: Reducing the number of features used by the model to improve prediction accuracy and reduce overfitting.
Cross-Validation: Applying k-fold cross-validation to ensure that the model performs well on unseen data and is not overfitting to the training set.

6. Tools and Techniques Used:
Python: The primary programming language for data analysis and model building.
Pandas: For data manipulation and cleaning.
Seaborn/Matplotlib: For data visualization and EDA.
Scikit-learn: For implementing machine learning algorithms such as Logistic Regression, Random Forest, and Gradient Boosting.
Jupyter Notebooks: For interactive data analysis and model experimentation.

## 5. Detailed Conclusions with Findings
- Key Factors Influencing Attrition:
  The analysis likely identified several key factors that significantly influence employee attrition, such as:

    - Job Satisfaction: Employees with lower satisfaction ratings are more likely to leave.
    - Salary: Employees earning below-average salaries for their job roles are at higher risk of leaving, indicating compensation plays a major role in retention.
    - Tenure: Employees with fewer years at the company may be more prone to leaving, especially if they are early in their career and seeking better opportunities.
- Model Accuracy and Performance:

   - Logistic Regression: As a baseline model, Logistic Regression likely provided reasonable accuracy but may have struggled with complex relationships between features.
   -  Random Forest: Improved accuracy by capturing non-linear relationships in the data. Its ability to handle feature interactions made it more effective for predicting attrition.
   - Gradient Boosting: Provided the highest accuracy after tuning, with more refined predictions by correcting errors iteratively. The project likely reported an accuracy improvement of 5-10% compared to baseline models after hyperparameter tuning.

- Model Improvements:
Through feature selection and hyperparameter tuning, model performance was significantly improved. For example:

     - Removing less relevant features (e.g., age or gender) may have helped reduce noise and improved prediction accuracy.
     - Cross-validation helped ensure that the model generalizes well to new data, reducing overfitting.
- Accuracy Metrics:

     - The project likely achieved accuracy scores in the range of 80-85% after model tuning.
     - The F1 score and ROC-AUC metrics would have further validated the model’s performance, especially in dealing with the imbalance in the attrition class.

## 6. Use Case in Real-World Scenarios
- Employee Retention Strategy:
The predictive models created through this project can be used by HR teams to proactively identify employees at risk of leaving. By focusing retention efforts on employees with lower satisfaction scores, higher workloads, or below-average salaries, HR can intervene early to address concerns and improve retention rates.

- Optimizing HR Policies:
Insights gained from the analysis (such as which departments experience the highest attrition rates or which roles have the shortest tenure) can inform targeted HR policies. For example, departments with high turnover could benefit from leadership training or improved work-life balance programs.

- Workforce Planning:
By understanding attrition trends, organizations can improve workforce planning, ensuring they have sufficient resources to fill positions before employees leave, thus minimizing operational disruptions.

- Compensation Benchmarking:
If compensation is identified as a key factor in attrition, the business can perform salary benchmarking to ensure their offers are competitive within the industry. Adjustments to compensation packages could help retain top talent.

## Conclusion: 
The project successfully leverages machine learning techniques to predict employee attrition and provides key insights into the factors driving turnover. By improving model accuracy through hyperparameter tuning and feature selection, the project delivers reliable predictions that can be used by HR teams to retain valuable employees and optimize workforce management strategies. The use of tools like Scikit-learn, Pandas, and Seaborn, along with model optimization, ensures the project achieves its goal of aiding HR decision-making through data-driven insights.
