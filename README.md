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
Code is present in AdamVsGSD.py and output is also shown in pynb file.
This taks is to train a neural network on the MNIST dataset using different loss functions and optimizers. The goal is to compare how the optimizers Adam and SGD perform with sparse_categorical_crossentropy and categorical_crossentropy loss functions.
Firstly load and preprocess the mnist dataset.
- load the data and normailze the data from (0-255) to (0-1) range.
Next, Define Loss Functions & Initialize History Dictionary.
I used sparse_categorical_crossentropy where labels are single integers (0-9).
categorical_crossentropy where labels are one-hot encoded.
history_dict stores training histories for different optimizers and loss functions.
Next create models to train with different loss functions.
Create adam and gsd loss fucntion optimizers.
Train models with adam and gsd loss functions in loop.
Lastly plot all validation losses using matplotlib functions.
From the results what I observe is
- Adam converges faster than SGD.
- SGD may perform better if tuned properly.
- categorical_crossentropy might be slightly slower due to one-hot encoding overhead.

**TASK4**
4.	Train a Neural Network and Log to TensorBoard

  
   

