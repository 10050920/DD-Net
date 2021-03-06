# DD-Net 
(A Double-feature Double-motion Network)
[![](mics/paper.png)](https://arxiv.org/pdf/1907.09658.pdf)

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/make-skeleton-based-action-recognition-model-1/skeleton-based-action-recognition-on-jhmdb-2d)](https://paperswithcode.com/sota/skeleton-based-action-recognition-on-jhmdb-2d?p=make-skeleton-based-action-recognition-model-1)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/make-skeleton-based-action-recognition-model-1/skeleton-based-action-recognition-on-shrec)](https://paperswithcode.com/sota/skeleton-based-action-recognition-on-shrec?p=make-skeleton-based-action-recognition-model-1)

JHMDB [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19gq3bUigdxIfyMCoWW93YhLEi1KQlBit)

SHREC-14 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jASRTHzsA03dZDC4yN29OK1G9L-l7jkP?usp=sharing)


# Update
Updating code to current Keras environment.

Thanks for [@muxizju](https://github.com/muxizju), [@pengfeiZhao1993](https://github.com/pengfeiZhao1993), and [@YLTsai0609](https://github.com/YLTsai0609) helped to fix bugs in this code. After fixing bugs, the performance is further improved - **JHMDB 82-83% and SHREC-14 96-97 %**.

Thanks for [Nightwatch](https://github.com/BlurryLight), who made a pytorch version DD-Net. You can check it at [Pytorch DD-Net](https://github.com/BlurryLight/DD-Net-Pytorch)

## 1.About this code
A lightweight network for body/hand action recognition, implemented by keras tensorflow backend. It also could be the simplest tutorial code to start skeleton-based action recognition.

## 2.How to use this code
### (1) clone DD-Net
```
git clone https://github.com/fandulu/DD-Net.git
```

### (2) I just noticed that the environment may not be available due to TensorFlow updating, so it is better to check the setting in [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19gq3bUigdxIfyMCoWW93YhLEi1KQlBit) and install the currently available environment

### (3) go to the folder of JHMDB or SHREC to play with ipython notebooks.
Note: You can download the raw data and use our code to preprocess them, or, directly use our preprocessed data under /data.
```
JHMDB raw data download link:   http://jhmdb.is.tue.mpg.de/challenge/JHMDB/datasets
SHREC raw data download link:   http://www-rech.telecom-lille.fr/shrec2017-hand/
```


## 3.Problems this code try to alleviate
<img src="https://github.com/fandulu/DD-Net/blob/master/mics/demo.png" width="550">

## 4.Performance
|No. parameters | SHREC-14 | SHREC-28 |
| :----: | :----: | :----: |
| 1.82 M | 94.6 | 91.9  |
| 0.15 M | 91.8| 90.0|

|No. parameters | JHMDB|
| :----: | :----: | 
| 1.82 M | 77.2|
| 0.50 M | 73.7 | 

Note: if you want to test the speed, please try to run the model.predict() at leat twice and do not take the speed of first run, the model initialization takes extra time.
## 5.Citation
If you find this code is helpful, thanks for citing our work as,
```
@inproceedings{yang2019ddnet,
  title={Make Skeleton-based Action Recognition Model Smaller, Faster and Better},
  author={Fan Yang, Sakriani Sakti, Yang Wu, and Satoshi Nakamura},
  booktitle={ACM International Conference on Multimedia in Asia},
  year={2019}
}
```
![](mics/look.gif)
*Hey, come take a look*
