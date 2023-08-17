# Face Mask Detection using MOBILENET V2

# Introduction

Face Mask Detection Technology is an AI based system that uses cameras to detect individuals who are not wearing masks in public places such as hospitals, schools, airport, malls and more. It is designed to help organization to monitor and enforce compliance with face mask use policies and to prevent the spread of COVID-19.

MOBILENET V2:
MobileNetV2 is an improvement over the original MobileNet
architecture,aiming to strike a balance between accuracy and computational
efficiency.The key features of MobileNetV2 include:
1. Depthwise Separable Convolution
2. Inverted Residuals with Linear Bottlenecks
3. Expansion Layer
4. ReLU6 Activation
5. Fully Convolutional Design

CNN:
A Convolutional Neural Network (CNN) is a type of deep learning algorithm that is particularly well-suited for image recognition and processing tasks. It is made up of multiple layers, including convolutional layers, pooling layers, and fully connected layers.

   
# Project Descvription
In this project, using MobileNet V2 algorithm to detect face masks. An image with
few people wearing a mask and not wearing a mask is sent as input dataset and the
segmented image of the same is obtained as output. The first step is pre-processing
where the image is resized to a particular resolution and it is converted to a numpy
array. Then, one hot encoding is performed on the images. Finally the data set is
split into training and testing. The second step is data augmentation where the
image is flipped, zoomed and finally flipped horizontally. The third step is training,
where the base model is loaded with imageNet weights and the last layer of the
pre-trained model is fine tuned. In the last fully connected layer, the average
pooling, flattening, dense, activation function (relu and softmax) and dropout value
are entered and processed. Then the model summary is obtained and configuration
is saved. In the fourth step, the optimizer loss entropy and accuracy metric are
configured and the trained model is evaluated and saved. In the fifth step, the
training loss and training accuracy data are plotted. Next, a prediction on the
training set is done. Finally, the model is evaluated. The sixth step is image
segmentation where the dataset is loaded and ID mapping is done where mask and
no mask is assigned. Next a tensorflow session is created and the Mask RCNN
model is loaded. Then, actual detection of Boxes, Class, Scores and Masks are
done. Then, instance segmentation is performed and Detection results are
visualized. Finally the model is implemented using a webcam where the video is
read by frame and resized as necessary. Then, the preprocessing function is
called to get the result of people wearing a mask and not wearing a mask along
with the accuracy in percentage.

<h3>Requirements</h3>
OpenCV,Numpy,TensorFlow,Keras


# Model Training & Testing
 
![image](https://github.com/thepoojabarui/face-maskDetection/assets/89887754/ba527599-5e02-41c8-b451-21de89122f2a)

# Implementation & Result

First, the video is read by frame and it resized as required to process.Then the preprocessing function is called Finally, people wearing a mask and not wearing a mask is predicted from the input data.The results are captured using webcam along the accuracy.

![image](https://github.com/thepoojabarui/face-maskDetection/assets/89887754/c7f2bae0-c4e0-4852-9c0e-8253686f9a11)

