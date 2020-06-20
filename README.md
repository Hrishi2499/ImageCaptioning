# ImageCaptioning
Attention mechanism is at the ground level of image captioning models.
Models are made of an encoder and decoder architecture.
Encoder is generates image vectors from the given images using convolutional neural networks (E.g. vgg16, inceptionV3, resnet50, etc. ) 
Recurrent neural networks (RNNs) are used as decoders. (E.g. Long Short Term Memory (LSTM) and Gradient Recurrent Unit (GRU)). 

# Model:-
Here we have used Inception V3 as encoder and GRU decoder.

* Here, features from the lower convolutional layer of InceptionV3 are extracted giving us a vector of shape (8, 8, 2048).
* Squash that to a shape of (64, 2048).
* This vector is then passed through the CNN Encoder (which consists of a single Fully connected layer).
* The RNN (here GRU) attends over the image to predict the next word.
* The model was trained on a subset of the Coco2017 Dataset for 100 epochs.

# Architecture:-
![Image Captioning Architecture](https://github.com/PranjalChitale/ImageCaptioning/blob/master/ImageCaptioningArchitecture.jpg?raw=true)


 
