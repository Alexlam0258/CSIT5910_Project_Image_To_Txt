# 2022 CSIT 5910 Group 2 Project
##  Topic: An Application of Transformer and GAN: Text to Image Synthesis

In this project, there would be three parts: Transformer, Image Encoder and GAN (?). 
The transformer will be used to embed the text description of the image into a set of vector. Similarly, the image encoder is used in embedding the image into a set of vector. To link up with two set of vectors, a loss function is built to minimise the L2 distance between two vectors in the same pair and at the same time, it will penalise the loss function if the image vector and the text vector is not in the same pair. 

All in all, the loss function is defined as L2-distance of same pair / average of L2-distance of different pairs.

After training the model of image-text classifier, the GAN(?) will be employed to generate large amount of images. Then, the trained classifier will be employed to link up with the closest pair of generated image and inputted text.