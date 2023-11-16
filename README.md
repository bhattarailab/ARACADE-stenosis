# Arcade-stenosis-task
This repo is the runner-up solution for stenosis detection task for [ARCADE challenge](https://arcade.grand-challenge.org/evaluation/final-phase-stenosis-detection-algorithm-submission/leaderboard/) at MICCAI 2023 achieving F1-score of 0.5353 on test dataset. 

![image](https://github.com/bhattarailab/ARCADE-stenosis/assets/53966090/cfdb0dd9-c520-4017-880d-1b79976e607e)

## Description
Coronary Artery Diseases although preventable are one of the leading cause of mortality worldwide. Due to the onerous nature of diagnosis, tackling CADs has proved challenging. This study addresses the automation of resource-intensive and time-consuming process of manually detecting stenotic lesions in coronary arteries in X-ray coronary angiography images. To overcome this challenge, we employ a specialized Convnext-V2 backbone based Mask RCNN model pre-trained for instance segmentation tasks. Our empirical findings affirm that the proposed model exhibits commendable performance in identifying stenotic lesions. Notably, our approach achieves a substantial F1 score of 0.5353 in this demanding task, underscoring its effectiveness in streamlining this intensive process.

You can explore the full details on this paper [here](https://arxiv.org/abs/2310.04749)

![image](https://github.com/bhattarailab/ARCADE-stenosis/assets/53966090/e9ad11d0-7fce-4576-b485-9e9f4e56d58f)


## Installation


1. Clone the repository:

```shell
git clone https://github.com/sanjaybhandarii/Arcade-stenosis-task
```

2. Then install torch and torchvision as:
```shell
pip install torch torchvision
```
3. Install MMEngine and MMCV using MIM.

```shell
pip install -U openmim
mim install mmengine
mim install "mmcv>=2.0.0"
```

4. Install mmdetection
```shell
cd mmdetection
pip install -v -e .
```
    

## Usage

Change the necessary configs in train_sten.py as per your need.

Then,to train the model:

    python train_sten.py


And to infer the model on stenosis test set, use sten_inference_demo.ipynb



