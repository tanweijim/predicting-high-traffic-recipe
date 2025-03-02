# About Tasty Bytes
Tasty Bytes was founded in 2020 in the midst of the COVID-19 pandemic. The world wanted
 inspiration so we decided to provide it. We started life as a search engine for recipes, helping
 people to find ways to use up the limited supplies they had at home.
 Now, over two years on, we are a fully fledged business. For a monthly subscription we will put
 together a full meal plan to ensure you and your family are getting a healthy, balanced diet
 whatever your budget. Subscribe to our premium plan and we will also deliver the ingredients
 to your door.

 # Project Overview
- High-traffic recipes increase overall website traffic by up to 40%, leading to more subscriptions and engagement
- Predict recipes that will lead to high traffic on the website
- Minimize the chance of displaying unpopular recipes
- Deploy predictive analytics to correctly predict high-traffic recipes 80% of the time

# Model Development
**Logistic Regression Model (baseline model) -** 
  A linear model used for binary classification. It uses a logistic function to predict the probability of a binary outcome and fits a decision boundary to separate the classes.

**Random Forest Classifier (comparison model) -**
  An ensemble model that combines multiple decision trees. It builds multiple trees during training and averages their predictions. This model can capture complex, non-linear relationships between features and uses bagging to reduce overfitting

  # Key metrics
1.	**Accuracy:** Measures the model’s overall detection accuracy by calculating the proportion of correct predictions.
2.	**Precision:** Measures the model’s ability to correctly identify relevant objects by calculating the ratio of true positives to all detections.
3.	**Recall:** Evaluates the model’s ability to detect all true objects by calculating the ratio of true positives among all actual truth instances.

#   Model Evaluation

| Model       | Accuracy  | Precision (Class 0)  |  Precision (Class 1)   | Recall (Class 0)   | Recall (Class 1)   |
| ----------- | :----: | :----: |  :----: | :----: | :----: |
| Random Forest Regressor | 0.75      | 0.67       | 0.80       | 0.67       | 0.80       |
| Extra Trees Regressor   | 0.70       | 0.61       | 0.76       | 0.59       | 0.77    |

1.	Precision: Logistic Regression has higher precision for both classes, meaning it makes fewer false positive predictions.
2.	Recall: Logistic Regression has a higher recall for Class 1 (high-traffic recipes at 80% of the time), meaning it correctly identifies more high-traffic recipes.
3.	Accuracy: Logistic Regression has higher overall accuracy, indicating it correctly predicts more instances overall compared to Random Forest, making it the better-performing model.

# Recommendations
- Adopt Logistic Regression as the primary model as it outperforms the Random Forest in terms of precision, recall and accuracy.
- It is more effective in predicting high-traffic recipes, and also has fewer misclassifications (false positives and false negatives), which reduces the risk of incorrect predictions.
- Continuously monitor model performance over time to ensure it remains effective as new data comes in. Track key metrics and detect any degradation in performance.
- Explore feature engineering for further improvements to the model. Test other models to ensure no better alternative exists.
- Since model achieves 80% recall for high-traffic recipes (Class 1), the business can :
   - Prioritize marketing efforts for high-traffic recipes.
   - Optimize inventory management for ingredients used in these recipes.
   - Improve customer satisfaction by promoting popular recipes.
