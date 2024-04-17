# Facial_Attribute_Classification
Lila Schisgal and Phoebe Jeske

This project aims to create a convolutional neural network which, when given an image of a face, can recognize various attributes such as the accessories, hairstyles, and expressions. It does this using the CelebFaces Attributes DataSet. We are doing our intitial train solely looking for eyeglasses, with the intent to build up the network with more attributes once we have trained it to look for that feature.

After the data processing, we intialize a Sequential model to begin our recognition process. The model definition and training are in the same block, and can be run together. To evaluate the model there is a following block of code which prints the accuracy score.

@inproceedings{liu2015faceattributes,
  title = {Deep Learning Face Attributes in the Wild},
  author = {Liu, Ziwei and Luo, Ping and Wang, Xiaogang and Tang, Xiaoou},
  booktitle = {Proceedings of International Conference on Computer Vision (ICCV)},
  month = {December},
  year = {2015} 
}
