# Objectives
#### Detect and localize the brain tumor using 3500+ brain MRI scans samples (brain image + tumour as mask image).
#### Understand the intuition and power of transfer learning using Resnet.
#### Know how to properly apply the techniques to speed up training process.
#### This training would drastically reduce the cost of cancer diagnosis & help in early diagnosis of tumors which could essentially be a life saver.

#### Approach: Take images of the brain MRI scans, perform the images segmentation to feed into 2 networks:
#### 1st n/w for detecting if tumour exists
#### if tumor exists 2nd n/w to detect location of tumour in brain MRI.

# Image segmentation (IS)
#### (IS): To understand and extract information from images at pixel level. It associate each pixel with a certain class.
#### The output produce by image segmentation model is called a 'mask' of the image.
#### IS can be used for object recognition and localization for various applications like medical imaging, self driving cars etc.

# UNet
#### UNet: Unlike conventional CNN, Unet encodes the image into a vector followed by decoding back again into an image having original size.
#### Unet formulates a loss function (Softmax) for every pixel in the input image which makes the segmentation problem works as classification problem at pixel level.

# RESNET overview (Residual Networks)
#### As CNNs grow deeper, vanishing gradient tend to occur which negatively impact n/w performance.
#### Vanishing gradient problem occurs when the gradient is back propagated to earlier layers which results in a very small gradient.

#### ResUNet combines UNet backbone architecture with residual blocks to overcome vanishing gradient problem in deep n/ws. It contains 3 parts:
#### (1): Encoder or contrating path
#### (2): Bottleneck
#### (3): Decoder or expansive path
#### Residual Neural networks (RNN - not Recurrent NN) includes 'skip connection' feature which enables training of 152 layers without vanishing gradient issues.
#### Resnet works by adding 'identity mappings' on top of CNN.
#### Imagenet contains 11million images and 11000 categories to train ResNet deep n/w.

[More extensive exercise is available here on Superdatascience](https://www.superdatascience.com/pages/modern-artificial-intelligence-masterclass-download-materials)
