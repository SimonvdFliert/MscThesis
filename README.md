# Worth More Than Gold
## A Master Thesis of model diagnostics in Transformers in the field of NLG
This repository contains the data and code used for my Master thesis in Natural Language Generation

[[https://github.com/SimonvdFliert/MscThesis/blob/main/Gold.jpg|alt=octocat]]
Table of Contents
=================

   * [Worth More Than Gold](#Worth-More-Than-Gold)
      * [Table of Contents](#table-of-contents)
      * [Installation](#installation)
      * [Background readings in NLG](#Background-readings-in-NLG)
      * [Repository Overview](#Repository-Overview)


## Installation
From Google Colab
All Colab files contain the required packages within the first cell. Run this cell and you should be good to go!
```
!pip install git+https://github.com/huggingface/datasets.git
!pip install rouge_score
!pip install sentencepiece
!pip install transformers
```

## Background readings in NLG
For those unfamiliar with NLG, below are some fantastic starting points
1. [Survey of the State of the Art in Natural Language Generation: Core tasks, applications and evaluation](https://www.jair.org/index.php/jair/article/view/11173)
2. [Pre-trained Language Models for Text Generation: A Survey](https://arxiv.org/pdf/2201.05273.pdf)
3. [Neural Natural Language Generation: A Survey on Multilinguality, Multimodality, Controllability and Learning](https://www.jair.org/index.php/jair/article/view/12918)
4. [Decoding Methods in Neural Language Generation: A Survey](https://www.mdpi.com/2078-2489/12/9/355)

## Repository Overview
This file contains several documents.

### CACAPO Data
The CACAPO data has been stored in the file named Data. Within this, several subfolders can be found.
1. CACAPO: The original CACAPO dataset retrievable from [Dataverse](https://dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/LIBYHP)
2. Cleaned_data: The originaltriples and texts extracted from the Original Dataset to train End-to-End systems
3. Cleaned_continuous: Used for the continuous experiment, where splits are made for each subject
4. Augmented_data: The dataset created by the script in "Data Augmentation Experiment", contains roughly 42K records compared to the original 20K
5. Elongated_data: The dataset that has been manually elongated with additional contextual input
6. GEM datasets: The datasets from different experiments adapted for the GEM Benchmark
7. Pickled_attributes: This folder contains pickles of the attributes stored within the entire dataset and also split per subject and language

### Code
This folder contains the code written for this project. Within this file is both the WebNLG_xmlReader (taken and not adapted from the WebNLG challenge) and Evaluation_Code. In the latter folder are two files, an file containing the unaltered BARTScore code and a file for the altered PARENT code.

### Manual_eval
This file contains all Excel and CSV documents that have been used during manual review sessions in this project.
