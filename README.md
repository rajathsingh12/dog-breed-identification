# Dog-Breed Identification
This is a Kaggle competition that I tried and this is my very first kernel. There are a total of 120 breeds of dog. I took the help of pre-trained weights in order to get good accuracy. 


The dataset is downloaded from the following: https://www.kaggle.com/c/dog-breed-identification/data

Libraries used – Keras, Numpy, Pandas, Open-CV, Scikit-learn. 

## First Step – Importing the important libraries.

## Second Step – Data Preparation – 
•	In this step the data is loaded from the given CSV files. <br>
•	Target variables are OneHotEncoded so as to add the final predictions into the submissions file. <br>
•	Setting up of a specific image size (90x90). <br>
•	Creating lists for train, valid and test and then reading in the image files from test and train folders provided by the dataset and appending them to the list created. <br>
•	Converting the lists containing the image data as arrays. <br>
•	Splitting up the training set into train and validation sets. <br>

## Third Step – Building the CNN – 
•	Importing the libraries. <br>
•	Building the Sequential model. <br>
•	Adding a convolutional layer with 64 filters followed by a max pool layer. <br>
•	Adding another conv layer with 32 filters followed by a max pool layer. <br>
•	Adding the last conv layer with 128 filters followed by a max pool layer. <br>
•	Adding a flatten layer to flatten the images. <br>
•	Then finally adding a fully connected layer. <br>
•	Increasing the efficiency with the help of ResNet Pre-Trained weights. <br>
•	Epochs used = 32 <br>

## Fourth Step – Predicting – 
•	Predicting the values of the classifier <br>
•	Creating a new data frame and adding predicted values. <br>
•	Setting the column names as generated from OneHotEncoding. <br>
•	Inserting the test set column id to the final submission file. <br>

