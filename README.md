# fashion-mnist-implementation-with-keras
Classification of fashion mnist with Keras

This is a experiment is to classify fashion-MNIST dataset with keras, using a Convolutional Neural Network (CNN) architecture. In just a few lines of code, you can define and train a model that is able to classify the images with over 93% accuracy, even without much optimization.

Fashion-MNIST can be used as drop-in replacement for the original MNIST dataset (10 categories of handwritten digits). It shares the same image size (28x28) and structure of training (60,000) and testing (10,000) splits. It’s great for writing “hello world” tutorials for deep learning.

Keras is popular and well-regarded high-level deep learning API. It’s built right into to TensorFlow — in addition to being an independent open source project. You can write all your usual great Keras programs as you normally would using this tf.keras, with the main change being just the imports. Using tf.keras enables you to take advantage of functionality like eager execution and tf.data — should you like to down the road. Here, I’ll cover basics.

Label Description

0 ----- T-shirt/top\
1 ----- Trouser\
2 ----- Pullover\
3 ----- Dress\
4 ----- Coat\
5 ----- Sandal\
6 ----- Shirt\
7 ----- Sneaker\
8 ----- Bag\
9 ----- Ankle boot\

Dataset of 60,000 28x28 grayscale images of 10 fashion categories, along with a test set of 10,000 images.

### Importing Libraries
<p align="center">
  <img src="data/1.png"  width=965 height=189>
</p>

### loading data
the data has been loaded keras.datasets which are available
<p align="center">
  <img src="data/2.PNG"  width=967 height=77>
</p>

### Visualizing data
the data has been explored visually to know the different categories available and label are provided as in Keras documentation, and visual interpretation has been used to know number of images for each category.
<p align="center">
  <img src="data/3.PNG"  width=968 height=321>
  <img src="data/4.PNG"  width=971 height=286>
  <img src="data/5.PNG"  width=971 height=383>
  <img src="data/6.PNG"  width=970 height=344>
</p>

### Expanding the axes to fit 4D Conv model
According to the dataset, the shape of image is (28x28), it was expanded to (28x28x1) here
<p align="center">
  <img src="data/8.PNG"  width=968 height=68>
</p>

### Scaling the data and converting categorical labels to Continous
<p align="center">
  <img src="data/9.PNG"  width=970 height=145>
</p>

### Building the model
to study the model, go for model.summary()
<p align="center">
  <img src="data/10.PNG"  width=970 height=305>
</p>

### Calling the Tensorboard
to configure the Tensorboard
<p align="center">
  <img src="data/11.PNG"  width=972 height=145>
</p>

### Fitting the model
<p align="center">
  <img src="data/12.PNG"  width=971 height=437>
</p>

### Evaluating the model
By the result, the accuracy obtained is 93.31% on test dataset and validation loss of 0.2859
<p align="center">
  <img src="data/13.PNG"  width=971 height=90>
</p>
