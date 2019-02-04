# DL-RootAnatomy: Root Anatomy Using Faster RCNN
Web-based application available at: https://rootanatomy.org/ <br />
Mobile friendly, no installation required, no coding skills required <br />
##
__DL-RootAnatomy__ detects root, stele and late metaxylm objects using Faster RCNN. The models are trained with around 300 images, including our own dataset and several images from RootAnalyzer (10 images) and RootCell (6 images).  <br />

![Rootnatomy Image](https://i.ibb.co/jH4g7sY/Screen-Shot-2019-01-20-at-4-47-08-PM.png) <br /> 

## Content of the Repository
__tf-faster-rcnn (stele&root)__ is the code for training the model for detection the root and stele in an image <br />
__tf-faster-rcnn (lm)__ is the code for training the model for detecting the late metaxylm objects <br />
__model__ folder cantains the models trained with about 300 images, including images in our dataset, and several images from Rootanalyzer (10 images) and RootCell (6 images). <br />

## Train:
See below the command to start the training: <br />

nohup ./experiments/scripts/train_faster_rcnn.sh 0 pascal_voc vgg16 &

## Predict:
See below the command to visualize the prediction results, and find the root/stele diameter and late metaxylem count and average diameter:
 <br />./tools/demo.py


