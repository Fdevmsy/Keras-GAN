# 3D Shape Completion 

## Introduction

This is a Keras Implementation of 3D Encoder-Decoder Generative Adversarial Network (3D-ED-GAN) for 3D shape Inpainting. The 3D-ED-GAN is a 3D convolutional neural network trained with a generative adversarial paradigm to fill missing 3D data. The cuboid data is generated through Python code and a random masking is applied to each instance to create corrupted shapes. 

In this experiment, since the shape is pretty simple, the network gives excellent performance after 3000 epochs. 

## Requirement

`Tensorflow-gpu==1.7.0`

`Keras==2.20`

## Example

~~~
python EncoderDecoderGAN3D.py
~~~

For the fist few epochs: 

![](images__32cube/photo_2018-07-06_19-34-57.jpg)


![](images__32cube/photo_2018-07-06_19-35-00.jpg)

After 2000 epochs:

![](images__32cube/photo_2018-07-06_19-34-53.jpg)

![](images__32cube/photo_2018-07-06_19-33-51.jpg)

![](images__32cube/photo_2018-07-06_19-33-26.jpg)

## Higher Resolution

3D convolutional neural networks are pretty computational expensive. I also tried 64^3 cubes and 64x32x32 shapes. The 64^3 cubes obviously need more memory and time to train. 

## Other Applications

This code can be easily applied to other dataset like ShapeNet. The input format used in this code is illustrated in voxelFormat.pdf

## Reference

[1] [https://github.com/eriklindernoren/Keras-GAN](https://github.com/eriklindernoren/Keras-GAN)

[2] [Shape Inpainting using 3D Generative Adversarial Network and Recurrent Convolutional Networks](https://arxiv.org/abs/1711.06375) Weiyue Wang, Qiangui Huang, Suya You, Chao Yang, Ulrich Neumann. 

## Contact 

**Maker Collider**

**Shiyu Mou**

**shiyumou@usc.edu**