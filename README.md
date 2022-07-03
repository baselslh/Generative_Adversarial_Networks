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

## Assignment 2
### Assignment Goal:
Implementing A Deep Convolutional AutoEncoders for reconstructing the images of the MNIST dataset.

### Assignment Details:
In this Assignment, you will use "convautoencoderimage.py" and make the following modifications:

1- The encoder and decoder should include more convolution, pooling, upsampling layers. In other words, a more deeper netwok is required.

2- A separate decoder model should be built in addition to the complete autoencoder and the encoder model.

3- Randomly select K images from the test set (K is a parameter that could be changed) and follow the below procedure:
Pass the image to the encoder model to get its code then pass the code to the decoder model to reconstruct the decoded image.
Visualize the original image, its code, and its decoded image

## Assignment 3
### Assignment Goal:
Implementing A Deep Dense Variant AutoEncoders (VAE) for reconstructing the images of the MNIST dataset.

### Assignment Details:
In this Assignment, you will use "vae_dense_based.py" and make the following modifications:

1-Modify the encoded data by two different methods with different values as below and trace the effect of such modification.


	z_zz = encoder.predict(x_train)

	Method 1: x_decoded = decoder.predict(z_zz[2]+Val1)   try different values for Val1 and figure-out the effect

	Method 2: x_decoded = decoder.predict(z_zz[0]+z_zz[1] * Val2)    try different values for Val2 and figure-out the effect

2-A deeper network is required. The encoder and decoder should include more layers.

3-Try different latent dimensions and figure-out the effect.