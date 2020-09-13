# Credit Risk
Brief summary and analysis of the models’ performance. Describe the precision and recall scores, as well as the balanced accuracy score. Additionally, include a final recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Accuaracy is how good the model is at predicting risk. Precision is the ratio of what our model predicted correctly to what our model predicted. For each category/class, there is one precision value. We use precision where the cost of getting a prediction wrong is much higher than the cost of missing out on the right prediction.  Recall is the ratio of what our model predicted correctly to what the actual labels are. Similar to precision, for each category/class, there is one recall value. We focus on recall when we have a FOMO(Fear Of Missing Out ) situation. Ideally, you want the model to capture all examples of a particular class. If we want our model to have a balanced precision and recall score, we average them to get a single metric. The F1 score, the harmonic mean (HM) of recall & precision. HM penalizes the model the most when even one of Precision and Recall is low.
Hence HM is more reliable to be F1-score compared to other means and most definitely must be used to evaluate if we are not in a position to decide levels of Precision and Recall.


## Resampling
### Naive Random Oversampling -
precision high risk = 0.01
recall high risk = 0.72
balanced accuracy score = 0.615
F1 high risk score  = 0.02
Model not good at predicting risk due to the low scores. Expectation for predicting high risk should be as close to 1 as possible. Specifically the balanced accuracy score and the recall score.

### SMOTE Oversampling -
precision high risk = 0.01
recall high risk = 0.60
balanced accuracy score = 0.624
F1 high risk score  = 0.02
Model not good at predicting risk due to the low scores. Expectation for predicting high risk should be as close to 1 as possible. Specifically the balanced accuracy score and the recall score.

### Undersampling -
precision high risk = 0.01
recall high risk = 0.55
balanced accuracy score = 0.488
F1 high risk score  = 0.01
Model not good at predicting risk due to the low scores. Expectation for predicting high risk should be as close to 1 as possible. Specifically the balanced accuracy score and the recall score.

### Combination Sampling -
precision high risk = 0.01
recall high risk = 0.72
balanced accuracy score = 0.642
F1 high risk score  = 0.02
Model not good at predicting risk due tothe low scores. Expectation for predicting high risk should be as close to 1 as possible. Specifically the balanced accuracy score and the recall score.

## Ensemble
### Balanced Random Forest Classifier
precision high risk = 0.04
recall high risk = 0.64
balanced accuracy score = 0.776
F1 high risk score  = 0.07
Model not good at predicting risk due tothe low scores. Expectation for predicting high risk should be as close to 1 as possible. Specifically the balanced accuracy score and the recall score.

### Easy Ensemble AdaBoost Classifier
precision high risk = 0.07
recall high risk = 0.90
balanced accuracy score = 0.92
F1 high risk score  = 0.14
Model semes to be good at predicting risk due to the higher scores. Expectation for predicting high risk should be as close to 1 as possible. Specifically the balanced accuracy score 0.092 and the recall score 0.90. However the F1 is low but could be irrelevant in this case. 

A solution to this could be to add an additional data set to compare and analyze or trying an additional model such as SMOTEEN (SMOTE and Edited Nearest Neighbors)




