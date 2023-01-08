# Cats VS Dogs 
## About Dataset
1. Cats vs Dogs is a Dataset with around 20,000 images for training and 10,000 images for Validation
2. Dataset can be found  [here](https://www.kaggle.com/datasets/salader/dogs-vs-cats) 

## About CNNs
In deep learning, a convolutional neural network (CNN, or ConvNet) is a class of artificial neural network (ANN), most commonly applied to analyze visual imagery.[1] CNNs are also known as Shift Invariant or Space Invariant Artificial Neural Networks (SIANN), based on the shared-weight architecture of the convolution kernels or filters that slide along input features and provide translation-equivariant responses known as feature maps.[2][3] Counter-intuitively, most convolutional neural networks are not invariant to translation, due to the downsampling operation they apply to the input.[4] They have applications in image and video recognition, recommender systems,[5] image classification, image segmentation, medical image analysis, natural language processing,[6] brain–computer interfaces,[7] and financial time series.[8]

CNNs are regularized versions of multilayer perceptrons. Multilayer perceptrons usually mean fully connected networks, that is, each neuron in one layer is connected to all neurons in the next layer. The "full connectivity" of these networks make them prone to overfitting data. Typical ways of regularization, or preventing overfitting, include: penalizing parameters during training (such as weight decay) or trimming connectivity (skipped connections, dropout, etc.) CNNs take a different approach towards regularization: they take advantage of the hierarchical pattern in data and assemble patterns of increasing complexity using smaller and simpler patterns embossed in their filters. Therefore, on a scale of connectivity and complexity, CNNs are on the lower extreme.

Convolutional networks were inspired by biological processes[9][10][11][12] in that the connectivity pattern between neurons resembles the organization of the animal visual cortex. Individual cortical neurons respond to stimuli only in a restricted region of the visual field known as the receptive field. The receptive fields of different neurons partially overlap such that they cover the entire visual field.

CNNs use relatively little pre-processing compared to other image classification algorithms. This means that the network learns to optimize the filters (or kernels) through automated learning, whereas in traditional algorithms these filters are hand-engineered. This independence from prior knowledge and human intervention in feature extraction is a major advantage.

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

![image](https://user-images.githubusercontent.com/84556711/211199346-8e9a4b80-6c4b-47fa-a19d-d1cbcad626ce.png)



## Predictions
Following are the predictions the model made on testing data

![image](https://user-images.githubusercontent.com/84556711/211199365-2db8891c-ee84-4f3c-b552-bc76392960fd.png)
![image](https://user-images.githubusercontent.com/84556711/211199374-aa8c3f97-10d4-4a90-9059-c6e9c0badf18.png)




