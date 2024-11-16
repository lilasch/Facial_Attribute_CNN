# Facial Attribute Classification
Lila Schisgal and Phoebe Jeske

This project aims to create a convolutional neural network which, when given an image of a face, can recognize various attributes such as the accessories, hairstyles, and expressions. It does this using the CelebFaces Attributes DataSet. 

The Final_project.ipynb file contains our final model. The milestone_1 and milestone_2.ipynb files are remnants from the previous milestones left to show the evolution of our code.

In order to accurately recreate our work, the user should use the following:
Tensorflow 2.15.0
scikit-learn 1.2.2
Pandas 2.0.3
NumPy 1.25.2
Seaborn 0.13.1
Matplotlib 3.7.1

The zip file is not included in our repository due to its excessive size. However, when locally downloaded from [our data source](https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) and added to the local repository clone, our code properly unzips it and accesses all of the images. It uses a generator to process them without using all of the systems processing power.

After the data processessing, we load in a pre trained model using transfer learning, upon which we add our own custom layers. The model uses binary crossentropy to find the individual prediction for each of the forty categories it is being trained to predict.

Afterwards, there are a series of evaluation codes. The precision, f1, and accuracy are output for each category. A confusion matrix for each category is created.

Finally, the user has the option to see the outputs from the matrix on individual photos, comparing with the photo. They can either use the predict_single_image code on one of the images from the dataset, or use the predict_real_image function to see the outputs the model would give one of their pictures. Two sample images for predict_real_image, sam.jpg and lila.png, are available in the repository.


@inproceedings{liu2015faceattributes,
  title = {Deep Learning Face Attributes in the Wild},
  author = {Liu, Ziwei and Luo, Ping and Wang, Xiaogang and Tang, Xiaoou},
  booktitle = {Proceedings of International Conference on Computer Vision (ICCV)},
  month = {December},
  year = {2015} 
}
