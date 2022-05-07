# CNN Food Image Classifier
The Image processing model was implemented using Convolutional Neural Network model through Keras and TensorFlow in python. The basic idea of CNN is to extract low level and high-level features from training dataset, assign random weights and biases and eventually fine-tune and learn these values. These weights and biases along with suitable activation functions are stored in the model which is generated by batchwise training over train dataset. The model can classify for an unseen input data, generally referred as test data because of these values. We created our own CNN architecture using Keras. The model type was Sequential, which allows to build a model layer by layer. Four convolutional layers along with pooling, flattening and dense layer. Gradient, color, dimensions, edges are few low-level features that are extracted by convolutional layer. The addition of more layers enables the model to capture high level features and hence a proper understanding of each image is established.
![Covolutional Operation](https://www.google.com/url?sa=i&url=https%3A%2F%2Fanalyticsindiamag.com%2Fconvolutional-neural-network-image-classification-overview%2F&psig=AOvVaw3Z8C0nIKnyMNs40v3-Xxa4&ust=1652012557886000&source=images&cd=vfe&ved=0CAwQjRxqFwoTCMi5hcWwzfcCFQAAAAAdAAAAABAf)
<br>
<br>
The methodology of CNN is quite like that of traditional ML algorithms – input, feature extraction, feature map, and classification. However, unlike ML algorithms the features are learned automatically by CNN network. The initial convolutional layers are responsible for feature extraction. The size of filter provided to Keras functions decided the dimensions of filter matrix in each convolution layer. The filter performs convolution operation by dragging the kernel matrix over same size portion of image and calculates product of matrix multiplication. The advantage lies in the fact that unlike traditional ML approach, we don’t have to hard-code the feature extractors. They are automatically assigned by the CNN algorithm We found out that features like corner, texture, shape, and edge were extracted by neural network. These features are automatically selected and updated.

Although CNN algorithm has capability to tackle highly complex problems, but it becomes important that parameters are selected appropriately. We performed hit and trail approach to select appropriate values for model. Various combination of number of filters in each layer, number of epochs and different activation functions were used in hyper-tuning the model in order to achieve an accurate and effective model. Training Accuracy and Training Loss are metrics associated with model’s performance with training dataset i.e., seen data, whereas Validation accuracy and validation loss refers to performance of model w.r.t. unseen data. Hence, we give more priority to validation accuracy and validation loss while deciding value of any parameter. 
