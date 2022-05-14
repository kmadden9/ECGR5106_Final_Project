# ECGR5106_Final_Project
The reference repository for the final project assignment of Dr. Hamed Tabhki's Real-Time ML class at UNCC. This repository is shared between Kevin Madden and Aaron Skow.

The final project investigate ResNet and DenseNet object classification models in the context of ASL sign detection.

# Project Abstract
Convolutional neural networks (CNNs) have been improving significantly in both performance and efficiency. Versatile architectures such as ResNet [1] and DenseNet [2] have made creating an “intelligent” object classification NN as straightforward as ever. In this paper, we apply these prominent architectures in order to recognize the American Sign Language (ASL) alphabet, as well as 3 other signs. Various techniques are utilized to generalize, expand, normalize, and, overall, improve our model’s test accuracy. In the end we test our network on webcam pictures to simulate the model’s ability to detect ASL letters in real time. The results show that a rich, robust dataset is necessary for a neural network to learn the nuances of how to distinguish sign letters from each other. Data which is not varied in its presentation of sign letters (background, position, etc.) will train a network with a narrow understanding of the ASL alphabet. Thus, resulting in low test accuracy.

# Folder Descriptions

ResNet contains training/test code for the base ResNet_10 model, ResNet_10 with dropout, ResNet_10 with batch normalization, ResNet_10 with weight decay and ResNet with 20 resblocks within a singular jupyter notebook.

DenseNet contains the training and test code for the ASL sign recognition using the models densenet121 and densenet201. The notebook containing "trainValSplit" has the first implementation of the training and validation split as well as the first use of the webcam for testing. The notebook containing "Different_Test_Set" contains a lot of the training that was carried out with the densenet121 and 201 models. It also has the first use of the test set that is referenced in the final report. The notebook containing "128" has all the training that used 128x128 images (instead of 64x64).
