# Deep-Learning-Mobile-Updated
Updated version of Deep-Learning-Mobile Project &amp; Errors fixed

# Getting Started
These codes contain Python notebooks that guide one through the process of converting the pre-trained model into smartphone-required model files; Android Studio project for deploying models on Android devices and Xcode project for deploying models on iOS devices.

# Prerequisites
As Python is the de-facto coding language used for TensorFlow and Keras, Anaconda is used to manage the environment for creating deployment models. The Anaconda environment used for this repository can be duplicated by running the following code after installing Anaconda:

`conda env create -f Deep-Learning-Mobile.yml`
The TensorFlow and Keras installed in this environment are the CPU version of the libraries. To install the GPU versions of these libraries, need to change in the .yml file or to update after creating the environment.

# Coding IDE
The apps are developed using `Xcode IDE` for iOS and `Android Studio` for Android. For image capturing, OpenCV wrappers are used for both types of devices.

### To set up OpenCV for Android, the following links are used:

https://opencv.org/platforms/android/
https://blog.codeonion.com/2016/04/09/show-camera-on-android-app-using-opencv-for-android/
To set up OpenCV for iOS, the following links are used:

https://docs.opencv.org/2.4.13.7/doc/tutorials/introduction/ios_install/ios_install.html
https://medium.com/@dwayneforde/image-recognition-on-ios-with-swift-and-opencv-b5cf0667b79
# Using the Projects
## Android Studio Project
* Clean the Project
* Make sure that OpenCV has been built and added properly to the Project
* Add the CNN model to use in the assets folder of the Project
* Update the settings in the ImageInference.java file according to the model
* If using a different set of labels, add the labels.txt file for that respective file
## iOS Project
* Build the OpenCV2 framework and add it to the main Project
* Add the model to the Project and update the model name and image size in the ViewController.swift files
* Build the Project
