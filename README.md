# MSCT
Small Target Cluster Tracking Method Based on Memory Enhancement

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

## Datasets

- Download training datasets from here
- Download testing datasets from here

## Training

Modify the path of the training set in the train.py folder, and finally execute the command in the terminal

```
python deep/train.py --data-dir=../deatsets/train/train1
```

## Testing

- First obtain the key point coordinates through FIDTM
- Use convert.py to convert the obtained key point coordinates to the format
- Modify the file path in test.py, and execute the command on the terminal to obtain ReID information

```
python deep/test.py
```

- Execute the command in the terminal to get the trace result

```
python memory_tracking.py --sequence_dir=./deatsets/test/test1 --detection_file=./resources/test1.npy --display=True
```

## References
