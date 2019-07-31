<!-- workthrough documentation -->
<!-- This documentation only for fr v3 -->
# Intrducton

In this version we are going to work with dlib lib and face_recognition packages. TO use those packages we need to setup the necessery packages.

## What is Dlib Library?

Dlib is a modern C++ toolkit containing machine learning algorithms and tools for creating complex software in C++ to solve real world problems. It is used in both industry and academia in a wide range of domains including robotics, embedded devices, mobile phones, and large high performance computing environments.This library also work with python.

[Dlib Library Full Documentaion](http://dlib.net/)

## Face Recognition Library Module

To recognisze and manipulate faces we need to algorithm.We are going to use face recognition library which is built using dlib's state-of-the-art face recognition built with deep learning. The model has an **accuracy** of **99.38%** on the Labeled Faces in the Wild benchmark.It also provide simple command tool to do work.

## Install Dlib on Ubuntu

The step by step instructions to install Dlib on Ubuntu.Install all the libraries as Admin which  will help to errorless install.

#### System Information

* Ubuntu 18.04 LTS
* Anaconda 2019.07
* Python 3.6



**step 1: Install OS libraries**

```
sudo apt-get install build-essential cmake pkg-config

sudo apt-get install libx11-dev libatlas-base-dev

sudo apt-get install libgtk-3-dev libboost-python-dev

```
**step 2:Install Python libraries**

Try to use Virtual Environment to install Python libraries.

```
sudo apt-get install python-dev python-pip python3-dev python3-pip

sudo -H pip3 install -U pip numpy scipy matplotlib scikit-image scikit-learn ipython opencv-contrib-python



```
**step 3: Compile DLib**

Clone the code from github:
```
git clone https://github.com/davisking/dlib.git
```
Build the main dlib library
```
cd dlib
mkdir build; cd build; cmake ..; cmake --build .
```
Build and install the Python extensions:
``` 
cd ..
python3 setup.py install
```
*If there any problem to install the python extension use **sudo -H** before install.*

## Install Face Recogniton Module on Ubuntu

First, make sure you have dlib already installed with Python bindings.Then, install this module from pypi using pip3

```
sudo -H pip3 install face_recognition
```
---------------------------------

## Virtual Enviroment

First we need to install the virtual evn in our os. 


**step 1: Install venv in os**
```
sudo pip install virtualenv
```

Then go to your work folder run the terminal

**step 2:Creating venv in workpath**

```
mkdir nameofenv
eg. mkdir venv

cd venv
virtualenv env1

```

**step 3:Activate Virtual env**

```
source virtualenv/env1/bin/activate
```

--------------------------------------

# Downloading Images Dataset automatically

We are going to download our images for our training dataset. To do that,we need to download so many images and it's not easy to download manually and also time consuming. We have a proper solution for this problem. How about we are going to build a script which are going to download images automatically in order and save in a directory with sub-folder. Isn't it a best solution for our problem.So lets make a script.

Before we start building our script there are 2 options. Those are

* [Google API image downloader]()
* [Bing API images downloader](https://www.pyimagesearch.com/2018/04/09/how-to-quickly-build-a-deep-learning-image-dataset/)

Follow Those link to build your own image downloader.

---------------------------------------






