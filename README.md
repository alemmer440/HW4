## Allison Lemmer HW4

# Repository Overview

This repository contains paired mRNA and microRNA data files from 1,097 breast cancer patients from the The Cancer Genome Atlas. It has code to generate a heatmap showing the levels of 30 of the microRNAs for 10 of the patients, as a means to begin exploring the data. The 

# Data

All data is pulled from the National Cancer Institute GDC Data Portal. Specifically, we filtered for patients from The Cancer Genome Atlas that had breast cancer and both mRNA and microRNA data files. When downloaded, the data came in a highly nested directory, so we flattened all of the files into one directory. We also downloaded the associated json file containing the metadata, from which we can determine which files belong to each patient. 

# Folder Structure

The Data folder has all of the data and metadata. The data files are all zipped in one folder, and the metadata is all in the json file. The Scripts folder contains the jupyter notebook code used to generate the figure in the Figures folder. 

# Installation

git clone https://github.com/alemmer440/HW4.git

