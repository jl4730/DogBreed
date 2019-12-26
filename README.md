## Project Overview

Welcome to the Convolutional Neural Networks (CNN) project in the DS Nanodegree! In this project, I will build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, the algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

The writeup of the project can be found here: https://medium.com/@jl4730/using-cnn-to-predict-dog-breed-f55954d14e3b

## Project Instructions

### Instructions

1. Clone the repository and navigate to the downloaded folder.
```	
git clone https://github.com/udacity/dog-project.git
cd dog-project
```

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`. 

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

4. Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.

5. All the packages used are embeded inside the notebook already.

## Results

In this project, I’ve built a dog breed classifier that can tell the breed of the user-uploaded pictures. Transfer learning was used to take advantage of the pre-trained ResNet-50 model. The project started with a dog detector and a human detector to identify the image type. Then the project went through 3 CNN models: self-trained 6 layer CNN, VGG model, and ResNet-50, of which ResNet is chosen as the accuracy is over 80%.
