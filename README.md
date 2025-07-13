# MSCT
A Memory-enhanced Small-target Cluster Tracking Method for Unduplicated Crowd Counting in Aerial Videos. This repository contains a [Pytorch](https://pytorch.org/) implementation for our [MSCT](https://yzueducn-my.sharepoint.com/:f:/g/personal/zhangxf_yzu_edu_cn/EktMPSTpJndHgUtb7NMnZeoBDlEyAhjwngS2CR9n2_maaQ). Our code is released only for scientific or personal use. Please contact us for commercial use.

## Introduction

## Environment

```
python >=3.6 
pytorch >=1.4
opencv-python >=4.0
scipy >=1.4.0
h5py >=2.10
pillow >=7.0.0
imageio >=1.18
nni >=2.0 (python3 -m pip install --upgrade nni)
```

## Aerial Crowd Datasets

Download Aerial dataset from this [link](https://yzueducn-my.sharepoint.com/:f:/g/personal/zhangxf_yzu_edu_cn/Erzew7eKpgREjqZ7b-ZpAZwBpI-0bHFdFXFodMxRs4iEGw?e=QacvhV)

## Training

Modify the path of the training set in the train.py folder, and finally execute the command in the terminal

```
python Impressed/train.py --data-dir=../deatsets/train/train1
```

## Testing

- First obtain the key point coordinates through FIDTM
- Use convert.py to convert the obtained key point coordinates to the format
- Modify the file path in test.py, and execute the command on the terminal to obtain impressed memory information

```
python impressed/test.py
```

- Execute the command in the terminal to get the trace result

```
python MSCT.py --sequence_dir=./deatsets/test/test1 --detection_file=./resources/test1.npy --display=True
```

## Demo
![img](imgs/demo1.gif)

![img](imgs/demo2.gif)

![img](imgs/demo3.gif)

![img](imgs/demo4.gif)

## References
