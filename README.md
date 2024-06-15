# Driver Drowsiness Detection using CNN
This repository contains Python code for detecting driver drowsiness using deep learning and computer vision techniques. The system monitors the driver's eye movements in real-time using a webcam and alerts if signs of drowsiness are detected.

## Features
1)Eye Detection: Utilizes Haar cascades for detecting eyes in the driver's face captured by the webcam.<br/>
2)Deep Learning Model: A CNN model trained to classify eye images as "Open" or "Closed" is used to determine the driver's eye state.<br/>
3)Real-time Monitoring: The system continuously monitors the driver's eye status and raises an alarm when signs of drowsiness, such as closed eyes for an extended period, are detected.<br/>
4)Configurability: Easily configurable parameters such as the alarm sound and drowsiness detection threshold allow customization according to specific requirements.<br/>
## Requirements<br/>
Python : The code is compatible with Python 3 .<br/>
OpenCV: OpenCV library is used for capturing video frames from the webcam and performing image processing tasks.<br/>
NumPy: NumPy is utilized for numerical operations and array manipulation.<br/>
TensorFlow: TensorFlow is required for loading and using the pre-trained deep learning model.<br/>
Keras: Keras, as a high-level neural networks API, is used for building and training the deep learning model.<br/>
playsound: The playsound library is used to play the alarm sound when drowsiness is detected.<br/>

Download the Dataset from the link given below and edit the address in the notebook accordingly.<br />
Run the Jupyter Notebook and add the model name in detect_drowsiness.py file in line 20.<br />

## The Dataset
The dataset which was used is a subnet of a dataset from(https://www.kaggle.com/datasets/dheerajperumandla/drowsiness-dataset)<br />
it has 4 folder which are <br />1) Closed_eyes - having 726 pictures<br />
                          2) Open_eyes - having 726 pictures<br />
                          3) Yawn - having 725 pictures<br />
                          4) no_yawn - having 723 pictures<br />

## The Convolution Neural Network
![image](https://github.com/OMDeshmukh317/Driver-Drowsiness-Detection-using-CNN/assets/95094190/638e799f-6196-443c-b4a3-6c7cfa4a6263)



## Accuracy 
We did 50 epochs, to get a good accuracy from the model i.e. 98% for training accuracy and 96% for validation accuracy.
![image](https://github.com/OMDeshmukh317/Driver-Drowsiness-Detection-using-CNN/assets/95094190/7bfa42a2-67f5-4142-b797-440560db5186)


## The Output 
1. Open Eyes<br />
![image_2024-06-15_23-16-03](https://github.com/OMDeshmukh317/Driver-Drowsiness-Detection-using-CNN/assets/95094190/0f19fa07-713a-4736-a5ad-1c199c544ff7)

2. Close Eyes<br />
Here we detect wheater the eyes are closed and count the number of frames for which the eyes were closed (which is 5 frame) greater then that the Alarm will ring and the WARNING sign is displayed.
![image_2024-06-15_23-15-24](https://github.com/OMDeshmukh317/Driver-Drowsiness-Detection-using-CNN/assets/95094190/3b47207c-41a9-4970-b7c6-92cfd218766c)
