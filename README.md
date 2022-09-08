# Level-3-Capstone-Project-3
Training a recurrent neural network to classify the sentiment of book reviews:
This is the Third Capstone Projject on Level 3 for the Data Science Bootcamp through HyperionDev.
For this project we are required to use recurrent neural networks in Keras to try and classify a movie review as either positive or negative.

The dataset consists of two text files: positive.txt and negative.txt. Each file contains positive and negative book reviews respectively.
we will be using the title field for training purposes. 

Links to dataset:
https://github.com/JanHof/Level-3-Capstone-Project-3/blob/main/negative.txt
https://github.com/JanHof/Level-3-Capstone-Project-3/blob/main/positive.txt

there are 5 functions to load and process the data:
The 'filter_words' function strips the unwanted charaacters from the lines and converts characters to lower case.
load_ata function loads the text files in to the jupyter notebook and reads only the titles. (https://github.com/JanHof/Level-3-Capstone-Project-3/blob/main/L3T20-checkpoint.ipynb)
The titles are then added to a 'data' list.
The remaining functions convert the predictions from numeric to word and visa versa, to classes from categrorical.

The two text files are concatenated into the data list
Another list is created with the words 'positive' and 'negative' equal in lenght to the input data files.
This is then converted to a 1 or a zero depending on the response.

Data Exploration:
Further exploration is done on the data using a pandas dataframe.
Displayed the shape and the head to get a better understanding of the data.
Calculated and report the mean review size, its standard deviation and created a boxplot
Calculated the number of unique words in the dataset.
There were no missing values in the dataset.

Data manipulation:

The dataset was tokenized to prepare for the neural network.
padded data was tokenised to a lenght of 4 words.
I split the data so that 20% was used for testing.

Building the Neural Network and Analysis:

I added a recurent neural network with input dimension of 2560 and the putut of 40 initially but the output of 100 resulted in a more accurate model.
'binary_crossentropy' was used as the loss and 'accuracy' as metrics.
The'asess_model'  function calculated the  predictions, precision f1 score, recall and displayed the confucion matrix.
Further predictions were made wih a sample outside of the dataset.











