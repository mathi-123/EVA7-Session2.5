# EVA7-Session2.5
Pytorch assignment

# Submission by Malathi Murugesan

# Objectie
The aim is to build a neural network which 

1.Recognize handwritten digits when provided as an image input 
2. Add any number between 0 to 9 to the number predicted from the MNIST image

# Data

The network would use the MNIST dataset to train images to recognize handwritten digits
We would also randomly append a number between 0 to 9 to each of the image in MNIST to train the model for addition
This also means, we would append the sum of the number in the image (data label) and the newly added random number, as the second "label" in the dataset
The random number would be converted into a one-hot encoded vector while training / prediction
