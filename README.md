# YOLOv1_implement_using_Tensorflow_or_Pytorch

<img width="618" alt="YOLO_architecture" src="https://user-images.githubusercontent.com/50979281/130927332-1aefef43-c67e-48db-98fe-68cd0a1ad629.png">

This repository consist of YOLO implement code for CUAI 2021 summer conference. We made these codes using Tensorflow or Pyrotch.

YOLO v1 : https://arxiv.org/abs/1506.02640

## Members
Minki Kang(School of Computer Science and Engineering, Chung-Ang University)
<br>
[Minkyu Kim](https://github.com/MinkyuKim26)(School of Electrical and Electronics Engineering)
<br>
Taeyun Kim(School of Computer Science and Engineering, Chung-Ang University)
<br>
Seungyeon Lee(School of Computer Science and Engineering, Chung-Ang University)

## Short paper
작성중!

## How to implement

### Using Tensorlfow - Minki Kang, Minkyu Kim

 For easy implementation, we use VGG or DenseNet which are made in Tensorflow so that input image size change to 224 x 224 when we use VGG as backbone network.
we choose same training method with YOLO, except that we use [ModelCheckpoint](https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/ModelCheckpoint) and do not use data argumentation in training dataset. By using ModelCheckpoint, we get the model that has lowest validation loss in training

#### test result
when we test our YOLO in training and test dataset. it shows good performance in training dataset, but poor performance in test dataset(overfitting). we think the reason of overfitting is skipping data argumentation in training set

### Using Pytorch - Taeyun Kim, Seungyeon Lee



## How to test our model

Minki Kang : 

Minkyu Kim : download YOLO_test.ipynb in YOLOv1_implement_using_Tensorflow_or_Pytorch/MinKyu Kim/ and yolo-minkyuKim.h5 in [this](https://drive.google.com/file/d/18wl62z2sU3O6NUl45K7iYSzWnGlpUYzV/view?usp=sharing). After download these files, put these files in same directory and Run the codes in YOLO_test.ipynb 

* You can put these files in different locations, but if you do this, you should modify the yolo-minkyuKim.h5's path in YOLO.load_weights() which in load_YOLO()

Taeyun Kim & Seungyeon Lee : 


