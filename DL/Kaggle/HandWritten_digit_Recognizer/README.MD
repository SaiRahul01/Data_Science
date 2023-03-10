# Hand Written Digit Classifier using ANN - MNIST Dataset
## About Dataset
1. MNIST is a datset with 60,000 images for training and 10,000 images for testing
2. Each image is of dimension 28 x 28 (low resolution)  images of handwritten digits
3. Dataset can be found  [here](https://www.kaggle.com/competitions/digit-recognizer/data) or can be imported directly from keras

## Model Architecture
 input layer is of dimension 784 which is fed into the first hidden layer with 128 hidden units of Relu activation function and then this is fed into the second hidden layer with 32 hidden units of Relu activation function, then these outputs are fed into the 10 dimensional output layer with Softmax activation function since we are performing Classification with 10 classes.

## Training
The training of the model included 100 epochs which was sufficient enough to produce good results. Validation data was 15% of the training data and the optimizer used was Adam optimizer.

## Model Summary
![image](https://user-images.githubusercontent.com/84556711/211181395-423a9037-2039-427e-90d3-7a97a45cf406.png)



## Predictions
Following are the predictions the model made on testing data

![image](https://user-images.githubusercontent.com/84556711/211181399-f7917348-b89a-4ec6-9131-b16dff8cbc99.png)
![image](https://user-images.githubusercontent.com/84556711/211181403-383c25e8-7682-4889-9b45-5360cc553f72.png)




## Accuracy
Accuracy achieved by the above described model on the MNISIT dataset is 97.79%.
