# Facial_Attribute_Classification
Lila Schisgal and Phoebe Jeske

This project aims to create a convolutional neural network which, when given an image of a face, can recognize various attributes such as the accessories, hairstyles, and expressions. It does this using the CelebFaces Attributes DataSet. We are doing our intitial train solely looking for eyeglasses, with the intent to build up the network with more attributes once we have trained it to look for that feature.

The basicmodel.ipynb file contains both our updated data processing and our model initialization. The data_processing.ipynb file has not been updated, and currently just includes our work from milestone 1. We have edited our data processing to use a data generator in order to deal with the tremendous size of our dataset.

After the data processing, we intialize a Sequential model to begin our recognition process. Currently, we have a binary classification model. This is because for this milestone we are just attempting to recognize one attribute, glasses. As we make it more advanced for future models we will switch our model type to categorical cross entropy. 


@inproceedings{liu2015faceattributes,
  title = {Deep Learning Face Attributes in the Wild},
  author = {Liu, Ziwei and Luo, Ping and Wang, Xiaogang and Tang, Xiaoou},
  booktitle = {Proceedings of International Conference on Computer Vision (ICCV)},
  month = {December},
  year = {2015} 
}
