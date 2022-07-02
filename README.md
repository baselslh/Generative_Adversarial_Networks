# Generative_Adversarial_Networks

## General info
This are the assignments that i had to complete in Generative_Adversarial_Networks course

## Assignment 1
- Read and prepare the circle points data 
- Geom.csv -> contains 22 circle sample and each circle sample contains 61 points (x,y coordinates) 
- Circles are with different radius but all are centered around origin. 
- Split the circle samples into training data (17 samples) and testing data (5 samples) 
- Building Autoencoders in Keras for reconstructing the circle points.  
    - Start with a single fully-connected neural layer for the encoder and also for the decoder. 
    - Try different code sizes (60,30). 
    - Create a separate encoder model as well as the decoder model. 
    - Train the autoencoder to reconstruct the circle points using only the training data.
- Verifying Results of our Autoencoder (Repeat the below steps for different code sizes (60,30)). 
    - Encode the testing data using the encoder model. 
    - Given the generated codes -> use the decoder model to reconstruct the circle points. 
    - Visualize the reconstructed circle points against their original circle points using the Matplotlib. 
    - Set the axis range to the biggest circle across the data. 
- For each test sample -> calculate the MSE between the original circle points and its reconstructed circle points.


