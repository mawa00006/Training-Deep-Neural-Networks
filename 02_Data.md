# Chapter 2: Data

## 1. Databases
Whether you are working on a DL project for fun, research, or as a work project, the size and quality
of the dataset you are working with is crucial. In the following a will present some databases that you 
can use as a starting point for a new project, or to supplement your existing datasets. 

### [Kaggle](https://www.kaggle.com)
Kaggle is a web-based platform for data science and machine learning competitions, where users can find and publish datasets, explore and build models, and enter competitions to solve challenges.
You can find datasets in any form, from any domain.

### [The Image Data Resource (IDR)](https://idr.openmicroscopy.org)
The Image Data Resource (IDR) is a public repository of image datasets from published scientific studies, where the community can submit, search and access high-quality bio-image data.

### [Cell Image Library](http://cellimagelibrary.org/home)
This library is a public and easily accessible resource database of images, videos, and animations of cells, capturing a wide diversity of organisms, cell types, and cellular processes. The purpose of this database is to advance research on cellular activity, with the ultimate goal of improving human health.

### [WHO data collections](https://www.who.int/data/collections)
The World Health Organization manages and maintains a wide range of data collections related to global health and well-being as mandated by our Member States.

### [Open Source Imaging Consortium (OSIC)](https://www.osicild.org)
The OSIC Data Repository was built with the expertise and help of global radiologists, pulmonologists, machine learners, and imaging experts from industry and academia. It is a data-rich repository of anonymized HRCT scans and clinical information regarding interstitial lung diseases (ILDs), and houses a plethora of real world clinical and imaging data that is both multi-ethnic and multi-center.

### [The Structural Antibody Database (SAbDab)](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabdab)
SAbDab is a database containing all the antibody structures available in the PDB, annotated and presented in a consistent fashion.


## Overview
|Name|    Domain     |  Type of Data  |
|:-:|:-------------:|:--------------:|
|[Kaggle](https://www.kaggle.com)|      Any      |      Any       |
|[The Image Data Resource (IDR)](https://idr.openmicroscopy.org)|  Bioimaging   |     Images     |
|[Cell Image Library](http://cellimagelibrary.org/home)|  Bioimaging   | Images, Videos |
|[WHO data collections](https://www.who.int/data/collections)|    Health     |      XLSX      |
|[Open Source Imaging Consortium (OSIC)](https://www.osicild.org)| Lung Diseases |     Images     |
|[The Structural Antibody Database (SAbDab)](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabdab)|  Antibodies   |      PDB       |
#### Interesting Datasets
Collection of datasets I find personally interesting.
- [Brain Tumor Segmentation(BraTS2020)](https://www.kaggle.com/datasets/awsaf49/brats2020-training-data)

Become one with the data
- inspect data (understand distribution, look for patterns)
	- corrupted data/labels?
	- data imbalances/biases?
	- visualizations distribution (e.g. type of label, size of annotations, number of annotations, image size, average sentence length) and outliers
	- Split data into train/test/eval
		- is the training data representative 
		- is there information leakage between the train/test/val data
		- is the distribution of the validation data similar to the data in the production environment
	- implement dataloader
	- visualize data just before passing it into the model (raw tensor data/labels)
	- What are important metrics?
	- Which loss function should be used? (Do we need a custom loss?)
