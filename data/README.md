# TNDC: Table Net Detection and Classification
## Abstract 

## Getting Started
### Install MMDetection v2.10.0+
TNDC has been implemented and tested with Python 3.7 and PyTorch 1.8.1. 
```
%cd $project_dir$
!pip install -q mmcv terminaltables
!git clone 'https://github.com/open-mmlab/mmdetection.git'
!pip install -r "$project_dir$/mmdetection/requirements/optional.txt"
%cd mmdetection/
!python setup.py install
!python setup.py develop
!pip install -r {"$project_dir$/mmdetection/requirements.txt"}
!pip install pillow
!pip install mmcv
!pip install mmcv-full
%cd ..
!pip uninstall pycocotools
!pip uninstall mmpycocotools
!pip install mmpycocotools
```

## Data Prepration 
You should convert your Pascal VOC XML annotation files to a single COCO Json file so we can train our models.
The Raw folder for the data should be like below, then used generateVOC2JSON.py

    .
    │   ├── data
    │   │   ├── TNDC Dataset
    │   │   │  ├── Annotations
    │   │   │  │    ├── 000ad0bb60e1ec4176713693a41f2115.xml
    │   │   │  │    ├── ...
    │   │   │  │    ├── ffda050fe78074f78b874540ad218fb9.xml
    │   │   │  ├── ImageSets
    │   │   │  │    ├── Main 
    │   │   │  │    │     ├── test.txt
    │   │   │  │    │     ├── train.txt
    │   │   │  │    │     ├── val.txt
    │   │   │  ├── Images
    │   │   │  │    ├── 000ad0bb60e1ec4176713693a41f2115.jpg
    │   │   │  │    ├── ...
    │   │   │  │    ├── ffda050fe78074f78b874540ad218fb9.jpg
    │   │   │  ├── Output Json
    ├── generateVOC2JSON.py   
## requirements

## Cite as
If you find this work useful for your research, please cite our paper:
```
```


