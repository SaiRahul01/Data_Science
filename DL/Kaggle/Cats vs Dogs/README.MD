# Cats VS Dogs 
## About Dataset
1. Cats vs Dogs is a Dataset with around 20,000 images for training and 10,000 images for testing
2. Dataset can be found  [here](https://www.kaggle.com/datasets/salader/dogs-vs-cats) 

## Model Architecture
Input Image is first Flatten into 1D array and fed into the CNN Model.

 1. a 2D convolution is applied with 32 kernels each of dimension 3x3 with activation of Relu
 2. Batch Normalization is carried out thereafter
 3. MaxPooling Layer with Pool Size of 2x2 with stride=2 and activation being Relu

 4. a 2D convolution is applied with 64 kernels each of dimension 3x3 with activation of Relu
 5. Batch Normalization is carried out thereafter
 6. MaxPooling Layer with Pool Size of 2x2 with stride=2 and activation being Relu

 7. a 2D convolution is applied with 128 kernels each of dimension 3x3 with activation of Relu
 8. Batch Normalization is carried out thereafter
 9. MaxPooling Layer with Pool Size of 2x2 with stride=2 and activation being Relu

    Dense layer of 128 units follwed by a dropout of 0.15 then a Dense layer of 64 units follwed by a dropout of 0.15 both with relu activation function, Finally it is fed into a single node with sigmoid activation to ouput 0(Cat) or 1(Dog).
## Training
The training of the model included 10 epochs which was sufficient enough to produce good results.optimizer used was Adam optimizer.

## Model Summary




## Predictions
Following are the predictions the model made on testing data





