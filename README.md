# fashion-mnist-implementation-with-keras
Classification of fashion mnist with Keras

This is a experiment is to classify fashion-MNIST dataset with keras, using a Convolutional Neural Network (CNN) architecture. In just a few lines of code, you can define and train a model that is able to classify the images with over 93% accuracy, even without much optimization.

Fashion-MNIST can be used as drop-in replacement for the original MNIST dataset (10 categories of handwritten digits). It shares the same image size (28x28) and structure of training (60,000) and testing (10,000) splits. It’s great for writing “hello world” tutorials for deep learning.

Keras is popular and well-regarded high-level deep learning API. It’s built right into to TensorFlow — in addition to being an independent open source project. You can write all your usual great Keras programs as you normally would using this tf.keras, with the main change being just the imports. Using tf.keras enables you to take advantage of functionality like eager execution and tf.data — should you like to down the road. Here, I’ll cover basics.

Label Description

0 ----- T-shirt/top/
1 ----- Trouser/
2 ----- Pullover/
3 ----- Dress
4 ----- Coat
5 ----- Sandal
6 ----- Shirt
7 ----- Sneaker
8 ----- Bag
9 ----- Ankle boot

Dataset of 60,000 28x28 grayscale images of 10 fashion categories, along with a test set of 10,000 images.

'''
from keras.datasets import fashion_mnist
import matplotlib.pyplot as plt
import numpy as np
from keras.models import Sequential
from keras.layers import Dense, Dropout, Flatten
from keras.constraints import maxnorm
from keras.optimizers import RMSprop
from keras.layers.convolutional import Conv2D, MaxPooling2D
from keras.utils import np_utils
import keras.callbacks as callbacks
import seaborn as sns
'''
