# 2d_to_3d_human_pose_converter

This module is for converting 2d human upper body poses to 3d.  
It is a part of [co-speech gesture generation project](https://sites.google.com/view/youngwoo-yoon/projects/co-speech-gesture-generation).  
You can find out more details in the paper.


## Installation
The scripts are tested on Windows 10 and Anaconda Python 3.6 (64 bit).  
CUDA Toolkit 9.0 is installed for GTX 1080 Ti.  

You need to install the following modules.  
$ numpy matplotlib pyquaternion scipy  
$ [conda install pytorch==1.1.0 torchvision==0.3.0 cudatoolkit=9.0 -c pytorch](https://pytorch.org/get-started/previous-versions/)



## How to run
* download [CMU panoptic dataset](http://domedb.perception.cs.cmu.edu/)
* run generate_dataset.py to make a single pickle file for training
* run train.py to train the simple neural network that estimates depth values from 2d poses
* run test.py to test the trained model
