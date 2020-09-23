![licence](https://img.shields.io/badge/Keras-V2.3.1-red) ![licencee](https://img.shields.io/badge/Tensorflow-V2.0-yellow) ![licence](https://img.shields.io/badge/demir-ai-blueviolet) ![licence](https://img.shields.io/badge/Ahmet%20Furkan-DEM%C4%B0R-blue)

# Face-Recognition

In this assignment, you will build a face recognition system. Many of the ideas presented here are from FaceNet.

**Face recognition problems commonly fall into two categories:**

* **Face Verification -** "is this the claimed person?". For example, at some airports, you can pass through customs by letting a system scan your passport and then verifying that you (the person carrying the passport) are the correct person. A mobile phone that unlocks using your face is also using face verification. This is a 1:1 matching problem.

* **Face Recognition -** "who is this person?". For example, the video lecture showed a face recognition video of Baidu employees entering the office without needing to otherwise identify themselves. This is a 1:K matching problem.

FaceNet learns a neural network that encodes a face image into a vector of 128 numbers. By comparing two such vectors, you can then determine if two pictures are of the same person.

**In this assignment, you will:**

* Implement the triplet loss function
* Use a pretrained model to map face images into 128-dimensional encodings
* Use these encodings to perform face verification and face recognition

**Channels-first notation**

* In this exercise, we will be using a pre-trained model which represents ConvNet activations using a "channels first" convention, as opposed to the "channels last" convention used in lecture and previous programming assignments.

* In other words, a batch of images will be of shape (𝑚,𝑛𝐶,𝑛𝐻,𝑛𝑊) instead of (𝑚,𝑛𝐻,𝑛𝑊,𝑛𝐶).

* Both of these conventions have a reasonable amount of traction among open-source implementations; there isn't a uniform standard yet within the deep learning community. 
![](https://user-images.githubusercontent.com/54184905/94004001-b0bf1c80-fda4-11ea-98b8-814ce3b1cc97.png) 

![](https://user-images.githubusercontent.com/54184905/94003997-af8def80-fda4-11ea-81b9-3c24a6c841b4.png)

###### **References : Convolutional Neural Networks -** https://www.coursera.org/learn/convolutional-neural-networks