# ReLayNet
[ReLayNet: Retinal Layer and Fluid Segmentation of Macular Optical Coherence Tomography using Fully Convolutional Network](https://arxiv.org/abs/1704.02161)

This repository contains the implementation(partly) of a convolutional neural network used to segment retinal layers and fluid in eye OCT scans,termed ReLayNet. ReLayNet is based on U-Net architecture and is trained to optimize a joint loss function comprising ofweighted logistic regression and Dice overlap loss.

# DataSets

The Duke SD-OCT publicly available dataset for DME patients. The dataset consists of 110 annotated SD-OCT B-scan images of size 512 × 740 obtained from 10 patients suffering from DME (11 B-scans per patient). The 11 B-scans per patient were annotated centered at fovea and 5 frames on either side of the fovea (foveal slice and scans laterally acquired at ±2, ±5, ±10, ±15 and ± 20 from the foveal slice). These 110 B-scans are annotated for the retinal layers and fluid regions by two expert clinicians. The details of this datasets in this [home-page](http://people.duke.edu/~sf59/Chiu_BOE_2014_dataset.htm).
# Results in paper

![image](https://github.com/Atomwh/ReLayNet/blob/master/image-folder/TIM%E6%88%AA%E5%9B%BE20180124162701.png)

# Results in this code

![results](https://github.com/Atomwh/ReLayNet/blob/master/image-folder/result.png)

![compare](https://github.com/Atomwh/ReLayNet/blob/master/image-folder/compare.png)

The (a) is the segmentation of this code and (b) is the ground truth.

The Final `dice_coef` is `0.957`
# ToDo
·Add Fluid segmentation
·Add the implementation of UNpooling with pooling indics
