# The Simpsons Character Recognition and Prediction:

**Project Background:**

The project aim to classify 18 Simpsons characters.The pretrained model detect and classify images with multiple characters.

**Dataset Description:**

The Simpsons characters data is a public dataset created by Alexandre Attia. The raw data contains 41,866 pictures for 42 unique characters. We divided pictures into two datasets: Training set(80%) and validation set(20%).

First, we install kaggle package to import the dataset from kaggle.

Further, we connect to kaggle.

Additionally, we get all the kaggle datasets list.

Then, we download the dataset from kaggle.

Lastly, we unzip the ziped files.

Number of pictures: 41866

Number of unique labels: 42

**Modeling:**

Image classification via Convolutional neural network plays a major role in image processing, since it uses multiple filters to learn intricated feature embeddings from the original pixel under convolutional layers and adopts pooling to summary a patch of image data to understand local features. Here, a pretrained model MobileNetV2 model is used.

We first visualize 40 pictures from the dataset. 

Splitting data into train and test with trainig data(80%) and validation data(20%).

We use ImageDataGenerator from keras to load images.
Later, we used pretrained model MobileNetV2 to train the training dataset.
The model iterated over batches of the training set for 50 epochs.

The visualization of results gives val_acccuracy of 86.10%.
The classification report for all the characters is loaded which gives 85% accuracy.

We print Normalized Confusion Matrix and lastly, predicted 50 pictures with labels of Simpsons characters.

The accuracy we obtained: val_accuracy as 86.10% and test accuracy as 85.38%.



