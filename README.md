The notebook contains model to **classify the MNIST dataset using Tensorflow.** 
--------------------------------------------------------------------------
The notebook is divided into five main parts:

* Data Pre-processing 
* Building the Model 
* Optimizing the Model
* Evaluating the Model
* Training the Model 

Dependencies required for this notebook:

``````````
import tensorflow as tf

from tensorflow.keras.layers import Dense, Flatten, Conv2D
from tensorflow.keras import Model
import numpy as np

```````````
Note: TensorFlow version: 2.8.0 is used.

Notebook file in detail: 

1. Data Pre-processing:
	* Import MNIST dataset and split the data into train and test set and add a channels dimensions. 
	* Data Augmentation is conducted by rotating the images by 180 degrees. 
	* Data is shuffled and batch size of 32 defined. 
2. Building the Model:
	* Model is built applying Conv2D to build simple Convolutional Neural Network layer with activation function. 
	*  Flatten and Dense layer is applied.
3. Optimizing the Model:
	* Adam Optimizer is applied.
	* Sparse Categorical cross entropy loss is used to computes the crossentropy loss between the labels and predictions. 
4. Evaluating the Model:
	* Performance of the model is evaluated using loss and accuracy for train and test state. 
5. Training the Model: 
	* Model is trained using tf.GradientTape which is Tensorflow's API for automatic differentiation. 
	* Model is trained on epoch 6 with test accuracy of 98.45. 
The following results could be improved by using Dropout and conducting more comprehensive data augmentation processes. 

This notebook file is referenced from Tensorflow tutorials: https://github.com/tensorflow/docs/tree/master/site/en/tutorials
