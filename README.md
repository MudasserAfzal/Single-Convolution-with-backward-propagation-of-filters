# Single-Convolution-with-backward-propagation-of-filters

The dataset used for this work is Cifar10.

Note: this is a incomplete assignment which means that the loss and accuracies are not that up to the mark. but the purpose here is to show you guys that how can we implement the backward propagation and update the weights of FCN and the filters for convolution layer. So we start with random features and train them.


In CNN firstly we have to implement convolution function in which I, implement a single step of convolution, in which you apply the filter to a single position of the input. This will be used to build a convolutional unit, which Takes an input volume, Applies a filter at every position of the input and Outputs another volume (usually of different size). As cifar data is three dimensional so we have to apply the filter to every channel and at the end add them up to make a 2D image After performing convolution, we normally do pooling operation which can max or average pooling with the main purpose to reduce the dimension of data which help in using less computation power. In both of these steps, we have to first calculate the dimension of the output value and then we execute out width and height loop with the condition on output dimension.

This methodology helps us to carry out a controlled operation. After pooling our task is to do backpropagation on filters to update them because we don’t want to add all weights on FCN. We then implement back_convolution and back_pooling function which get back the original image and update the filter vectors.

___________________________________________________________________________________________________________________________________
In case of any query feel free to ask
