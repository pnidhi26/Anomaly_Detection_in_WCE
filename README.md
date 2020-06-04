# Anomaly_Detection_in_WCE

Anomaly (Diseases) Detection in Wireless Capsule Endoscope Images using UNET and RCNN

Used Tools:
-Python3
-Tensorflow
-Keras
-UNET
-Deep Learning (CNN)


I have a dataset consisting of images captured by WCE(Wireless Capsule Endoscope). 
This contains images of disease and their location ( In annocation folder which is binary images). 
Also normal images of that part (Without Disease). So task is to identify the disease in the WCE image (if it is present) and also their location.


Used Model:
The UNET was developed by Olaf Ronneberger et al. for Bio Medical Image Segmentation. 
The architecture contains two paths. First path is the contraction path (also called as the encoder) which is used to capture the context in the image. 
The encoder is just a traditional stack of convolutional and max pooling layers. The second path is the symmetric expanding path (also called as the decoder) which is used to enable precise localization using transposed convolutions. 
Thus it is an end-to-end fully convolutional network (FCN), i.e. it only contains Convolutional layers and does not contain any Dense layer because of which it can accept image of any size.

DataSet:
KID Dataset for WCE images
