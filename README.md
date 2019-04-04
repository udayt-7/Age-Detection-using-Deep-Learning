# Age-Detection-using-Deep-Learning
The task is to predict the age of a person from his/her facial attributes, it is a multi-class problem where the age of the subjects is categorized into classes such as Young, Middle and Old. The obtained images have different dimensions, multiple viewpoints as such that needs to be processed. A model that is capable of predicting age amid these challenges is built and tested for accuracy.

The data has 2 parts - Train and Test data
  Train data contains 19000 images
  Test data contains 7000 imags
  train.csv file - contains 2 columns ID [Name of the jpg file]
                                      Class [age class of the image]
  test.csv file has ID of all the test images and the class should  be predicted!
  

I have used Convolution Neural Networks  along with a Sequential model
The main layers used are
    1. Input Layer
    2. 2 Convolutional Layers with Relu as a Activation function
    3. 2 MaxPooling Layers with 2,2 output matrix
    4. 2 Dropout Layers 
    5. 1 Flatten Layer
    6. 3 Dense Layers [2 with Relu and 1 with Softmax function]

For training the model with above layers i got around 97% accuracy

I then split the training data of 19000 as train and test for validation and tested for accuracy in which around 82% accuracy had been obtained.

Then i tried doing Data Augmentaion so that the model could learn better, the accuracy had actually reduced to around 86%,
Then i predicted the outcome of age group for Test data.

The test data could not be verified completely but most of the images that were compared with the observed data and predicted data turned out to be accurate,

Future work includes converting the images to grayscale so that the feature encoding is much more efficient and accurate to train the model.

