# Facial_Attribute_Classification
Lila Schisgal and Phoebe Jeske

This project aims to create a convolutional neural network which, when given an image of a face, can recognize various attributes such as the accessories, hairstyles, and expressions. It does this using the CelebFaces Attributes DataSet. We are doing our intitial train solely looking for eyeglasses, with the intent to build up the network with more attributes once we have trained it to look for that feature.

After the data processing, we intialize a Sequential model to begin our recognition process. The model definition and training are in the same block, and can be run together. Currently, we have a binary classification model. This is because for this milestone we are just attempting to recognize one attribute, glasses. As we make it more advanced for future models we will switch our model type to categorical cross entropy. 

To evaluate the model there is a following block of code which prints the accuracy score.

We have two ways of processing the data: with and without a generator. The "old processing", or the processing we turned in for milestone 1, is without a generator. We have been having issues with RAM crashes using both methods, though we plan to move forward with the generator. We have tested the processing and models on small sections of our data and have confirmed that both of our models run with the data format given.

@inproceedings{liu2015faceattributes,
  title = {Deep Learning Face Attributes in the Wild},
  author = {Liu, Ziwei and Luo, Ping and Wang, Xiaogang and Tang, Xiaoou},
  booktitle = {Proceedings of International Conference on Computer Vision (ICCV)},
  month = {December},
  year = {2015} 
}
