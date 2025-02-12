# Assignment1
Name: Pothuru Sivarkamani Naga Mruthyunjaya
Student ID: 700751259  
 **TASK1**
1.	Tensor Manipulations & Reshaping
Code is present in Tensor_operations.py and output is also shown in pynb file.
This task is about performing fundamental TensorFlow operations, including:
- Tensor creation and manipulation
- Reshaping and transposing
- Broadcasting operations
Firstly I created a random tensor of shape(4,6) with tf.random.uniform function and then i found the rank and shape.
  I reshaped into (2,3,4) shaped tensor using reshape function.
  Then I transposed it into (3,2,4) shaped tensor using transpose function.
  Lastly I broadcasted a tensor(1,4) into (3,2,4). Then added that broadcasted tensor to tensor(3,2,4).

**TASK2**
2.	Loss Functions & Hyperparameter Tuning
Code is present in Lossfunctions.py and output is also shown in pynb file.
This task is to perform  
- Computations on Mean Squared Error (MSE) and Categorical Cross-Entropy (CCE) losses.
-  how modifying predictions affects the loss values.
- Visualizations on the loss values using a bar chart.
  Coming to code Firstly I defined true values(0 or 1) and model predictions.
  Then I defined the two loss functions(mean-squared error and categorical cross entropy).
  I computed MSE losses and defined true values for CCE loss because it needs to binary for this loss.
  So I one-hot encoded the values for true values and computede the cce loss.
  After that I modified the model prediction values and computed the values for both losses.
  I visualised the both results with help of matplotlib functions.
  From the result, I observed that
  - CCE Loss is Higher than MSE Loss
  - Categorical Cross-Entropy penalizes incorrect predictions more.
  - When Predictions Become Less Confident, Both Losses Increase
  This shows that both MSE and CCE correctly capture prediction uncertainty.

**TASK3**
3.	Train a Model with Different Optimizers

  
   

