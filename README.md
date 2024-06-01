
# **Summary and Discussion**


> I have  implemented the **Logistic Regression model from scratch using numpy and pandas only** , for classifying the heart disease dataset. The steps included data preprocessing, model initialization, training, and evaluating its performance.

# **Data Preprocessing**

> After checking for nulls and removed the duplicates, I have applied feature scaling by standardizing them to have a mean of 0 and std of 1, scaling the data is an essential step for optimizing and to prevent the features with larger values from dominating the process



> then I randomly shuffled the data and splitted it into training and testing with the ratio (80:20)


#**Model Implementation**
*The logistic regression model was implemented  as follows:*

1.   Initialize the weights and bias = 0
2.   mapping the linear combination (z) into 0 and 1 by using the **Sigmoid function**.
1.   Loss funciton : The binary cross-entropy loss function was implemented to measure the performance.
2.   Gradient Descent:  to update the weights and bias iteratively. The learning rate was set to 0.05, and the model was trained for 5000 epochs.

During Training process, I  printed the loss in each interval to monitor the model while leraning.
After predicting and evaluating the model, the accuracy where calculated as follows:
* **Training Accuracy: 85.12%**
* **Testing Accuracy: 81.96%**


## **Some Notes:**
* The initial loss was high, but it decreased significantly after each epoch, and that indicated that the model was learning.
* But after several epochs the loss remained the same , which means that the model (gradient descent) has reached a local minimum.
* since the final accuracies were high, that indicates that the model was generalized
* I applied hyper-parameter tuning to choose the suitable learning rate and epochs
