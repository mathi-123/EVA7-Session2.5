# EVA7-Session2.5
Pytorch assignment

# Submission by Malathi Murugesan

# Objectie
The aim is to build a neural network which 

1.Recognize handwritten digits when provided as an image input 

2. Add any number between 0 to 9 to the number predicted from the MNIST image

# Data

1. MNIST dataset to train images to recognize handwritten digits

2.Randomly append a number between 0 to 9 to each of the image in MNIST to train the model for addition

3. Append the sum of the number in the image (data label) and the newly added random number, as the second "label" in the dataset
The random number would be converted into a one-hot encoded vector while training / prediction

# The network architecture

Two convolutions with pooling applied to feature map
Dropout layer
Six fully connected layers leading to the two outputs - recognized digit & addition result

The network would have 2 parts: 

a. For digit recognition

b. For adding the digit to the random number

With the output from part a, concatenate the one-hot encoded random number to the output

we get 2 outputs : 

1. A vector of 10 number giving the probabilities of the image being 0 to 9 

2.A vector of 19 numbers giving the probabilities of the addition being 0 to 18

# Model Summary

![Screenshot (4)](https://user-images.githubusercontent.com/91079217/137569289-36a89c1e-df72-443e-8ed8-21e6a6e6cf6e.png)

# The netwwork loss function

Loss function used is Negative Log Likelihood loss .

# Training logs

![Screenshot (3)](https://user-images.githubusercontent.com/91079217/137569277-ad23c527-2d70-45da-a733-25bb0e3e73e5.png)


# Plots representing the losses and accuracy

![image](https://user-images.githubusercontent.com/91079217/137569084-166983b9-f87f-4021-bc2d-2487de1d4067.png)
![image](https://user-images.githubusercontent.com/91079217/137569146-5e715e8e-5251-44c0-b710-f9f76c96d962.png)

![image](https://user-images.githubusercontent.com/91079217/137569175-813606e6-d960-4ab4-9f5b-c938d92e9e77.png)
![image](https://user-images.githubusercontent.com/91079217/137569193-e1aea8e6-e17c-43cb-98c3-69509e074c85.png)





