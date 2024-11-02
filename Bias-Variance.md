1. Bias-Variance Trade-off :
   
Bias: It is phenomena that skews the result of an algorithm in favour or against an idea(Training data). High bias means the model is too simple and doesn't capture the underlying patterns well, leading to underfitting. Underfitting results in poor performance on both the training data and unseen data.

Variance: Refers to the changes in the model when using different portions of the training or test data. High variance means the model is too complex and captures noise or random fluctuations in the training data, leading to overfitting. Overfitting results in good performance on the training data but poor performance on unseen data.

2. Balancing Bias and Variance
The goal is to find a middle ground where the model captures the underlying patterns in the data (low bias) without overfitting to noise (low variance). This is where hyperparameter tuning plays a role.

3. Impact of Hyperparameter Tuning
High Bias (Underfitting):
If hyperparameters like max_depth are set too low, the tree will be too shallow, and the model will be too simplistic. It won't capture the complexity of the data, leading to high bias.
High Variance (Overfitting):
If hyperparameters like max_depth or min_samples_split are set too high (or too low, in the case of min_samples_split), the tree becomes too deep and complex, capturing even noise in the data. This leads to high variance, where the model performs well on the training data but poorly on unseen data.

4. Generalization to Unseen Data
Generalization means that the model performs well not only on the training data but also on new, unseen data. A well-tuned decision tree has an appropriate balance between bias and variance, ensuring that it captures the essential patterns in the data without being overly influenced by noise or small fluctuations in the training set.

Example:
If you set max_depth=2, the tree will be very shallow and may miss important patterns (underfitting, high bias).
If you set max_depth=20, the tree might become very complex and memorize the training data, including irrelevant details (overfitting, high variance).
Tuning max_depth=5, for instance, might give a good balance where the tree captures key patterns but doesn't overfit, leading to better performance on unseen data.
