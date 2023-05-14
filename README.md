CIFAR-10 Image Classification with ResNet Architecture

In this project, CIFAR-10 dataset is taken. It has 60,000 images with 10 different classes. Training dataset has 50,000 images and testing set has 10,000 images. 
ResNet model is considered as base. This model is modified to optimize the loss. Two model architectures were considered for our problem with SGD optimizer L2 regularization weight decay as 0.00001 and momentum 0.9. These models have [64,96,128,512] as the number of output channels for all the layers. And [1,2,2,2] as the stride size of the first convolution layer in each layer of the architecture. 
With these model specifications, we changed the learning rate hyper parameter from 0.1 to 0.01. Then we observed that we got optimized results for 0.05 and 0.01 values.
Then we continued in this direction. And changed the architecture of the model making [1,4,4,1] as the number of blocks in each layer of architecture. Then we observed that the results are improved. From this, we can conclude that this is the better architecture than previous.
Then, we changed the optimizer to ADAM and observed the results. And found that SGD outperforms the ADAM because it better suits the image classification problem.
