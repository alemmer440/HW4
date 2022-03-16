# Allison Lemmer HW4

## Repository Overview

This repository contains paired mRNA and microRNA data files from 1,097 breast cancer patients from The Cancer Genome Atlas. It has code to generate a heatmap showing the levels of 30 of the microRNAs for 10 of the patients, as a means to begin exploring the data. 

## Data

All data is pulled from the National Cancer Institute GDC Data Portal, which can be found at this link: https://portal.gdc.cancer.gov/. Specifically, we filtered for female breast cancer patients from The Cancer Genome Atlas project that had both mRNA and microRNA data files. For mRNA files, we selected the versions using FPKM normalization, and for microRNAs we selected the version without isoforms. When downloaded, the data came in a highly nested directory, so we flattened all of the files into one directory. We also downloaded the associated json file containing the metadata, from which we can determine which files belong to each patient based on the file Case IDs.

## Folder Structure

The Data folder has all of the data and metadata. The data files are all zipped in one folder titled GDC\_Data.zip, and the metadata is all in the GDC\_Metadata.json file. The Scripts folder contains the jupyter notebook used to generate the figure in the Figures folder. 

## Installation

The code runs using python3.

The following packages are required for the code to run, and were all installed using conda:
* Jupyter Notebook
* Numpy
* Json
* Seaborn
* Matplotlib

A list of package versions for the environment the code was created in, and the command you can use to create the same conda enviroment, in is in the file requirements.txt. Alternatively, these packages can be installed using pip. 

Once the necessary packages are installed, run the following command:  
git clone https://github.com/alemmer440/HW4.git

Then, navigate in the folder to Data/GDC\_Data.zip and unzip the file.

Finally, navigate to Scripts/Generate\_Plot.ipynb. Open the jupyter notebook, run all cells, and the figure will output in the Figures folder.
