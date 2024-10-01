# SukkariDataset
Sukkari Dates Dataset
This repository contains a dataset of Sukkari Dates, a popular variety of dates from Saudi Arabia. This dataset can be used for research, machine learning models, or data analysis tasks related to agriculture, food classification, or image recognition.

Table of Contents
Overview
Dataset Structure
Installation
Usage
License
Contributing

Overview
The Sukkari Dates dataset includes high-quality data points and images related to this specific type of date. It can be used for tasks such as:

Classification of date varieties.
Analyzing the physical properties of dates.
Building machine learning models for quality analysis.

Dataset Structure
The dataset is organized as follows:
Raw dataset: 
  Label: 
    run_x: 
      Data 
        ID_RGB.png 
        ID_NIR900.png
        ID_NIR970.png
        ID_Mask.png
      Meta Data
        Weight.xlsx
        Images.xlsx
        Calibration files  
        Notes.txt 
          {label:Galaxy, Collection data : X.X.XXXX, Motor1_speed: X, Motor2_speed: X} 
Clean Dataset: 
/dataset
├── train/
│   ├── Mufattal/
│   │   ├── mufattal_001.jpg
│   │   └── ...
│   ├── Qisher/
│   │   ├── qisher_001.jpg
│   │   └── ...
│   ├── Rutab/
│   │   ├── rutab_001.jpg
│   │   └── ...
│   ├── Galaxy/
│   │   ├── galaxy_001.jpg
│   │   └── ...
│   └── Nagad/
│       ├── nagad_001.jpg
│       └── ...
│
├── val/
│   ├── Mufattal/
│   │   ├── mufattal_003.jpg
│   │   └── ...
│   ├── Qisher/
│   │   ├── qisher_003.jpg
│   │   └── ...
│   ├── Rutab/
│   │   ├── rutab_003.jpg
│   │   └── ...
│   ├── Galaxy/
│   │   ├── galaxy_003.jpg
│   │   └── ...
│   └── Nagad/
│       ├── nagad_003.jpg
│       └── ...
│
└── test/
    ├── Mufattal/
    │   ├── mufattal_004.jpg
    │   └── ...
    ├── Qisher/
    │   ├── qisher_004.jpg
    │   └── ...
    ├── Rutab/
    │   ├── rutab_004.jpg
    │   └── ...
    ├── Galaxy/
    │   ├── galaxy_004.jpg
    │   └── ...
    └── Nagad/
        ├── nagad_004.jpg
        └── ...

