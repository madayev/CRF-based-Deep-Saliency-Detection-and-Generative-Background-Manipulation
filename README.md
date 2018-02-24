# CRF based Deep Saliency Detection and Generative Background Manipulation

<h3 align="center">Abstract</h3>

We proposed a method to detect a saliency map of the object and manipulate the background of the given object. Saliency detection is identifying the most visually distinctive objects in an image. It is useful as a pre-processing step for many computer vision tasks. Recently, great features from convolutional neural network (CNN) has shown considerable progress in this area. However, CNN-based saliency detection results blurry map near the boundary of salient objects. Applying conditional random field (CRF) in super-pixel domain can refine the saliency map from CNN, and make sharp and fine boundaries. Generative background manipulation is the scheme that neural networks find a different and suitable background for the given object. To manipulate the background for the object, we learn the probability model of the dataset by generative adversarial networks. In our project, we first present the saliency detection using CNN and CRF, then we manipulate the saliency map by transferring saliency map to the image domain using Generative Adversarial Network(GAN).

<h4 align="center">Brief description</h4>

First, using CNN and CRF the saliency map is detected. Then the GAN, which is trained on the same dataset, generates background and foreground for the input image. 

<p align="center"><img src="https://github.com/madayev/CRF-based-Deep-Saliency-Detection-and-Generative-Background-Manipulation/blob/master/images/Figure3.png" width="70%"><br><i>Figure 1</i>. Overall scheme of proposed method</p>

Dataset: [HKU-IS dataset](http://i.cs.hku.hk/~gbli/deep_saliency.html)

<h4 align="center">Results</h4>

Results of saliency map detection using CNN and CRF  
<p align="center"><img src="https://github.com/madayev/CRF-based-Deep-Saliency-Detection-and-Generative-Background-Manipulation/blob/master/images/Figure2.png" width="70%"><br><i>Figure 2</i>. Visual comparison on the HKU-IS dataset: (from left top to right bottom) input, YS, MDF, DCL and ground truth images.</p>

Results of background generation using GAN 
<p align="center"><img src="https://github.com/madayev/CRF-based-Deep-Saliency-Detection-and-Generative-Background-Manipulation/blob/master/images/Figure1.png" width="44%"><br><i>Figure 3</i>. Background Manipulation Result on the HKU-IS dataset: (from left to right) saliency map, generated background, and ground truth.</p>

For more details, please check out the [paper](https://github.com/madayev/CRF-based-Deep-Saliency-Detection-and-Generative-Background-Manipulation/blob/master/paper.pdf).
