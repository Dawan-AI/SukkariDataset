# SukkariDataset

## Sukkari Dates Dataset

This repository contains a dataset of **Sukkari Dates**, a popular variety of dates from Saudi Arabia. This dataset can be used for research, machine learning models, or data analysis tasks related to agriculture, food classification, or image recognition.

## Table of Contents

- [Overview](#overview)
- [Dataset Structure](#dataset-structure)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Contributing](#contributing)

## Overview
We present our efforts to construct an open source dataset of Sukkari dates that are sorted
and graded based on market standards. We chose Sukkari dates because of the complexity of their grading
criteria and their widespread availability. This dataset comprises 14,000 images, each sorted
into one of five categories.

## Dataset Structure

The dataset is organized as follows:

### Raw Dataset:
The rew dataset consists of all data collected during our data collection runs. There is no preprocessing or any cleaning steps during collection. 
each folder in the dataset consists of segmentation data and meta data folders. 
segmentatoin data folder contains a list of images saved with DateId_ImageType.png. date id is an integer to represent date captured. Image type could be either BGR, NIR900, NIR970, or Mask. 
the other folder is meta data folder which contains weight information, frame numbers information, and calibration files. 

the raw dataset structure is as follows: 
- Label:
  - run_x:
    - Data: 
      - ID_RGB.png 
      - ID_NIR900.png 
      - ID_NIR970.png 
      - ID_Mask.png 
    - Meta Data 
      - Weight.xlsx 
      - Images.xlsx 
      - Calibration files
      - Notes.txt: 
        - Example: {Label:Galaxy, Date of Collection : %Y-%m-%d %H:%M, Motor 1 Speed: X, Motor 2 Speed: X}

### Clean Dataset:
The clean dataset consist of date images that have been cleaned and preprocessed. 
The date images are ready to be consumed by different AI models and ready for training. 
- train
  - Mufattal
    - mufattal_001.jpg 
  - Qisher
    - qisher_001.jpg
  - Rutab
    - rutab_001.jpg)
  - Galaxy
    - galaxy_001.jpg
  - Nagad
    - nagad_001.jpg)
- val
  - Mufattal
    - mufattal_003.jpg
  - Qisher
    - qisher_003.jpg
  - Rutab
    - rutab_003.jpg
  - Galaxy
    - galaxy_003.jpg
  - Nagad
    - nagad_003.jpg
- test
  - Mufattal
    - mufattal_004.jpg
  - Qisher
    - qisher_004.jpg)
  - Rutab
    - rutab_004.jpg
  - Galaxy
    - galaxy_004.jpg
  - Nagad
    - nagad_004.jpg)
- ....
