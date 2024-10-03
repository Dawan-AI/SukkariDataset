---
title: Home
layout: home
nav_order: 1
---

## Table of Contents

- [Overview](#overview)
- [Dataset Structure](#dataset-structure)
- [Installation](#installation)

  
## Overview of the Sukkari Dataset
We present our ongoing efforts to construct an open-source dataset of **Sukkari dates**, a widespread variety of dates from Saudi Arabia, that are sorted and graded according to market standards. This dataset can be used for research, machine learning models, or data analysis tasks related to agriculture, food classification, or image recognition.
This dataset comprises 14,000 images, each sorted into one of five categories, as detailed in [Data Collection]({{site.baseurl}}/data_collection). 
To enhance productivity, we developed a system that automates the data collection process, which is explained in [How We Collected the Data]({{site.baseurl}}/data_collection_setup).
We also mention [how this dataset can contribute]({{site.baseurl}}/contributions) to the date palm industry and our efforts to build a sorting machine using the current dataset.
The long-term goal of this project is to commercialize a compact, low-cost machine that automates the sorting and classification of date fruits for small and medium-sized farmers.


## Dataset Structure

The dataset is organized as follows:

### Raw Dataset:


The raw dataset contains all the data collected during our data collection runs,
without any preprocessing or cleaning steps applied. Each folder in the dataset is divided into two subfolders: 
a segmentation data folder and a metadata folder.

- The segmentation data folder includes a series of images saved with the format DateId_ImageType.png.
The DateId is an integer representing the date that was captured, while the ImageType specifies the image modality, 
which could be one of the following:
  - BGR (color image)
  - NIR900 (near-infrared at 900 nm)
  - NIR970 (near-infrared at 970 nm)
  - Mask (segmentation mask)
- The metadata folder contains additional information, including:
  - Weight data
  - Frame numbers
  - Calibration files 

the raw dataset structure is as follows: 

```
┌─ ...
├─ (main label files)
├─ Label
    ├─ ...
    ├─ (run files)
    ├─ run_x
        ├─ Segmentation_Data
            ├─...
            ├─ID_RGB.png
            ├─ID_NIR900.png 
            ├─ID_NIR970.png 
            ├─ID_Mask.png
            └─...
        └─ Meta Data
            ├─...
            ├─ Weight.xlsx
            ├─ Images.xlsx 
            ├─ Notes.txt
            └─ Calibration files
    └─ (other run files)
└─(other label files)
```

### Clean Dataset:
The clean dataset consist of date images that have been cleaned and preprocessed. 
The date images are ready to be consumed by different AI models and ready for training. 
- train
  - label
    - label_001.jpg 
    - label_002.jpg
    - ...
- val
  - label
    - label_001.jpg 
    - label_002.jpg
    - ...
- test
  - label
    - label_001.jpg 
    - label_002.jpg
    - ...

## Installation
The dataset is hosted on OneDrive and is publicly accessible. It consists of two main folders: raw_dataset, 
which contains all the collected runs, and clean_dataset.zip, a zipped folder that includes the cleaned images 
along with their labels

-  [Dataset link](https://1drv.ms/f/s!Ajkda3liMT8ykeAPrZTHnwKp13D2JQ?e=R8YOhs)
